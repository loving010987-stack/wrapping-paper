[포장지만들기 (2).html](https://github.com/user-attachments/files/28572231/2.html)
<!DOCTYPE html>
<html lang="ko">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>🎁 나만의 포장지 만들기</title>
<style>
*{box-sizing:border-box;margin:0;padding:0;}
body{font-family:'Apple SD Gothic Neo','Noto Sans KR',sans-serif;background:#fff;}
.wrap{padding:12px;}
.top-bar{text-align:center;margin-bottom:14px;}
.top-bar h1{font-size:22px;font-weight:700;color:#333;}
.top-bar p{font-size:13px;color:#888;margin-top:4px;}
.steps{display:flex;gap:6px;justify-content:center;margin-bottom:14px;flex-wrap:wrap;}
.step{background:#f0f0f0;border-radius:20px;padding:5px 14px;font-size:12px;color:#888;font-weight:500;}
.step.active{background:#FFD600;color:#333;}
.main{display:flex;gap:14px;flex-wrap:wrap;}
.left{flex:0 0 auto;display:flex;flex-direction:column;gap:10px;}
.right{flex:1;min-width:260px;}
.panel{background:#fafafa;border:1px solid #eee;border-radius:12px;padding:10px;}
.panel-title{font-size:11px;font-weight:700;color:#aaa;letter-spacing:.06em;text-transform:uppercase;margin-bottom:8px;}
canvas{display:block;touch-action:none;}
#drawCanvas{border:3px dashed #ddd;border-radius:10px;cursor:crosshair;background:white;}
#tessCanvas{border:2px solid #eee;border-radius:10px;background:white;}
.color-grid{display:grid;grid-template-columns:repeat(5,1fr);gap:5px;}
.cbtn{width:32px;height:32px;border-radius:50%;border:3px solid transparent;cursor:pointer;transition:transform .1s;}
.cbtn.on{border-color:#333;transform:scale(1.2);}
.row{display:flex;gap:6px;align-items:center;}
.row input[type=range]{flex:1;}
.row span{font-size:12px;color:#555;min-width:20px;text-align:right;}
.tbtn{flex:1;padding:7px 4px;font-size:12px;border:1.5px solid #ddd;border-radius:8px;background:white;cursor:pointer;color:#555;text-align:center;line-height:1.4;}
.tbtn:hover{background:#f5f5f5;}
.tbtn.on{background:#E8F5E9;color:#2E7D32;border-color:#81C784;}
.abtn{width:100%;padding:9px;font-size:13px;border:1.5px solid #ddd;border-radius:9px;background:white;cursor:pointer;color:#555;font-weight:500;}
.abtn:hover{background:#f5f5f5;}
.clear-btn{background:#FFF3E0;color:#E65100;border-color:#FFCC80;}
.clear-btn:hover{background:#FFE0B2;}
.make-btn{background:#FFD600;border:none;color:#333;font-size:15px;font-weight:700;padding:12px;border-radius:12px;width:100%;cursor:pointer;margin-top:4px;}
.make-btn:hover{background:#FFC107;}
.dl-btn{background:#4CAF50;border:none;color:white;font-size:14px;font-weight:700;padding:11px;border-radius:12px;width:100%;cursor:pointer;margin-top:8px;display:none;}
.dl-btn:hover{background:#388E3C;}
.tess-btns{display:grid;grid-template-columns:1fr 1fr;gap:5px;}
.undo-row{display:flex;gap:6px;}
.undo-row button{flex:1;}
.hint{font-size:11px;color:#aaa;text-align:center;margin-top:4px;}
#modeDesc{font-size:12px;color:#555;margin-top:8px;text-align:center;background:#f9f9f9;border-radius:8px;padding:6px;}
.celebrate{display:none;text-align:center;font-size:28px;}
</style>
</head>
<body>
<div class="wrap">
  <div class="top-bar">
    <h1>🎁 나만의 포장지 만들기</h1>
    <p>초등 4학년 · 평면도형의 이동</p>
  </div>
  <div class="steps">
    <div class="step active" id="s1">① 타일 그리기</div>
    <div class="step" id="s2">② 변환 고르기</div>
    <div class="step" id="s3">③ 포장지 완성!</div>
  </div>

  <div class="main">
    <div class="left">
      <div class="panel">
        <div class="panel-title">🎨 색깔</div>
        <div class="color-grid" id="colorGrid"></div>
      </div>
      <div class="panel">
        <div class="panel-title">✏️ 굵기</div>
        <div class="row">
          <input type="range" id="thick" min="3" max="28" value="8" step="1">
          <span id="thickN">8</span>
        </div>
      </div>
      <div class="panel">
        <div class="panel-title">🖊 도구</div>
        <div class="row">
          <button class="tbtn on" id="penBtn">✏️ 펜</button>
          <button class="tbtn" id="erBtn">🧽 지우개</button>
        </div>
      </div>
      <div class="undo-row">
        <button class="abtn" id="undoBtn">↶ 취소</button>
        <button class="abtn" id="redoBtn">↷ 다시</button>
      </div>
      <button class="abtn clear-btn" id="clearBtn">🧹 전체 지우기</button>
      <div class="hint">가장자리까지 그리면 더 멋져요!</div>
      <canvas id="drawCanvas" width="200" height="200"></canvas>
    </div>

    <div class="right">
      <div class="panel" style="margin-bottom:10px;">
        <div class="panel-title">🔄 변환 방식</div>
        <div class="tess-btns">
          <button class="tbtn on" data-m="translate">➡️ 밀기</button>
          <button class="tbtn" data-m="flipH">↔️ 좌우 뒤집기</button>
          <button class="tbtn" data-m="flipV">↕️ 위아래 뒤집기</button>
          <button class="tbtn" data-m="rot90">🔄 90° 돌리기</button>
          <button class="tbtn" data-m="rot180">🔁 180° 돌리기</button>
          <button class="tbtn" data-m="random">🎲 섞기</button>
        </div>
        <div id="modeDesc">같은 모양을 그대로 반복해요</div>
      </div>

      <button class="make-btn" id="makeBtn">✨ 포장지 만들기!</button>
      <div class="celebrate" id="celebrate">🎉🎁🎊</div>
      <canvas id="tessCanvas" width="480" height="400" style="margin-top:8px;width:100%;max-width:480px;"></canvas>
      <button class="dl-btn" id="dlBtn">📥 이미지 저장하기</button>
      <div class="hint" id="dlHint" style="display:none;">저장한 이미지를 인쇄하면 진짜 포장지가 돼요! 🖨️</div>
    </div>
  </div>
</div>

<script>
const COLORS=['#e74c3c','#e67e22','#f1c40f','#27ae60','#1abc9c','#3498db','#9b59b6','#e91e8c','#795548','#222222'];
const DESC={
  translate:'➡️ 같은 모양을 그대로 반복해요 (밀기)',
  flipH:'↔️ 한 칸씩 좌우로 뒤집어서 반복해요',
  flipV:'↕️ 한 칸씩 위아래로 뒤집어서 반복해요',
  rot90:'🔄 90°씩 돌려서 반복해요 (4방향)',
  rot180:'🔁 180°씩 돌려서 반복해요 (2방향)',
  random:'🎲 여러 방법을 섞어서 반복해요'
};

let curColor=COLORS[9], eraser=false, drawing=false, lx, ly, mode='translate';
let history=[], future=[];

// 색깔 버튼
const cg=document.getElementById('colorGrid');
COLORS.forEach(c=>{
  const b=document.createElement('button');
  b.className='cbtn'+(c===curColor?' on':'');
  b.style.background=c;
  b.onclick=()=>{
    curColor=c; eraser=false;
    document.querySelectorAll('.cbtn').forEach(x=>x.classList.remove('on'));
    b.classList.add('on');
    document.getElementById('penBtn').classList.add('on');
    document.getElementById('erBtn').classList.remove('on');
  };
  cg.appendChild(b);
});

// 굵기
const thickEl=document.getElementById('thick');
const thickN=document.getElementById('thickN');
thickEl.oninput=()=>thickN.textContent=thickEl.value;

// 도구
document.getElementById('penBtn').onclick=()=>{
  eraser=false;
  document.getElementById('penBtn').classList.add('on');
  document.getElementById('erBtn').classList.remove('on');
};
document.getElementById('erBtn').onclick=()=>{
  eraser=true;
  document.getElementById('erBtn').classList.add('on');
  document.getElementById('penBtn').classList.remove('on');
};

// 캔버스 그리기
const dc=document.getElementById('drawCanvas');
const dctx=dc.getContext('2d');
dctx.fillStyle='white';
dctx.fillRect(0,0,200,200);
history.push(dctx.getImageData(0,0,200,200));

function getP(e){
  const r=dc.getBoundingClientRect();
  const sx=200/r.width, sy=200/r.height;
  if(e.touches) return [(e.touches[0].clientX-r.left)*sx,(e.touches[0].clientY-r.top)*sy];
  return [(e.clientX-r.left)*sx,(e.clientY-r.top)*sy];
}
function dot(x,y){
  dctx.beginPath();
  dctx.arc(x,y,parseInt(thickEl.value)/2,0,Math.PI*2);
  dctx.fillStyle=eraser?'white':curColor;
  dctx.fill();
}
function line(x1,y1,x2,y2){
  dctx.beginPath();
  dctx.moveTo(x1,y1);
  dctx.lineTo(x2,y2);
  dctx.strokeStyle=eraser?'white':curColor;
  dctx.lineWidth=parseInt(thickEl.value);
  dctx.lineCap='round';
  dctx.lineJoin='round';
  dctx.stroke();
}
function saveH(){
  history.push(dctx.getImageData(0,0,200,200));
  if(history.length>50) history.shift();
  future=[];
}
function startD(e){e.preventDefault();drawing=true;saveH();[lx,ly]=getP(e);dot(lx,ly);}
function moveD(e){e.preventDefault();if(!drawing)return;const[x,y]=getP(e);line(lx,ly,x,y);[lx,ly]=[x,y];}
function endD(e){e.preventDefault();drawing=false;}

dc.addEventListener('mousedown',startD);
dc.addEventListener('mousemove',moveD);
dc.addEventListener('mouseup',endD);
dc.addEventListener('mouseleave',endD);
dc.addEventListener('touchstart',startD,{passive:false});
dc.addEventListener('touchmove',moveD,{passive:false});
dc.addEventListener('touchend',endD,{passive:false});

document.getElementById('undoBtn').onclick=()=>{
  if(history.length>1){future.push(history.pop());dctx.putImageData(history[history.length-1],0,0);}
};
document.getElementById('redoBtn').onclick=()=>{
  if(future.length){const s=future.pop();history.push(s);dctx.putImageData(s,0,0);}
};
document.getElementById('clearBtn').onclick=()=>{
  saveH();dctx.fillStyle='white';dctx.fillRect(0,0,200,200);
};

// 변환 방식 선택
document.querySelectorAll('.tess-btns .tbtn').forEach(btn=>{
  btn.onclick=()=>{
    mode=btn.dataset.m;
    document.querySelectorAll('.tess-btns .tbtn').forEach(b=>b.classList.remove('on'));
    btn.classList.add('on');
    document.getElementById('modeDesc').textContent=DESC[mode]||'';
    document.getElementById('s2').classList.add('active');
  };
});

// ★ 핵심: 타일 변환 함수 ★
// angle: 0, 90, 180, 270 (도)
// flipH: 좌우반전, flipV: 상하반전
function makeTile(srcCanvas, angle, flipH, flipV) {
  const t = document.createElement('canvas');
  t.width = 200; t.height = 200;
  const c = t.getContext('2d');
  c.save();
  c.translate(100, 100); // 중심으로 이동
  if(flipH) c.scale(-1, 1);
  if(flipV) c.scale(1, -1);
  c.rotate(angle * Math.PI / 180);
  c.drawImage(srcCanvas, -100, -100);
  c.restore();
  return t;
}

// 셀(row, col)에 맞는 타일 반환
function getCell(row, col, srcCanvas, m) {
  if(m === 'translate') {
    // 밀기: 모두 동일
    return makeTile(srcCanvas, 0, false, false);
  }
  else if(m === 'flipH') {
    // 좌우뒤집기: 짝수열=원본, 홀수열=좌우반전
    return makeTile(srcCanvas, 0, col % 2 !== 0, false);
  }
  else if(m === 'flipV') {
    // 위아래뒤집기: 짝수행=원본, 홀수행=상하반전
    return makeTile(srcCanvas, 0, false, row % 2 !== 0);
  }
  else if(m === 'rot90') {
    // 90°돌리기: (row+col)%4 → 0°, 90°, 180°, 270°
    const angles = [0, 90, 180, 270];
    return makeTile(srcCanvas, angles[(row + col) % 4], false, false);
  }
  else if(m === 'rot180') {
    // 180°돌리기: (row+col)%2 → 0°, 180°
    return makeTile(srcCanvas, (row + col) % 2 === 0 ? 0 : 180, false, false);
  }
  else if(m === 'random') {
    // 섞기: 랜덤
    const modes = ['translate','flipH','flipV','rot90','rot180'];
    return getCell(row, col, srcCanvas, modes[Math.floor(Math.random()*modes.length)]);
  }
  return makeTile(srcCanvas, 0, false, false);
}

// 포장지 생성
const tc = document.getElementById('tessCanvas');
const tctx = tc.getContext('2d');

document.getElementById('makeBtn').onclick = () => {
  const sz = 80, cols = 6, rows = 5;
  tctx.clearRect(0, 0, 480, 400);

  // 원본 타일 복사
  const src = document.createElement('canvas');
  src.width = 200; src.height = 200;
  src.getContext('2d').drawImage(dc, 0, 0);

  for(let r = 0; r < rows; r++) {
    for(let c = 0; c < cols; c++) {
      const tile = getCell(r, c, src, mode);
      tctx.drawImage(tile, c * sz, r * sz, sz, sz);
    }
  }

  // 격자선 (옅게)
  tctx.strokeStyle = 'rgba(0,0,0,0.06)';
  tctx.lineWidth = 0.5;
  for(let c = 0; c <= cols; c++){
    tctx.beginPath(); tctx.moveTo(c*sz, 0); tctx.lineTo(c*sz, rows*sz); tctx.stroke();
  }
  for(let r = 0; r <= rows; r++){
    tctx.beginPath(); tctx.moveTo(0, r*sz); tctx.lineTo(cols*sz, r*sz); tctx.stroke();
  }

  document.getElementById('s3').classList.add('active');
  const cel = document.getElementById('celebrate');
  cel.style.display = 'block';
  setTimeout(()=>cel.style.display='none', 1500);
  document.getElementById('dlBtn').style.display = 'block';
  document.getElementById('dlHint').style.display = 'block';
};

// 이미지 저장
document.getElementById('dlBtn').onclick = () => {
  const merged = document.createElement('canvas');
  merged.width = 480; merged.height = 400;
  const mctx = merged.getContext('2d');
  mctx.fillStyle = 'white';
  mctx.fillRect(0, 0, 480, 400);
  mctx.drawImage(tc, 0, 0);
  const a = document.createElement('a');
  a.download = '나만의_포장지.png';
  a.href = merged.toDataURL('image/png');
  a.click();
};
</script>
</body>
</html>
