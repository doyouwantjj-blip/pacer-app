<!DOCTYPE html>
<html lang="ko">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, viewport-fit=cover">
<title>페이서 · 러닝 페이스 코치</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=IBM+Plex+Sans+KR:wght@400;500;600;700&family=IBM+Plex+Mono:wght@500;600&display=swap" rel="stylesheet">
<style>
  :root{
    --bg: #0A0E16;
    --bg-elevated: #10151F;
    --contour: #1A2230;
    --ink: #F2F4F8;
    --ink-dim: #7C879B;
    --teal: #2DD4BF;
    --coral: #FF6B4A;
    --amber: #F2B84B;
    --line: #212B3B;
  }
  *{ box-sizing: border-box; margin:0; padding:0; -webkit-tap-highlight-color: transparent; }
  html,body{ height:100%; }
  body{
    background:
      radial-gradient(circle at 15% -10%, rgba(45,212,191,0.10), transparent 45%),
      radial-gradient(circle at 100% 10%, rgba(255,107,74,0.08), transparent 40%),
      repeating-radial-gradient(circle at 50% 120%, transparent 0, transparent 38px, var(--contour) 39px, transparent 40px),
      var(--bg);
    color: var(--ink);
    font-family: 'IBM Plex Sans KR', sans-serif;
    height: 100dvh;
    display:flex;
    flex-direction:column;
    overflow:hidden;
  }
  .eyebrow{
    font-family:'IBM Plex Mono', monospace;
    font-size:11px;
    letter-spacing:0.18em;
    color: var(--ink-dim);
    text-transform:uppercase;
  }
  header{
    padding: 18px 20px 10px;
    display:flex;
    justify-content:space-between;
    align-items:center;
    border-bottom:1px solid var(--line);
    flex-shrink:0;
  }
  header .brand{ display:flex; flex-direction:column; gap:2px; }
  header .brand b{
    font-family:'Bebas Neue', sans-serif;
    font-size:22px;
    letter-spacing:0.04em;
  }
  .status-pill{
    display:flex; align-items:center; gap:6px;
    font-family:'IBM Plex Mono', monospace;
    font-size:11px;
    color: var(--ink-dim);
    border:1px solid var(--line);
    padding:5px 10px;
    border-radius:99px;
  }
  .status-pill .dot{ width:6px; height:6px; border-radius:50%; background: var(--ink-dim); transition: background .3s; }
  .status-pill.live .dot{ background: var(--teal); box-shadow:0 0 8px var(--teal); }

  main{
    flex:1;
    min-height:0;
    overflow-y:auto;
    -webkit-overflow-scrolling:touch;
    display:flex; flex-direction:column; align-items:center;
    padding: 16px 20px 12px;
    gap:16px;
  }

  .ring-wrap{ position:relative; width:min(58vw, 220px); aspect-ratio:1; flex-shrink:0; }
  svg.ring{ width:100%; height:100%; transform:rotate(-90deg); }
  .ring-track{ fill:none; stroke: var(--line); stroke-width:10; }
  .ring-fill{ fill:none; stroke: var(--teal); stroke-width:10; stroke-linecap:round; transition: stroke-dashoffset .6s ease, stroke .4s; }
  .ring-center{
    position:absolute; inset:0; display:flex; flex-direction:column; align-items:center; justify-content:center; gap:2px;
  }
  .ring-center .label{ font-family:'IBM Plex Mono', monospace; font-size:11px; letter-spacing:.14em; color:var(--ink-dim); text-transform:uppercase; }
  .ring-center .pace{ font-family:'Bebas Neue', sans-serif; font-size:46px; line-height:1; letter-spacing:.02em; }
  .ring-center .pace small{ font-size:17px; color:var(--ink-dim); margin-left:4px; }
  .ring-center .delta{ font-family:'IBM Plex Mono', monospace; font-size:12px; margin-top:5px; padding:3px 10px; border-radius:99px; border:1px solid var(--line); }
  .delta.slow{ color: var(--coral); border-color: rgba(255,107,74,.35); }
  .delta.fast{ color: var(--teal); border-color: rgba(45,212,191,.35); }
  .delta.even{ color: var(--ink-dim); }

  .slope-badge{
    display:flex; align-items:center; gap:8px;
    font-family:'IBM Plex Mono', monospace; font-size:12px; color:var(--amber);
    border:1px solid rgba(242,184,75,.3); background: rgba(242,184,75,.06);
    padding:7px 14px; border-radius:99px;
    opacity:0; transform:translateY(-6px); transition: all .35s;
  }
  .slope-badge.show{ opacity:1; transform:translateY(0); }

  .stat-grid{ width:100%; max-width:420px; display:grid; grid-template-columns:1fr 1fr 1fr; gap:10px; }
  .stat{ background: var(--bg-elevated); border:1px solid var(--line); border-radius:14px; padding:12px 10px; text-align:center; }
  .stat .eyebrow{ margin-bottom:6px; }
  .stat .val{ font-family:'IBM Plex Mono', monospace; font-weight:600; font-size:18px; }

  .target-row{
    width:100%; max-width:420px;
    display:flex; align-items:center; justify-content:space-between;
    background: var(--bg-elevated); border:1px solid var(--line); border-radius:14px;
    padding:14px 16px;
  }
  .target-row .eyebrow{ margin-bottom:4px; }
  .target-row .pace-input{
    display:flex; align-items:center; gap:6px;
  }
  .target-row input{
    width:46px; background:transparent; border:none; color:var(--ink);
    font-family:'IBM Plex Mono', monospace; font-size:20px; font-weight:600; text-align:center;
    border-bottom:1px solid var(--line); padding-bottom:2px;
  }
  .target-row input:focus{ outline:none; border-color: var(--teal); }
  .target-row .sep{ color:var(--ink-dim); font-family:'IBM Plex Mono', monospace; }

  .mode-tabs{
    width:100%; max-width:420px;
    display:flex; gap:6px;
    background: var(--bg-elevated); border:1px solid var(--line); border-radius:12px;
    padding:4px;
  }
  .mode-tabs button{
    flex:1; padding:9px 8px; border-radius:9px; border:none; background:transparent;
    color: var(--ink-dim); font-family:'IBM Plex Sans KR', sans-serif; font-size:13px; font-weight:600;
  }
  .mode-tabs button.active{ background: var(--line); color: var(--ink); }

  .goal-panel{
    width:100%; max-width:420px;
    background: var(--bg-elevated); border:1px solid var(--line); border-radius:14px;
    padding:14px 16px;
    display:flex; flex-direction:column; gap:12px;
  }
  .goal-row{ display:flex; align-items:center; justify-content:space-between; gap:12px; }
  .goal-row .pace-input input{
    width:44px; background:transparent; border:none; color:var(--ink);
    font-family:'IBM Plex Mono', monospace; font-size:18px; font-weight:600; text-align:center;
    border-bottom:1px solid var(--line); padding-bottom:2px;
  }
  .goal-row .pace-input input:focus{ outline:none; border-color: var(--teal); }
  .goal-row .sep{ color:var(--ink-dim); font-family:'IBM Plex Mono', monospace; }
  .level-group{ display:flex; gap:6px; }
  .level-group button{
    flex:1; padding:9px 4px; border-radius:9px; border:1px solid var(--line); background:transparent;
    color: var(--ink-dim); font-family:'IBM Plex Sans KR', sans-serif; font-size:12px; font-weight:600;
  }
  .level-group button.active{ background: var(--teal); border-color: var(--teal); color:#04211D; }
  .goal-derived{
    font-family:'IBM Plex Mono', monospace; font-size:12px; color: var(--ink-dim);
    border-top:1px dashed var(--line); padding-top:10px;
  }
  .goal-derived b{ color: var(--ink); }
  .segment-badge{
    display:inline-flex; align-items:center; gap:6px;
    font-family:'IBM Plex Mono', monospace; font-size:11px; color: var(--teal);
    border:1px solid rgba(45,212,191,.3); background: rgba(45,212,191,.06);
    padding:4px 10px; border-radius:99px; margin-top:4px;
  }

  .log{
    width:100%; max-width:420px; flex:1;
    display:flex; flex-direction:column; gap:8px;
    overflow-y:auto; padding-bottom:8px;
    min-height:70px;
  }
  .log-item{
    display:flex; gap:10px; align-items:baseline;
    font-size:13px; color: var(--ink-dim);
    border-left:2px solid var(--line); padding-left:10px;
  }
  .log-item .t{ font-family:'IBM Plex Mono', monospace; font-size:11px; color:var(--ink-dim); white-space:nowrap; }
  .log-item.voice{ color: var(--ink); border-left-color: var(--teal); }
  .log-item.slope{ color: var(--amber); border-left-color: var(--amber); }

  footer{
    padding: 12px 20px calc(14px + env(safe-area-inset-bottom));
    display:flex; gap:10px;
    border-top:1px solid var(--line);
    background: var(--bg-elevated);
    flex-shrink:0;
  }
  button.primary{
    flex:1; padding:16px; border-radius:14px; border:none;
    font-family:'IBM Plex Sans KR', sans-serif; font-weight:700; font-size:16px;
    background: var(--teal); color:#04211D; letter-spacing:.01em;
  }
  button.primary.running{ background: var(--coral); color:#2A0D06; }
  button.ghost{
    padding:16px 18px; border-radius:14px; border:1px solid var(--line);
    background:transparent; color:var(--ink-dim); font-family:'IBM Plex Sans KR', sans-serif; font-size:14px;
  }
  .permission-note{
    max-width:420px; font-size:12px; color:var(--ink-dim); text-align:center; line-height:1.6;
    padding: 0 20px;
  }
  .permission-note b{ color: var(--ink); }
</style>
</head>
<body>

<header>
  <div class="brand">
    <span class="eyebrow">준썰 · 러닝 프로토타입</span>
    <b>PACER</b>
  </div>
  <div class="status-pill" id="gpsStatus"><span class="dot"></span><span id="gpsStatusText">GPS 대기</span></div>
</header>

<main>
  <div class="ring-wrap">
    <svg class="ring" viewBox="0 0 200 200">
      <circle class="ring-track" cx="100" cy="100" r="88"></circle>
      <circle class="ring-fill" id="ringFill" cx="100" cy="100" r="88" stroke-dasharray="553" stroke-dashoffset="553"></circle>
    </svg>
    <div class="ring-center">
      <span class="label">현재 페이스</span>
      <div class="pace"><span id="curPace">--:--</span><small>/km</small></div>
      <div class="delta even" id="deltaBadge">목표 대비 --</div>
    </div>
  </div>

  <div class="slope-badge" id="slopeBadge">▲ 오르막 구간 감지</div>

  <div class="mode-tabs">
    <button id="tabTraining" class="active">페이스 훈련 모드</button>
    <button id="tabGoal">목표 완주 모드</button>
  </div>

  <div class="target-row" id="trainingPanel">
    <div>
      <div class="eyebrow">목표 페이스</div>
      <div style="font-size:12px; color:var(--ink-dim)">km당 도달 시간</div>
    </div>
    <div class="pace-input">
      <input type="number" id="targetMin" value="6" min="2" max="15">
      <span class="sep">:</span>
      <input type="number" id="targetSec" value="0" min="0" max="59">
    </div>
  </div>

  <div class="goal-panel" id="goalPanel" style="display:none;">
    <div class="goal-row">
      <div>
        <div class="eyebrow">목표 거리</div>
      </div>
      <div class="pace-input">
        <input type="number" id="goalDist" value="5" min="1" max="42" step="0.5">
        <span class="sep">km</span>
      </div>
    </div>
    <div class="goal-row">
      <div>
        <div class="eyebrow">목표 시간</div>
      </div>
      <div class="pace-input">
        <input type="number" id="goalMin" value="40" min="1" max="300">
        <span class="sep">:</span>
        <input type="number" id="goalSec" value="0" min="0" max="59">
      </div>
    </div>
    <div>
      <div class="eyebrow" style="margin-bottom:8px;">러너 레벨 (평지 기준 페이스 곡선)</div>
      <div class="level-group" id="levelGroup">
        <button data-level="beginner">초급</button>
        <button data-level="intermediate" class="active">중급</button>
        <button data-level="advanced">고급</button>
      </div>
    </div>
    <div class="goal-derived" id="goalDerived">평균 페이스 <b>--:--</b>/km · 초반 <b>--:--</b> · 후반 <b>--:--</b></div>
  </div>

  <div class="slope-badge" id="segmentBadge" style="border-color:rgba(45,212,191,.3); background:rgba(45,212,191,.06); color:var(--teal);">초반 구간 · 여유 있게</div>

  <div class="stat-grid">
    <div class="stat"><div class="eyebrow">거리</div><div class="val" id="statDist">0.00 km</div></div>
    <div class="stat"><div class="eyebrow">시간</div><div class="val" id="statTime">00:00</div></div>
    <div class="stat"><div class="eyebrow">평균 페이스</div><div class="val" id="statAvg">--:--</div></div>
  </div>

  <div class="log" id="log"></div>

  <p class="permission-note" id="permNote">시작을 누르면 <b>위치 권한</b>을 요청합니다. 음성 코칭은 폰의 <b>블루투스 출력 기기</b>(글라스 스피커)로 자동 재생됩니다 — 폰 설정에서 미리 페어링해두세요.</p>
</main>

<footer>
  <button class="primary" id="toggleBtn">러닝 시작</button>
  <button class="ghost" id="testVoiceBtn">음성 테스트</button>
</footer>

<script>
(function(){
  const $ = (id) => document.getElementById(id);
  const els = {
    gpsStatus: $('gpsStatus'), gpsStatusText: $('gpsStatusText'),
    curPace: $('curPace'), deltaBadge: $('deltaBadge'), ringFill: $('ringFill'),
    slopeBadge: $('slopeBadge'), segmentBadge: $('segmentBadge'),
    tabTraining: $('tabTraining'), tabGoal: $('tabGoal'),
    trainingPanel: $('trainingPanel'), goalPanel: $('goalPanel'),
    targetMin: $('targetMin'), targetSec: $('targetSec'),
    goalDist: $('goalDist'), goalMin: $('goalMin'), goalSec: $('goalSec'),
    levelGroup: $('levelGroup'), goalDerived: $('goalDerived'),
    statDist: $('statDist'), statTime: $('statTime'), statAvg: $('statAvg'),
    log: $('log'), toggleBtn: $('toggleBtn'), testVoiceBtn: $('testVoiceBtn'),
    permNote: $('permNote')
  };

  const LEVEL_CURVES = {
    beginner: {
      start: 8, mid: 0, end: -8,
      labels: { start: '초반 구간 · 여유 있게 시작하세요', mid: '중반 구간 · 목표 페이스 유지', end: '후반 구간 · 컨디션 되면 살짝 당겨보세요' }
    },
    intermediate: {
      start: 0, mid: 0, end: 0,
      labels: { start: '균등 페이스 구간', mid: '균등 페이스 구간', end: '균등 페이스 구간 · 끝까지 유지' }
    },
    advanced: {
      start: 3, mid: 0, end: -3,
      labels: { start: '초반 구간 · 절제된 페이스', mid: '중반 구간 · 목표 페이스 유지', end: '후반 구간 · 네거티브 스플릿 스퍼트' }
    }
  };
  let currentMode = 'training';
  let currentLevel = 'intermediate';
  let lastSegment = null;

  const RING_CIRC = 2 * Math.PI * 88;

  let watchId = null;
  let running = false;
  let startTime = null;
  let timerInterval = null;

  let totalDistanceM = 0;
  let lastPos = null;
  let recentPoints = [];
  let lastVoiceAt = 0;
  let lastKmAnnounced = 0;
  let slopeState = 'flat';
  let slopeSince = 0;
  let altBuffer = [];

  const VOICE_MIN_GAP_MS = 20000;
  const PACE_SLOW_THRESHOLD_S = 12;
  const PACE_FAST_THRESHOLD_S = 12;
  const SLOPE_GRADE_THRESHOLD = 0.03;
  const SLOPE_WINDOW_M = 40;
  const ACCURACY_REJECT_M = 25;
  const ACCURACY_WARN_M = 15;
  let poorSignalStreak = 0;

  function fmtPace(secPerKm){
    if(!isFinite(secPerKm) || secPerKm <= 0) return '--:--';
    const m = Math.floor(secPerKm / 60);
    const s = Math.round(secPerKm % 60);
    return `${m}:${String(s).padStart(2,'0')}`;
  }

  function fmtTime(totalSec){
    const m = Math.floor(totalSec / 60);
    const s = Math.floor(totalSec % 60);
    return `${String(m).padStart(2,'0')}:${String(s).padStart(2,'0')}`;
  }

  function targetPaceSec(){
    const m = parseInt(els.targetMin.value || '6', 10);
    const s = parseInt(els.targetSec.value || '0', 10);
    return m * 60 + s;
  }

  function goalBasePaceSec(){
    const dist = parseFloat(els.goalDist.value || '5');
    const m = parseInt(els.goalMin.value || '40', 10);
    const s = parseInt(els.goalSec.value || '0', 10);
    if(!dist || dist <= 0) return NaN;
    return (m * 60 + s) / dist;
  }

  function segmentByProgress(progress){
    if(progress < 1/3) return 'start';
    if(progress < 2/3) return 'mid';
    return 'end';
  }

  function goalSegmentPaceSec(base, segment){
    const curve = LEVEL_CURVES[currentLevel];
    const pct = curve[segment] || 0;
    return base * (1 + pct / 100);
  }

  function currentTargetPaceSec(){
    if(currentMode === 'training'){
      return targetPaceSec();
    }
    const base = goalBasePaceSec();
    if(!isFinite(base)) return NaN;
    const dist = parseFloat(els.goalDist.value || '5');
    const progress = dist > 0 ? Math.min(1, (totalDistanceM/1000) / dist) : 0;
    const segment = segmentByProgress(progress);
    return goalSegmentPaceSec(base, segment);
  }

  function updateGoalDerived(){
    const base = goalBasePaceSec();
    if(!isFinite(base) || base <= 0){
      els.goalDerived.innerHTML = '평균 페이스 <b>--:--</b>/km';
      return;
    }
    const startP = goalSegmentPaceSec(base, 'start');
    const endP = goalSegmentPaceSec(base, 'end');
    els.goalDerived.innerHTML = `평균 페이스 <b>${fmtPace(base)}</b>/km · 초반 <b>${fmtPace(startP)}</b> · 후반 <b>${fmtPace(endP)}</b>`;
  }

  function setMode(mode){
    currentMode = mode;
    els.tabTraining.classList.toggle('active', mode === 'training');
    els.tabGoal.classList.toggle('active', mode === 'goal');
    els.trainingPanel.style.display = mode === 'training' ? 'flex' : 'none';
    els.goalPanel.style.display = mode === 'goal' ? 'flex' : 'none';
    lastSegment = null;
    if(mode === 'goal') updateGoalDerived();
  }

  function setLevel(level){
    currentLevel = level;
    [...els.levelGroup.children].forEach(btn => btn.classList.toggle('active', btn.dataset.level === level));
    updateGoalDerived();
  }

  function maybeAnnounceSegmentChange(){
    if(currentMode !== 'goal' || !running) return;
    const dist = parseFloat(els.goalDist.value || '5');
    if(!dist || dist <= 0) return;
    const progress = Math.min(1, (totalDistanceM/1000) / dist);
    const segment = segmentByProgress(progress);
    if(segment !== lastSegment){
      lastSegment = segment;
      const label = LEVEL_CURVES[currentLevel].labels[segment];
      els.segmentBadge.textContent = label;
      els.segmentBadge.classList.add('show');
      speak(label.replace(/·/g, ','));
      addLog(label, 'voice');
    }
  }

  function haversine(lat1, lon1, lat2, lon2){
    const R = 6371000;
    const toRad = (d) => d * Math.PI / 180;
    const dLat = toRad(lat2 - lat1);
    const dLon = toRad(lon2 - lon1);
    const a = Math.sin(dLat/2)**2 + Math.cos(toRad(lat1)) * Math.cos(toRad(lat2)) * Math.sin(dLon/2)**2;
    return R * 2 * Math.atan2(Math.sqrt(a), Math.sqrt(1-a));
  }

  function addLog(text, cls){
    const item = document.createElement('div');
    item.className = 'log-item' + (cls ? ' ' + cls : '');
    const now = new Date();
    const t = now.toTimeString().slice(0,8);
    item.innerHTML = `<span class="t">${t}</span><span>${text}</span>`;
    els.log.prepend(item);
    while(els.log.children.length > 30) els.log.removeChild(els.log.lastChild);
  }

  function speak(text){
    if(!('speechSynthesis' in window)) { addLog('(TTS 미지원 브라우저) ' + text, 'voice'); return; }
    window.speechSynthesis.cancel();
    const u = new SpeechSynthesisUtterance(text);
    u.lang = 'ko-KR';
    u.rate = 1.02;
    window.speechSynthesis.speak(u);
    addLog('🔊 ' + text, 'voice');
  }

  function updateRing(curSec, tgtSec){
    let ratio;
    if(!isFinite(curSec) || curSec <= 0){ ratio = 0; }
    else {
      const diff = Math.abs(curSec - tgtSec);
      ratio = Math.max(0, 1 - diff / 60);
    }
    const offset = RING_CIRC * (1 - ratio);
    els.ringFill.style.strokeDashoffset = offset;

    const diff = curSec - tgtSec;
    els.deltaBadge.classList.remove('slow','fast','even');
    if(!isFinite(curSec) || curSec <= 0){
      els.deltaBadge.textContent = '목표 대비 --';
      els.deltaBadge.classList.add('even');
      els.ringFill.style.stroke = 'var(--ink-dim)';
    } else if(diff > 3){
      els.deltaBadge.textContent = `목표보다 ${Math.round(diff)}초 느림`;
      els.deltaBadge.classList.add('slow');
      els.ringFill.style.stroke = 'var(--coral)';
    } else if(diff < -3){
      els.deltaBadge.textContent = `목표보다 ${Math.round(-diff)}초 빠름`;
      els.deltaBadge.classList.add('fast');
      els.ringFill.style.stroke = 'var(--teal)';
    } else {
      els.deltaBadge.textContent = '목표 페이스 유지 중';
      els.deltaBadge.classList.add('even');
      els.ringFill.style.stroke = 'var(--teal)';
    }
  }

  function evaluatePaceAndMaybeSpeak(curSec){
    const tgt = currentTargetPaceSec();
    updateRing(curSec, tgt);
    maybeAnnounceSegmentChange();
    if(!isFinite(curSec) || curSec <= 0 || !isFinite(tgt)) return;

    const now = Date.now();
    if(now - lastVoiceAt < VOICE_MIN_GAP_MS) return;

    const diff = curSec - tgt;
    if(diff >= PACE_SLOW_THRESHOLD_S){
      speak('페이스가 목표보다 느립니다. 조금 더 올려보세요.');
      lastVoiceAt = now;
    } else if(diff <= -PACE_FAST_THRESHOLD_S){
      speak('목표보다 빠릅니다. 페이스를 살짝 낮춰도 좋아요.');
      lastVoiceAt = now;
    }
  }

  function evaluateSlope(){
    if(altBuffer.length < 2) return;
    const last = altBuffer[altBuffer.length - 1];
    let ref = altBuffer[0];
    for(let i = altBuffer.length - 1; i >= 0; i--){
      if(last.distM - altBuffer[i].distM >= SLOPE_WINDOW_M){ ref = altBuffer[i]; break; }
      ref = altBuffer[i];
    }
    const distDelta = last.distM - ref.distM;
    if(distDelta < SLOPE_WINDOW_M * 0.5) return;

    const altDelta = last.alt - ref.alt;
    if(altDelta == null || isNaN(altDelta)) return;
    const grade = altDelta / distDelta;

    let newState = 'flat';
    if(grade >= SLOPE_GRADE_THRESHOLD) newState = 'up';
    else if(grade <= -SLOPE_GRADE_THRESHOLD) newState = 'down';

    if(newState !== slopeState){
      slopeState = newState;
      if(newState === 'up'){
        els.slopeBadge.textContent = '▲ 오르막 구간 감지';
        els.slopeBadge.classList.add('show');
        speak('오르막 구간입니다. 페이스보다 힘 조절에 집중하세요.');
        addLog('오르막 구간 진입 (경사 약 ' + (grade*100).toFixed(1) + '%)', 'slope');
      } else if(newState === 'down'){
        els.slopeBadge.textContent = '▼ 내리막 구간 감지';
        els.slopeBadge.classList.add('show');
        speak('내리막 구간입니다. 무릎에 무리가 가지 않게 보폭을 조절하세요.');
        addLog('내리막 구간 진입 (경사 약 ' + (grade*100).toFixed(1) + '%)', 'slope');
      } else {
        els.slopeBadge.classList.remove('show');
        addLog('평지 구간으로 복귀', 'slope');
      }
    }
  }

  function onPosition(pos){
    const { latitude, longitude, altitude, accuracy } = pos.coords;
    const t = pos.timestamp;

    els.gpsStatus.classList.add('live');

    if(accuracy != null && accuracy > ACCURACY_REJECT_M){
      poorSignalStreak++;
      els.gpsStatusText.textContent = `GPS 신호 약함 (±${Math.round(accuracy)}m)`;
      els.gpsStatus.classList.remove('live');
      if(poorSignalStreak === 1 || poorSignalStreak % 10 === 0){
        addLog(`GPS 신호가 약해 이번 측정값(±${Math.round(accuracy)}m)은 건너뜁니다.`, 'slope');
      }
      return;
    }
    poorSignalStreak = 0;
    els.gpsStatusText.textContent = accuracy > ACCURACY_WARN_M
      ? `GPS 정확도 ±${Math.round(accuracy)}m (약함)`
      : `GPS 정확도 ±${Math.round(accuracy || 0)}m`;

    if(lastPos){
      const d = haversine(lastPos.lat, lastPos.lon, latitude, longitude);
      const dt = (t - lastPos.t) / 1000;
      if(dt > 0 && d / dt < 8){
        totalDistanceM += d;
        recentPoints.push({ t, distM: totalDistanceM });
        const cutoff = t - 20000;
        recentPoints = recentPoints.filter(p => p.t >= cutoff);

        if(altitude != null){
          altBuffer.push({ distM: totalDistanceM, alt: altitude });
          if(altBuffer.length > 200) altBuffer.shift();
          evaluateSlope();
        }
      }
    }
    lastPos = { lat: latitude, lon: longitude, alt: altitude, t };

    let curPaceSec = NaN;
    if(recentPoints.length >= 2){
      const first = recentPoints[0];
      const last = recentPoints[recentPoints.length - 1];
      const dm = last.distM - first.distM;
      const dtSec = (last.t - first.t) / 1000;
      if(dm > 3 && dtSec > 0){
        curPaceSec = (dtSec / dm) * 1000;
      }
    }
    els.curPace.textContent = fmtPace(curPaceSec);
    evaluatePaceAndMaybeSpeak(curPaceSec);

    const km = totalDistanceM / 1000;
    if(Math.floor(km) > lastKmAnnounced){
      lastKmAnnounced = Math.floor(km);
      const elapsedSec = (Date.now() - startTime) / 1000;
      const avgPace = elapsedSec / km;
      speak(`${lastKmAnnounced}킬로미터 통과. 평균 페이스 ${fmtPace(avgPace)}.`);
    }

    els.statDist.textContent = (totalDistanceM/1000).toFixed(2) + ' km';
  }

  function onPositionError(err){
    els.gpsStatus.classList.remove('live');
    els.gpsStatusText.textContent = 'GPS 오류: ' + err.message;
    addLog('GPS 오류 — ' + err.message, 'slope');
  }

  function tick(){
    if(!running) return;
    const elapsedSec = (Date.now() - startTime) / 1000;
    els.statTime.textContent = fmtTime(elapsedSec);
    const km = totalDistanceM / 1000;
    if(km > 0.01){
      els.statAvg.textContent = fmtPace(elapsedSec / km);
    }
  }

  function start(){
    if(!('geolocation' in navigator)){
      addLog('이 브라우저는 위치 정보를 지원하지 않습니다.', 'slope');
      return;
    }
    running = true;
    startTime = Date.now();
    totalDistanceM = 0; lastPos = null; recentPoints = []; altBuffer = [];
    lastKmAnnounced = 0; slopeState = 'flat'; lastVoiceAt = 0; poorSignalStreak = 0; lastSegment = null;
    els.slopeBadge.classList.remove('show');
    els.segmentBadge.classList.remove('show');
    els.toggleBtn.textContent = '러닝 종료';
    els.toggleBtn.classList.add('running');
    els.permNote.style.display = 'none';
    const startTgt = currentTargetPaceSec();
    const modeLabel = currentMode === 'goal' ? `목표 완주 모드(${els.goalDist.value}km, ${{beginner:'초급',intermediate:'중급',advanced:'고급'}[currentLevel]})` : '페이스 훈련 모드';
    addLog(`러닝 시작 — ${modeLabel}, 목표 페이스 ${fmtPace(startTgt)}`);
    speak('러닝을 시작합니다. 목표 페이스는 ' + fmtPace(startTgt) + '입니다.');

    watchId = navigator.geolocation.watchPosition(onPosition, onPositionError, {
      enableHighAccuracy: true, maximumAge: 1000, timeout: 15000
    });
    timerInterval = setInterval(tick, 1000);
  }

  function stop(){
    running = false;
    if(watchId != null) navigator.geolocation.clearWatch(watchId);
    if(timerInterval) clearInterval(timerInterval);
    els.toggleBtn.textContent = '러닝 시작';
    els.toggleBtn.classList.remove('running');
    els.gpsStatus.classList.remove('live');
    els.gpsStatusText.textContent = 'GPS 대기';
    const elapsedSec = (Date.now() - startTime) / 1000;
    const km = totalDistanceM/1000;
    addLog(`러닝 종료 — 총 ${km.toFixed(2)}km, ${fmtTime(elapsedSec)}`);
    speak('러닝을 종료합니다. 수고하셨습니다.');
  }

  els.toggleBtn.addEventListener('click', () => running ? stop() : start());
  els.testVoiceBtn.addEventListener('click', () => speak('음성 코칭 테스트입니다. 블루투스 스피커로 잘 들리시나요?'));

  els.tabTraining.addEventListener('click', () => setMode('training'));
  els.tabGoal.addEventListener('click', () => setMode('goal'));
  [...els.levelGroup.children].forEach(btn => {
    btn.addEventListener('click', () => setLevel(btn.dataset.level));
  });
  [els.goalDist, els.goalMin, els.goalSec].forEach(input => {
    input.addEventListener('input', updateGoalDerived);
  });

  updateRing(NaN, currentTargetPaceSec());
})();
</script>
</body>
</html>
