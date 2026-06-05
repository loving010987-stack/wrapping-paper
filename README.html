[aziit_design_v4.html](https://github.com/user-attachments/files/28623592/aziit_design_v4.html)
<!DOCTYPE html>
<html lang="ko">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>나만의 원룸 아지트 설계하기</title>
<link href="https://fonts.googleapis.com/css2?family=Nanum+Gothic:wght@400;700;800&display=swap" rel="stylesheet">
<style>
*{box-sizing:border-box;margin:0;padding:0;}
body{font-family:'Nanum Gothic',sans-serif;background:#f5f0e8;min-height:100vh;}
.header{background:#3d5a4a;padding:14px 20px;}
.header h1{font-size:17px;font-weight:800;color:#fff;}
.header p{font-size:11px;color:#a8c8b8;margin-top:2px;}
.step-bar{display:flex;border-bottom:1px solid #e0d8cc;overflow-x:auto;}
.step-tab{flex:1;min-width:60px;padding:9px 4px;text-align:center;font-size:10px;font-weight:700;color:#aaa;background:#faf7f2;border-right:1px solid #e0d8cc;cursor:default;white-space:nowrap;}
.step-tab.active{background:#fff;color:#3d5a4a;border-bottom:2px solid #3d5a4a;}
.step-tab.done{color:#3d5a4a;background:#f0f5f2;}
.step-tab .num{display:block;font-size:14px;margin-bottom:1px;}
.page{display:none;padding:16px;max-width:640px;margin:0 auto;}
.page.show{display:block;}
.card{background:#fff;border-radius:12px;padding:16px;margin-bottom:12px;box-shadow:0 1px 4px rgba(0,0,0,0.07);}
.card h2{font-size:15px;font-weight:800;color:#3d5a4a;margin-bottom:4px;}
.card p{font-size:12px;color:#888;line-height:1.6;margin-bottom:10px;}
.quiz-box{background:#fff8e8;border:1.5px solid #f0c040;border-radius:10px;padding:12px;margin-bottom:10px;}
.quiz-box .qlabel{font-size:13px;font-weight:700;color:#b07000;margin-bottom:10px;line-height:1.5;}
.answer-opts{display:flex;gap:8px;flex-wrap:wrap;margin-bottom:8px;}
.answer-opt{padding:8px 14px;border:1.5px solid #e0d8cc;border-radius:8px;font-size:13px;cursor:pointer;background:#fff;font-family:'Nanum Gothic',sans-serif;transition:all .15s;}
.answer-opt:hover{border-color:#f0c040;background:#fff8e8;}
.answer-opt.correct{border-color:#3d5a4a;background:#e8f0ec;color:#3d5a4a;font-weight:700;}
.answer-opt.wrong{border-color:#e24b4a;background:#ffebee;color:#e24b4a;}
.explain-box{background:#e8f0ec;border-radius:6px;padding:8px 12px;font-size:12px;color:#2d4a3e;line-height:1.6;display:none;margin-top:6px;}
.qmsg{font-size:12px;margin-top:6px;padding:5px 10px;border-radius:6px;display:none;}
.qmsg.ok{background:#e8f5e9;color:#2e7d32;}
.qmsg.no{background:#ffebee;color:#c62828;}
.hint-box{background:#e8f5e9;border:1px solid #81c784;border-radius:6px;padding:8px 12px;margin-top:6px;font-size:12px;color:#2e7d32;display:none;line-height:1.6;}
.size-hint{font-size:11px;padding:6px 10px;border-radius:6px;margin-top:4px;display:none;line-height:1.5;}
.size-hint.small{background:#fff3e0;color:#e65100;border:1px solid #ffb74d;}
.size-hint.big{background:#e3f2fd;color:#1565c0;border:1px solid #64b5f6;}
.btn{padding:10px 16px;border:none;border-radius:8px;font-size:13px;font-weight:700;cursor:pointer;font-family:'Nanum Gothic',sans-serif;transition:all .15s;}
.btn-green{background:#3d5a4a;color:#fff;}
.btn-green:hover{background:#4d7a5a;}
.btn-green:disabled{background:#ccc;cursor:not-allowed;}
.btn-gold{background:#c8a030;color:#fff;}
.btn-gold:hover{background:#b09020;}
.btn-hint{background:#fff;color:#c8a030;border:1.5px solid #c8a030;padding:6px 12px;font-size:11px;}
.btn-outline{background:#fff;color:#3d5a4a;border:1.5px solid #3d5a4a;}
.btn-full{width:100%;}
.btn-sm{padding:6px 12px;font-size:12px;}
.sec{font-size:10px;font-weight:800;color:#3d5a4a;letter-spacing:.06em;text-transform:uppercase;margin-bottom:6px;}
.form-row{display:grid;grid-template-columns:1fr 1fr;gap:8px;margin-bottom:8px;}
.form-row.three{grid-template-columns:1fr 1fr 1fr;}
.field label{font-size:11px;font-weight:700;color:#666;display:block;margin-bottom:3px;}
.field input,.field select,.field textarea{width:100%;padding:7px 9px;border:1.5px solid #e0d8cc;border-radius:7px;font-size:13px;font-family:'Nanum Gothic',sans-serif;color:#333;background:#fff;}
.field textarea{resize:vertical;min-height:60px;line-height:1.6;}
.field input:focus,.field select:focus,.field textarea:focus{outline:none;border-color:#3d5a4a;}
.total-bar{display:flex;align-items:center;justify-content:space-between;background:#e8f0ec;border-radius:8px;padding:10px 14px;margin-bottom:10px;}
.total-bar .lbl{font-size:11px;color:#555;}
.total-bar .val{font-size:16px;font-weight:800;color:#3d5a4a;}
.progress-bar{height:8px;background:#e0d8cc;border-radius:4px;margin-bottom:12px;overflow:hidden;}
.progress-fill{height:100%;background:#3d5a4a;border-radius:4px;transition:width .3s;}
.progress-fill.over{background:#e24b4a;}
.over-msg{background:#ffebee;border:1px solid #ef9a9a;border-radius:8px;padding:10px 14px;margin-bottom:10px;font-size:12px;color:#c62828;display:none;line-height:1.6;}
.room-list{display:flex;flex-direction:column;gap:6px;margin-bottom:12px;}
.room-tag{display:flex;align-items:center;justify-content:space-between;padding:8px 12px;border-radius:8px;color:#fff;font-size:12px;font-weight:700;}
.room-tag .info{display:flex;flex-direction:column;gap:2px;}
.room-tag .sub{font-size:10px;font-weight:400;opacity:.85;}
.room-tag button{background:rgba(255,255,255,0.25);border:none;color:#fff;cursor:pointer;border-radius:4px;padding:2px 7px;font-size:13px;}
.divider{height:1px;background:#e0d8cc;margin:12px 0;}
.empty-msg{text-align:center;color:#bbb;font-size:12px;padding:16px;}
.notice-box{background:#e8f0ec;border-left:4px solid #3d5a4a;border-radius:0 8px 8px 0;padding:12px 14px;margin-bottom:12px;font-size:13px;color:#2d4a3e;line-height:1.7;}
/* 루브릭 */
.rubric-table{width:100%;border-collapse:collapse;font-size:12px;margin-bottom:12px;}
.rubric-table th{background:#3d5a4a;color:#fff;padding:8px 6px;text-align:center;font-size:11px;}
.rubric-table th:first-child{text-align:left;padding-left:10px;}
.rubric-table td{padding:8px 6px;border-bottom:1px solid #e8e4dd;vertical-align:top;}
.rubric-table td:first-child{font-weight:700;color:#333;padding-left:10px;min-width:110px;}
.rubric-table tr:last-child td{border-bottom:none;}
.radio-group{display:flex;gap:4px;flex-wrap:wrap;}
.radio-btn{padding:5px 8px;border:1.5px solid #ddd;border-radius:6px;cursor:pointer;font-size:11px;font-weight:700;color:#888;background:#fff;white-space:nowrap;}
.radio-btn.sel-good{border-color:#3d5a4a;background:#e8f0ec;color:#3d5a4a;}
.radio-btn.sel-ok{border-color:#c8a030;background:#fff8e8;color:#c8a030;}
.radio-btn.sel-bad{border-color:#e24b4a;background:#ffebee;color:#e24b4a;}
.rubric-desc{font-size:10px;color:#888;margin-top:2px;font-weight:400;line-height:1.3;}
.check-item{display:flex;align-items:flex-start;gap:8px;padding:8px 10px;background:#f5f0e8;border-radius:8px;margin-bottom:6px;cursor:pointer;}
.check-item input[type=checkbox]{width:16px;height:16px;margin-top:1px;accent-color:#3d5a4a;flex-shrink:0;}
.check-item label{font-size:12px;color:#444;cursor:pointer;line-height:1.5;}
.eum-box{background:#f0f5f2;border-radius:8px;padding:12px;}
.eum-box .eum-q{font-size:12px;font-weight:700;color:#3d5a4a;margin-bottom:4px;}
.eum-box textarea{width:100%;padding:6px 8px;border:1.5px solid #c8d8cc;border-radius:6px;font-size:12px;resize:none;height:50px;font-family:'Nanum Gothic',sans-serif;margin-bottom:8px;background:#fff;}
.eum-box textarea:last-child{margin-bottom:0;}
canvas#resultCv{display:block;border-radius:10px;border:1px solid #e0d8cc;width:100%;}
</style>
</head>
<body>
<div class="header">
  <h1>🏠 나만의 원룸 아지트 설계하기</h1>
  <p>공간 디자이너가 되어 나만의 아지트를 설계해봐요!</p>
</div>
<div class="step-bar">
  <div class="step-tab active" id="tab1"><span class="num">①</span>목적</div>
  <div class="step-tab" id="tab2"><span class="num">②</span>양감확인</div>
  <div class="step-tab" id="tab3"><span class="num">③</span>구역설계</div>
  <div class="step-tab" id="tab4"><span class="num">④</span>루브릭</div>
  <div class="step-tab" id="tab5"><span class="num">⑤</span>저장</div>
</div>

<!-- STEP 1: 공간의 목적 -->
<div class="page show" id="page1">
  <div class="card" style="margin-top:16px;">
    <h2>💭 어떤 공간을 만들고 싶나요?</h2>
    <p>설계를 시작하기 전에 내가 만들 아지트에 대해 생각해봐요!</p>
    <div class="field" style="margin-bottom:10px;">
      <label>이 아지트에서 무엇을 하고 싶나요?</label>
      <textarea id="purpose1" placeholder="예: 친구들과 게임도 하고, 혼자 음악도 듣고 싶어요."></textarea>
    </div>
    <div class="field" style="margin-bottom:10px;">
      <label>어떤 구역이 꼭 필요할 것 같나요?</label>
      <textarea id="purpose2" placeholder="예: 침실, 취미방, 화장실이 필요해요."></textarea>
    </div>
    <div class="field" style="margin-bottom:12px;">
      <label>이 아지트를 완성하면 어떤 점이 좋을까요?</label>
      <textarea id="purpose3" placeholder="예: 내가 원하는 공간에서 마음껏 쉴 수 있을 것 같아요."></textarea>
    </div>
    <button class="btn btn-green btn-full" onclick="goStep(2)">양감 확인하러 가기 →</button>
  </div>
</div>

<!-- STEP 2: 양감 확인 -->
<div class="page" id="page2">
  <div class="card" style="margin-top:16px;">
    <h2>📐 양감 확인 퀴즈</h2>
    <p>설계 전에 가구의 실제 크기를 알아봐요! 모눈 <b>1칸(가로) × 1줄(세로) = 1m²</b>이에요.</p>
    <div class="quiz-box" id="furnitureQuiz">
      <div class="qlabel" id="furnitureQ"></div>
      <div class="answer-opts" id="furnitureOpts"></div>
      <div class="explain-box" id="furnitureExplain"></div>
    </div>
    <div class="quiz-box" id="totalQuiz">
      <div class="qlabel">내 아지트는 모눈 77칸이에요. 전체 넓이는 몇 m²인가요?</div>
      <div class="answer-opts">
        <div class="answer-opt" onclick="checkTotal(this,7)">① 7m²</div>
        <div class="answer-opt" onclick="checkTotal(this,17)">② 17m²</div>
        <div class="answer-opt" onclick="checkTotal(this,77)">③ 77m²</div>
        <div class="answer-opt" onclick="checkTotal(this,177)">④ 177m²</div>
      </div>
      <div class="explain-box" id="totalExplain">모눈 1칸 = 1m²이니까 77칸 = 77m²예요! 꽤 넓죠? 약 23평 크기예요.</div>
    </div>
    <button class="btn btn-green btn-full" id="btn2" disabled onclick="goStep(3)">구역 설계 시작하기 →</button>
  </div>
</div>

<!-- STEP 3: 구역 설계 -->
<div class="page" id="page3">
  <div class="card" style="margin-top:16px;">
    <h2>🗂 구역 추가하기</h2>
    <p>아지트에 넣고 싶은 구역을 설계해봐요. 구역마다 넓이를 직접 계산해야 추가할 수 있어요!</p>
    <div class="total-bar">
      <div><div class="lbl">현재 사용 넓이</div><div class="val"><span id="usedArea">0</span> m²</div></div>
      <div><div class="lbl">남은 넓이</div><div class="val"><span id="leftArea">77</span> m²</div></div>
      <div><div class="lbl">최대</div><div class="val" style="font-size:13px;">77 m²</div></div>
    </div>
    <div class="progress-bar"><div class="progress-fill" id="progressFill" style="width:0%"></div></div>
    <div class="over-msg" id="overMsg">
      ⚠️ 전체 넓이가 77m²를 넘었어요! 구역 크기를 줄이거나 삭제해봐요.<br>
      💡 침실 8~10m², 화장실 4~5m², 거실 15~20m² 정도면 충분해요!
    </div>
    <div class="room-list" id="roomList"><p class="empty-msg">아직 구역이 없어요. 아래에서 추가해봐요!</p></div>
    <div class="divider"></div>
    <div class="sec">새 구역 추가</div>
    <div class="form-row">
      <div class="field"><label>구역 이름</label><input type="text" id="rname" placeholder="예: 침실, 취미방, 화장실..."></div>
      <div class="field"><label>모양 선택</label>
        <select id="rshape" onchange="onShapeChange()">
          <option value="">선택하세요</option>
          <option value="rect">직사각형</option>
          <option value="para">평행사변형</option>
          <option value="tri">삼각형</option>
          <option value="trap">사다리꼴</option>
          <option value="diamond">마름모</option>
        </select>
      </div>
    </div>
    <div id="dimArea"></div>
    <div id="quizArea" style="display:none;">
      <canvas id="prevCv" width="200" height="90" style="display:block;margin:0 auto 10px;border-radius:8px;border:1px solid #e0d8cc;background:#f5f0e8;"></canvas>
      <div class="quiz-box">
        <div class="qlabel" id="quizLabel"></div>
        <div style="display:flex;align-items:center;gap:8px;flex-wrap:wrap;">
          <input type="number" id="quizInput" placeholder="?" style="width:80px;padding:7px 10px;border:1.5px solid #f0c040;border-radius:6px;font-size:16px;text-align:center;font-family:'Nanum Gothic',sans-serif;">
          <span style="font-size:13px;color:#888;">m²</span>
          <button class="btn btn-gold btn-sm" onclick="checkRoomQuiz()">확인</button>
          <button class="btn btn-hint" id="roomHintBtn" onclick="showHint('roomHint')" style="display:none;">💡 힌트</button>
        </div>
        <div class="hint-box" id="roomHint"></div>
        <div class="size-hint" id="sizeHint"></div>
        <div class="qmsg" id="quizMsg"></div>
      </div>
      <button class="btn btn-green btn-full" id="addRoomBtn" disabled onclick="addRoom()">+ 이 구역 추가하기</button>
    </div>
  </div>
  <div class="notice-box">
    <b>✏️ 이제 모눈종이에 설계도를 그려봐요!</b><br>
    각 구역을 어디에 배치할지, 문과 창문은 어느 방향에 놓을지 생각하면서 그려봐요.<br>
    나머지 공간은 자유롭게 꾸며봐요 😊
  </div>
  <div style="display:flex;gap:8px;">
    <button class="btn btn-outline" onclick="goStep(2)">← 이전</button>
    <button class="btn btn-green" style="flex:1;" id="btn3" disabled onclick="goStep(4)">루브릭 확인하기 →</button>
  </div>
</div>

<!-- STEP 4: 루브릭 -->
<div class="page" id="page4">
  <div class="card" style="margin-top:16px;">
    <h2>✅ 루브릭 자기평가</h2>
    <p>내 설계를 스스로 평가해봐요!</p>
    <table class="rubric-table">
      <thead>
        <tr><th>평가 항목</th><th colspan="3">자기평가</th></tr>
      </thead>
      <tbody>
        <tr>
          <td>공간의 목적<div class="rubric-desc">목적을 잘 썼나요?</div></td>
          <td colspan="3">
            <div class="radio-group">
              <div class="radio-btn" id="r1a" onclick="setRubric(1,'good')">잘함<div class="rubric-desc">목적이 구체적이에요</div></div>
              <div class="radio-btn" id="r1b" onclick="setRubric(1,'ok')">도달<div class="rubric-desc">목적을 썼어요</div></div>
              <div class="radio-btn" id="r1c" onclick="setRubric(1,'bad')">미도달<div class="rubric-desc">목적이 없어요</div></div>
            </div>
          </td>
        </tr>
        <tr>
          <td>구역 설계<div class="rubric-desc">현재 <span id="rc1">0</span>개</div></td>
          <td colspan="3">
            <div class="radio-group">
              <div class="radio-btn" id="r2a" onclick="setRubric(2,'good')">잘함<div class="rubric-desc">3개 이상, 크기 적절</div></div>
              <div class="radio-btn" id="r2b" onclick="setRubric(2,'ok')">도달<div class="rubric-desc">3개 이상 설계했어요</div></div>
              <div class="radio-btn" id="r2c" onclick="setRubric(2,'bad')">미도달<div class="rubric-desc">3개보다 적어요</div></div>
            </div>
          </td>
        </tr>
        <tr>
          <td>넓이 계산<div class="rubric-desc">공식 활용</div></td>
          <td colspan="3">
            <div class="radio-group">
              <div class="radio-btn" id="r3a" onclick="setRubric(3,'good')">잘함<div class="rubric-desc">모든 구역 공식으로 정확하게</div></div>
              <div class="radio-btn" id="r3b" onclick="setRubric(3,'ok')">도달<div class="rubric-desc">계산은 했어요</div></div>
              <div class="radio-btn" id="r3c" onclick="setRubric(3,'bad')">미도달<div class="rubric-desc">계산이 틀리거나 못했어요</div></div>
            </div>
          </td>
        </tr>
      </tbody>
    </table>

    <div class="sec" style="margin-top:4px;">체크리스트</div>
    <div class="check-item">
      <input type="checkbox" id="chk1">
      <label for="chk1">평면도에 각 구역의 배치, 문, 창문을 모두 표현했나요?</label>
    </div>
    <div class="check-item" style="background:#fff8e8;">
      <input type="checkbox" id="chk2">
      <label for="chk2">⭐ 가산점: 직사각형 외 다각형(삼각형, 사다리꼴 등)을 1개 이상 사용했나요?</label>
    </div>
  </div>

  <div class="card">
    <h2>🔗 이음 루틴</h2>
    <div class="eum-box">
      <div class="eum-q">💡 새롭게 알게 된 점은?</div>
      <textarea id="eum1" placeholder="이번 활동에서 새롭게 알게 된 것을 써봐요."></textarea>
      <div class="eum-q">🌍 생활 속에서 어떻게 활용할 수 있을까?</div>
      <textarea id="eum2" placeholder="넓이와 둘레가 실생활에서 어떻게 쓰이는지 써봐요."></textarea>
      <div class="eum-q">📚 앞으로 무엇을 배우면 좋을까?</div>
      <textarea id="eum3" placeholder="더 배우고 싶은 것이 있나요?"></textarea>
    </div>
  </div>

  <div style="display:flex;gap:8px;">
    <button class="btn btn-outline" onclick="goStep(3)">← 수정하기</button>
    <button class="btn btn-green" style="flex:1;" onclick="goStep(5)">저장하러 가기 →</button>
  </div>
</div>

<!-- STEP 5: 저장 -->
<div class="page" id="page5">
  <div class="card" style="margin-top:16px;">
    <h2>💾 학습지 저장하기</h2>
    <p>저장 버튼을 누르면 클래스보드에 올릴 수 있는 이미지가 저장돼요!</p>
    <button class="btn btn-gold btn-full" onclick="generateResult()">학습지 미리보기 생성</button>
  </div>
  <div id="resultWrap" style="display:none;">
    <div class="card">
      <canvas id="resultCv" width="560" height="1000"></canvas>
      <button class="btn btn-green btn-full" style="margin-top:12px;" onclick="saveResult()">📥 이미지로 저장하기</button>
    </div>
  </div>
  <div style="margin-top:8px;">
    <button class="btn btn-outline btn-full" onclick="goStep(4)">← 다시 확인하기</button>
  </div>
</div>

<script>
var COLORS=['#e8906a','#6aae90','#9080c8','#d4a030','#5a90d0','#c07080','#70b070','#c07090'];
var SHAPE_NAMES={rect:'직사각형',para:'평행사변형',tri:'삼각형',trap:'사다리꼴',diamond:'마름모'};
var SHAPE_HINTS={
  rect:'넓이 = 가로(칸) × 세로(줄)',
  para:'넓이 = 밑변(칸) × 높이(줄)',
  tri:'넓이 = 밑변(칸) × 높이(줄) ÷ 2',
  trap:'넓이 = (윗변 + 아랫변)(칸) × 높이(줄) ÷ 2',
  diamond:'넓이 = 대각선1(칸) × 대각선2(줄) ÷ 2'
};

var FURNITURE_QUIZ=[
  {q:'싱글 침대의 넓이는 몇 m²일까요?',opts:['① 1m²','② 2m²','③ 4m²','④ 6m²'],ans:1,explain:'싱글 침대는 가로 약 1m × 세로 약 2m = 2m²예요! (1칸 × 2줄)'},
  {q:'책상 의자 한 개의 넓이는 몇 m²일까요?',opts:['① 0.25m²','② 1m²','③ 2m²','④ 4m²'],ans:0,explain:'의자는 약 0.5m × 0.5m = 0.25m²예요! 생각보다 작죠?'},
  {q:'화장실의 최소 넓이는 몇 m²일까요?',opts:['① 1m²','② 2m²','③ 4m²','④ 8m²'],ans:2,explain:'화장실은 최소 가로 2m × 세로 2m = 4m² 정도 필요해요! (2칸 × 2줄)'},
  {q:'2인용 소파의 넓이는 몇 m²일까요?',opts:['① 1m²','② 2m²','③ 5m²','④ 10m²'],ans:1,explain:'2인용 소파는 약 1.5m × 0.9m ≈ 2m²예요! (가로 2칸 × 세로 1줄 정도)'},
  {q:'책상(학생용)의 넓이는 몇 m²일까요?',opts:['① 0.5m²','② 1m²','③ 3m²','④ 5m²'],ans:1,explain:'학생용 책상은 약 1.2m × 0.6m ≈ 1m²예요! (1칸 × 1줄 정도)'},
];

var rooms=[], roomQuizPassed=false, pendingArea=0;
var rubric={1:null,2:null,3:null};
var furnitureDone=false, totalDone=false;
var currentFurniture=null;

function initFurnitureQuiz(){
  var idx=Math.floor(Math.random()*FURNITURE_QUIZ.length);
  currentFurniture=FURNITURE_QUIZ[idx];
  document.getElementById('furnitureQ').textContent=currentFurniture.q;
  var opts=document.getElementById('furnitureOpts');
  opts.innerHTML='';
  currentFurniture.opts.forEach(function(o,i){
    var d=document.createElement('div');
    d.className='answer-opt';
    d.textContent=o;
    d.onclick=function(){checkFurniture(d,i);};
    opts.appendChild(d);
  });
}

function checkFurniture(el,idx){
  if(furnitureDone) return;
  var opts=document.getElementById('furnitureOpts').children;
  Array.from(opts).forEach(function(o){o.className='answer-opt';});
  if(idx===currentFurniture.ans){
    el.classList.add('correct');
    var exp=document.getElementById('furnitureExplain');
    exp.textContent=currentFurniture.explain;
    exp.style.display='block';
    furnitureDone=true;
    checkStep2Done();
  } else {
    el.classList.add('wrong');
  }
}

function checkTotal(el,val){
  if(totalDone) return;
  var opts=el.parentElement.children;
  Array.from(opts).forEach(function(o){o.className='answer-opt';});
  if(val===77){
    el.classList.add('correct');
    document.getElementById('totalExplain').style.display='block';
    totalDone=true;
    checkStep2Done();
  } else {
    el.classList.add('wrong');
  }
}

function checkStep2Done(){
  if(furnitureDone&&totalDone){
    document.getElementById('btn2').disabled=false;
  }
}

function goStep(n){
  for(var i=1;i<=5;i++){
    document.getElementById('page'+i).classList.remove('show');
    var t=document.getElementById('tab'+i);
    t.classList.remove('active');
    if(i<n) t.classList.add('done'); else t.classList.remove('done');
  }
  document.getElementById('page'+n).classList.add('show');
  document.getElementById('tab'+n).classList.add('active');
  if(n===4) updateRubricCount();
}

function showHint(id){
  var el=document.getElementById(id);
  el.style.display=el.style.display==='block'?'none':'block';
}

function calcArea(s,d1,d2,d3){
  if(s==='rect'||s==='para') return Math.round(d1*d2*10)/10;
  if(s==='tri') return Math.round(d1*d2/2*10)/10;
  if(s==='trap') return Math.round((d1+d2)*d3/2*10)/10;
  if(s==='diamond') return Math.round(d1*d2/2*10)/10;
  return 0;
}

function onShapeChange(){
  var s=document.getElementById('rshape').value;
  roomQuizPassed=false;
  document.getElementById('quizArea').style.display='none';
  document.getElementById('addRoomBtn').disabled=true;
  if(!s){document.getElementById('dimArea').innerHTML='';return;}
  var h='<div class="form-row'+(s==='trap'?' three':'')+'" style="margin-bottom:8px;">';
  if(s==='rect') h+='<div class="field"><label>가로 (칸)</label><input type="number" id="d1" min="1" max="20" oninput="onDimChange()"></div><div class="field"><label>세로 (줄)</label><input type="number" id="d2" min="1" max="20" oninput="onDimChange()"></div>';
  if(s==='para') h+='<div class="field"><label>밑변 (칸)</label><input type="number" id="d1" min="1" max="20" oninput="onDimChange()"></div><div class="field"><label>높이 (줄)</label><input type="number" id="d2" min="1" max="20" oninput="onDimChange()"></div>';
  if(s==='tri') h+='<div class="field"><label>밑변 (칸)</label><input type="number" id="d1" min="1" max="20" oninput="onDimChange()"></div><div class="field"><label>높이 (줄)</label><input type="number" id="d2" min="1" max="20" oninput="onDimChange()"></div>';
  if(s==='trap') h+='<div class="field"><label>윗변 (칸)</label><input type="number" id="d1" min="1" max="20" oninput="onDimChange()"></div><div class="field"><label>아랫변 (칸)</label><input type="number" id="d2" min="1" max="20" oninput="onDimChange()"></div><div class="field"><label>높이 (줄)</label><input type="number" id="d3" min="1" max="20" oninput="onDimChange()"></div>';
  if(s==='diamond') h+='<div class="field"><label>대각선1 (칸)</label><input type="number" id="d1" min="1" max="20" oninput="onDimChange()"></div><div class="field"><label>대각선2 (줄)</label><input type="number" id="d2" min="1" max="20" oninput="onDimChange()"></div>';
  h+='</div>';
  document.getElementById('dimArea').innerHTML=h;
  drawPreview(s,0,0,0);
}

function onDimChange(){
  var s=document.getElementById('rshape').value;
  var d1=+document.getElementById('d1').value||0;
  var d2=+(document.getElementById('d2')?document.getElementById('d2').value:0)||0;
  var d3=+(document.getElementById('d3')?document.getElementById('d3').value:0)||0;
  var ready=(s!=='trap')?(d1>0&&d2>0):(d1>0&&d2>0&&d3>0);
  roomQuizPassed=false;
  document.getElementById('addRoomBtn').disabled=true;
  document.getElementById('quizMsg').style.display='none';
  document.getElementById('roomHint').style.display='none';
  document.getElementById('roomHintBtn').style.display='none';
  if(ready){
    pendingArea=calcArea(s,d1,d2,d3);
    var lbl='';
    if(s==='rect') lbl='가로 '+d1+'칸, 세로 '+d2+'줄일 때 넓이는 몇 m²인가요?';
    if(s==='para') lbl='밑변 '+d1+'칸, 높이 '+d2+'줄일 때 넓이는 몇 m²인가요?';
    if(s==='tri') lbl='밑변 '+d1+'칸, 높이 '+d2+'줄일 때 넓이는 몇 m²인가요?';
    if(s==='trap') lbl='윗변 '+d1+'칸, 아랫변 '+d2+'칸, 높이 '+d3+'줄일 때 넓이는 몇 m²인가요?';
    if(s==='diamond') lbl='대각선1이 '+d1+'칸, 대각선2가 '+d2+'줄일 때 넓이는 몇 m²인가요?';
    document.getElementById('quizLabel').textContent=lbl;
    document.getElementById('roomHint').textContent=SHAPE_HINTS[s];
    document.getElementById('quizInput').value='';
    document.getElementById('quizArea').style.display='block';
    drawPreview(s,d1,d2,d3);
    showSizeHint(pendingArea);
  } else {
    document.getElementById('quizArea').style.display='none';
    document.getElementById('sizeHint').style.display='none';
  }
}

function showSizeHint(area){
  var h=document.getElementById('sizeHint');
  if(area>0&&area<=2){
    h.className='size-hint small'; h.style.display='block';
    h.textContent='이 공간이 너무 작지 않나요? 💡 싱글 침대 한 개가 약 2m²예요.';
  } else if(area>=20){
    h.className='size-hint big'; h.style.display='block';
    h.textContent='이 공간이 너무 크지 않나요? 💡 우리 교실이 약 60m²예요.';
  } else {
    h.style.display='none';
  }
}

function drawPreview(s,d1,d2,d3){
  var cv=document.getElementById('prevCv');
  if(!cv) return;
  var ctx=cv.getContext('2d');
  var W=cv.width,H=cv.height,p=10;
  ctx.clearRect(0,0,W,H);
  ctx.fillStyle='#f5f0e8'; ctx.fillRect(0,0,W,H);
  ctx.fillStyle='#e8906a'; ctx.strokeStyle='#c07040'; ctx.lineWidth=2;
  ctx.beginPath();
  if(s==='rect'){ctx.rect(p,p,W-p*2,H-p*2);}
  else if(s==='para'){var sk=16;ctx.moveTo(p+sk,p);ctx.lineTo(W-p,p);ctx.lineTo(W-p-sk,H-p);ctx.lineTo(p,H-p);ctx.closePath();}
  else if(s==='tri'){ctx.moveTo(W/2,p);ctx.lineTo(W-p,H-p);ctx.lineTo(p,H-p);ctx.closePath();}
  else if(s==='trap'){var tw=(W-p*2)*.55;ctx.moveTo((W-tw)/2,p);ctx.lineTo((W+tw)/2,p);ctx.lineTo(W-p,H-p);ctx.lineTo(p,H-p);ctx.closePath();}
  else if(s==='diamond'){ctx.moveTo(W/2,p);ctx.lineTo(W-p,H/2);ctx.lineTo(W/2,H-p);ctx.lineTo(p,H/2);ctx.closePath();}
  ctx.fill(); ctx.stroke();
}

function checkRoomQuiz(){
  var ans=+document.getElementById('quizInput').value;
  var msg=document.getElementById('quizMsg');
  msg.style.display='block';
  if(Math.abs(ans-pendingArea)<0.05){
    msg.className='qmsg ok'; msg.textContent='정확해요! 구역을 추가할 수 있어요.';
    roomQuizPassed=true;
    document.getElementById('addRoomBtn').disabled=false;
    document.getElementById('roomHintBtn').style.display='none';
  } else {
    msg.className='qmsg no'; msg.textContent='다시 계산해봐요!';
    roomQuizPassed=false;
    document.getElementById('addRoomBtn').disabled=true;
    document.getElementById('roomHintBtn').style.display='inline-block';
  }
}

function addRoom(){
  if(!roomQuizPassed) return;
  var name=document.getElementById('rname').value||'구역';
  var s=document.getElementById('rshape').value;
  var total=rooms.reduce(function(a,r){return a+r.area;},0);
  if(total+pendingArea>77){document.getElementById('overMsg').style.display='block';return;}
  rooms.push({name:name,shape:s,area:pendingArea,color:COLORS[rooms.length%COLORS.length]});
  updateRoomList(); updateProgress();
  document.getElementById('rname').value='';
  document.getElementById('rshape').value='';
  document.getElementById('dimArea').innerHTML='';
  document.getElementById('quizArea').style.display='none';
  document.getElementById('addRoomBtn').disabled=true;
  document.getElementById('overMsg').style.display='none';
  roomQuizPassed=false;
  if(rooms.length>=3) document.getElementById('btn3').disabled=false;
}

function removeRoom(i){
  rooms.splice(i,1); updateRoomList(); updateProgress();
  if(rooms.length<3) document.getElementById('btn3').disabled=true;
}

function updateRoomList(){
  var l=document.getElementById('roomList');
  if(!rooms.length){l.innerHTML='<p class="empty-msg">아직 구역이 없어요. 아래에서 추가해봐요!</p>';return;}
  l.innerHTML='';
  rooms.forEach(function(r,i){
    var d=document.createElement('div');
    d.className='room-tag'; d.style.background=r.color;
    d.innerHTML='<div class="info"><span>'+r.name+'</span><span class="sub">'+SHAPE_NAMES[r.shape]+' · '+r.area+'m²</span></div><button onclick="removeRoom('+i+')">×</button>';
    l.appendChild(d);
  });
}

function updateProgress(){
  var total=rooms.reduce(function(a,r){return a+r.area;},0);
  var pct=Math.min(100,Math.round(total/77*100));
  document.getElementById('usedArea').textContent=total;
  document.getElementById('leftArea').textContent=Math.max(0,77-total);
  var fill=document.getElementById('progressFill');
  fill.style.width=pct+'%';
  fill.className='progress-fill'+(total>77?' over':'');
}

function updateRubricCount(){
  document.getElementById('rc1').textContent=rooms.length;
}

function setRubric(num,val){
  rubric[num]=val;
  var prefix='r'+num;
  ['a','b','c'].forEach(function(b,i){
    var el=document.getElementById(prefix+b);
    if(el){
      el.className='radio-btn';
      var v=['good','ok','bad'][i];
      if(v===val) el.classList.add(['sel-good','sel-ok','sel-bad'][i]);
    }
  });
}

function getRubricLabel(val){
  if(val==='good') return '잘함';
  if(val==='ok') return '도달';
  if(val==='bad') return '미도달';
  return '미선택';
}
function getRubricColor(val){
  if(val==='good') return '#3d5a4a';
  if(val==='ok') return '#c8a030';
  if(val==='bad') return '#e24b4a';
  return '#aaa';
}

function wrapText(ctx,text,x,y,maxW,lh){
  if(!text) return y;
  var line='';
  for(var i=0;i<text.length;i++){
    var t=line+text[i];
    if(ctx.measureText(t).width>maxW&&line){ctx.fillText(line,x,y);y+=lh;line=text[i];}
    else line=t;
  }
  if(line){ctx.fillText(line,x,y);y+=lh;}
  return y;
}

function generateResult(){
  var p1=document.getElementById('purpose1').value||'';
  var p2=document.getElementById('purpose2').value||'';
  var p3=document.getElementById('purpose3').value||'';
  var eum1=document.getElementById('eum1').value||'';
  var eum2=document.getElementById('eum2').value||'';
  var eum3=document.getElementById('eum3').value||'';
  var chk1=document.getElementById('chk1').checked;
  var chk2=document.getElementById('chk2').checked;
  var total=rooms.reduce(function(a,r){return a+r.area;},0);
  var W=560;

  // 동적 높이
  var H=70+120+rooms.length*48+60+160+160+50;
  var cv=document.getElementById('resultCv');
  cv.width=W; cv.height=H;
  var ctx=cv.getContext('2d');
  ctx.fillStyle='#fff'; ctx.fillRect(0,0,W,H);

  // 헤더
  ctx.fillStyle='#3d5a4a'; ctx.fillRect(0,0,W,52);
  ctx.fillStyle='#fff'; ctx.font='bold 16px sans-serif'; ctx.textAlign='left';
  ctx.fillText('🏠 나만의 원룸 아지트 설계 학습지',18,32);
  var y=66;

  // 공간의 목적
  ctx.fillStyle='#3d5a4a'; ctx.font='bold 13px sans-serif';
  ctx.fillText('💭 공간의 목적',18,y); y+=18;
  ctx.fillStyle='#f5f0e8'; ctx.fillRect(14,y,W-28,100);
  ctx.fillStyle='#444'; ctx.font='11px sans-serif';
  var pad=24;
  y+=14;
  y=wrapText(ctx,'• '+p1,pad,y,W-48,16);
  y=wrapText(ctx,'• '+p2,pad,y,W-48,16);
  y=wrapText(ctx,'• '+p3,pad,y,W-48,16);
  y+=10;

  // 구역 설계
  ctx.fillStyle='#3d5a4a'; ctx.font='bold 13px sans-serif'; ctx.textAlign='left';
  ctx.fillText('📋 구역 설계 내용',18,y); y+=16;
  rooms.forEach(function(r,i){
    ctx.fillStyle=r.color+'22'; ctx.fillRect(14,y,W-28,40);
    ctx.strokeStyle=r.color; ctx.lineWidth=1.5; ctx.strokeRect(14,y,W-28,40);
    ctx.fillStyle=r.color; ctx.fillRect(14,y,5,40);
    ctx.fillStyle='#222'; ctx.font='bold 12px sans-serif';
    ctx.fillText((i+1)+'. '+r.name,26,y+14);
    ctx.fillStyle='#555'; ctx.font='11px sans-serif';
    ctx.fillText('모양: '+SHAPE_NAMES[r.shape]+'  |  넓이: '+r.area+'m²  ✓',26,y+30);
    y+=44;
  });
  ctx.fillStyle='#e8f0ec'; ctx.fillRect(14,y,W-28,32);
  ctx.fillStyle='#3d5a4a'; ctx.font='bold 12px sans-serif';
  ctx.fillText('총 사용 넓이: '+total+'m²  /  77m²',24,y+21); y+=44;

  // 루브릭
  ctx.fillStyle='#3d5a4a'; ctx.font='bold 13px sans-serif';
  ctx.fillText('✅ 루브릭 자기평가',18,y); y+=16;
  var rubrics=[
    {label:'공간의 목적',val:rubric[1]},
    {label:'구역 설계',val:rubric[2]},
    {label:'넓이 계산',val:rubric[3]},
  ];
  rubrics.forEach(function(r){
    ctx.fillStyle='#f5f0e8'; ctx.fillRect(14,y,W-28,34);
    ctx.strokeStyle='#e0d8cc'; ctx.lineWidth=0.5; ctx.strokeRect(14,y,W-28,34);
    ctx.fillStyle='#333'; ctx.font='bold 12px sans-serif'; ctx.textAlign='left';
    ctx.fillText(r.label,24,y+22);
    ctx.fillStyle=getRubricColor(r.val); ctx.font='bold 12px sans-serif'; ctx.textAlign='right';
    ctx.fillText('[ '+getRubricLabel(r.val)+' ]',W-20,y+22);
    y+=38;
  });
  ctx.fillStyle='#fff8e8'; ctx.fillRect(14,y,W-28,34);
  ctx.strokeStyle='#f0c040'; ctx.lineWidth=0.5; ctx.strokeRect(14,y,W-28,34);
  ctx.fillStyle='#333'; ctx.font='bold 12px sans-serif'; ctx.textAlign='left';
  ctx.fillText('배치·문·창문 표현',24,y+14);
  ctx.fillText('⭐ 직사각형 외 도형',24,y+28);
  ctx.fillStyle=chk1?'#3d5a4a':'#aaa'; ctx.textAlign='right';
  ctx.fillText(chk1?'✓ 완료':'미완료',W-20,y+14);
  ctx.fillStyle=chk2?'#c8a030':'#aaa';
  ctx.fillText(chk2?'✓ 완료':'미완료',W-20,y+28);
  y+=44;

  // 이음 루틴
  ctx.fillStyle='#3d5a4a'; ctx.font='bold 13px sans-serif'; ctx.textAlign='left';
  ctx.fillText('🔗 이음 루틴',18,y); y+=16;
  var eums=[
    {q:'💡 새롭게 알게 된 점',t:eum1},
    {q:'🌍 생활 속 활용',t:eum2},
    {q:'📚 앞으로 배우고 싶은 것',t:eum3},
  ];
  eums.forEach(function(e){
    ctx.fillStyle='#f0f5f2'; ctx.fillRect(14,y,W-28,50);
    ctx.strokeStyle='#c8d8cc'; ctx.lineWidth=0.5; ctx.strokeRect(14,y,W-28,50);
    ctx.fillStyle='#3d5a4a'; ctx.font='bold 11px sans-serif';
    ctx.fillText(e.q,24,y+14);
    ctx.fillStyle='#333'; ctx.font='12px sans-serif';
    wrapText(ctx,e.t||'',24,y+28,W-48,15);
    y+=54;
  });

  document.getElementById('resultWrap').style.display='block';
}

function saveResult(){
  var cv=document.getElementById('resultCv');
  var a=document.createElement('a');
  a.download='아지트설계_학습지.png';
  a.href=cv.toDataURL('image/png');
  a.click();
}

// 초기화
initFurnitureQuiz();
</script>
</body>
</html>
