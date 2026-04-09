<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Production Budget Tool</title>
<style>
*{box-sizing:border-box;margin:0;padding:0}
body{font-family:sans-serif;background:#0e0e14;color:#dde2f0;min-height:100vh}
.nav{background:#090910;padding:12px 24px;display:flex;align-items:center;justify-content:space-between;border-bottom:1px solid #1e2030;position:sticky;top:0;z-index:100}
.nav-left{display:flex;align-items:center;gap:10px}
.nav-icon{width:28px;height:28px;background:#2a3580;border-radius:6px;display:flex;align-items:center;justify-content:center}
.nav-icon svg{width:15px;height:15px}
.nav-title{font-size:14px;font-weight:500}
.nav-sub{font-size:11px;color:#555a7a;margin-top:1px}
.nav-right{display:flex;gap:8px;align-items:center}
.pill{font-size:11px;padding:4px 11px;border-radius:20px;cursor:default}
.pill-blue{background:#1a2260;color:#7090f0;border:0.5px solid #2a3580}
.pill-warn{background:#2a1e08;color:#d08820;border:0.5px solid #604010}
.pill-ok{background:#0d2218;color:#30b878;border:0.5px solid #1a5030}
.pill-red{background:#2a0e0e;color:#d04040;border:0.5px solid #601010}

.tabs{background:#0a0a12;padding:0 24px;display:flex;gap:0;border-bottom:1px solid #1e2030}
.tab{font-size:12px;padding:10px 16px;color:#555a7a;border-bottom:2px solid transparent;cursor:pointer;transition:all .15s}
.tab:hover{color:#aab0d0}
.tab.active{color:#7090f0;border-bottom-color:#7090f0}

.main{padding:20px 24px;max-width:1200px;margin:0 auto}

.kpis{display:grid;grid-template-columns:repeat(5,minmax(0,1fr));gap:12px;margin-bottom:20px}
.kpi{background:#12131e;border:0.5px solid #1e2030;border-radius:8px;padding:14px 16px}
.kpi-label{font-size:10px;text-transform:uppercase;letter-spacing:.07em;color:#555a7a;margin-bottom:6px}
.kpi-val{font-size:22px;font-weight:500}
.kpi-sub{font-size:11px;margin-top:4px;color:#555a7a}

.grid2{display:grid;grid-template-columns:minmax(0,1.5fr) minmax(0,1fr);gap:16px;margin-bottom:16px}
.card{background:#12131e;border:0.5px solid #1e2030;border-radius:8px;padding:16px 18px}
.card-title{font-size:11px;text-transform:uppercase;letter-spacing:.07em;color:#555a7a;margin-bottom:14px}

/* dept rows */
.dept-row{display:flex;align-items:center;gap:10px;margin-bottom:11px;cursor:pointer;padding:6px 8px;border-radius:6px;transition:background .12s}
.dept-row:hover{background:#1a1c2e}
.dept-name{font-size:12px;color:#c0c8e8;min-width:140px}
.dept-track{flex:1;height:20px;background:#1a1c2a;border-radius:3px;overflow:hidden;position:relative}
.dept-fill{height:100%;border-radius:3px;transition:width .6s ease}
.dept-budget-line{position:absolute;top:0;height:100%;width:2px;background:#3a3f5a;pointer-events:none}
.dept-vals{font-size:11px;min-width:110px;text-align:right;color:#8890b0}
.dept-pct{font-size:11px;min-width:38px;text-align:right;font-weight:500}

/* add expense modal */
.modal-bg{display:none;position:fixed;inset:0;background:rgba(0,0,0,.6);z-index:200;align-items:center;justify-content:center}
.modal-bg.open{display:flex}
.modal{background:#14151f;border:0.5px solid #2a2d48;border-radius:10px;padding:24px;width:420px;max-width:95vw}
.modal h3{font-size:15px;font-weight:500;margin-bottom:16px}
.form-row{margin-bottom:12px}
.form-row label{font-size:11px;text-transform:uppercase;letter-spacing:.06em;color:#555a7a;display:block;margin-bottom:5px}
.form-row input,.form-row select{width:100%;background:#0e0f1a;border:0.5px solid #2a2d48;border-radius:6px;padding:8px 10px;font-size:13px;color:#dde2f0;font-family:sans-serif}
.form-row input:focus,.form-row select:focus{outline:none;border-color:#4a5598}
.form-actions{display:flex;gap:8px;margin-top:16px}
.btn-primary{flex:1;padding:9px;background:#2a3580;border:none;border-radius:6px;color:#a0b0f8;font-size:13px;cursor:pointer;transition:background .15s}
.btn-primary:hover{background:#3a45a0}
.btn-cancel{padding:9px 16px;background:transparent;border:0.5px solid #2a2d48;border-radius:6px;color:#555a7a;font-size:13px;cursor:pointer}
.btn-cancel:hover{background:#1a1c2e;color:#aaa}

/* activity */
.activity-row{display:flex;align-items:flex-start;gap:10px;margin-bottom:10px;padding:8px;border-radius:6px;transition:background .12s}
.activity-row:hover{background:#1a1c2e}
.adot{width:7px;height:7px;border-radius:50%;margin-top:4px;flex-shrink:0}
.atext{font-size:12px;color:#8890b0;line-height:1.5;flex:1}
.atime{font-size:10px;color:#3a3f5a;margin-top:2px}
.adel{font-size:10px;color:#3a3f5a;cursor:pointer;padding:2px 6px;border-radius:4px;transition:all .12s;flex-shrink:0;margin-top:2px}
.adel:hover{background:#2a0e0e;color:#d04040}

/* approvals */
.appr-row{display:flex;align-items:center;justify-content:space-between;padding:8px 0;border-bottom:0.5px solid #1a1c2a}
.appr-row:last-child{border-bottom:none}
.appr-label{font-size:12px;color:#c0c8e8;flex:1}
.appr-amount{font-size:12px;font-weight:500;margin:0 12px}
.appr-actions{display:flex;gap:4px}
.appr-btn{font-size:10px;padding:3px 8px;border-radius:4px;cursor:pointer;border:none;font-family:sans-serif;transition:all .12s}
.appr-approve{background:#0d2218;color:#30b878;border:0.5px solid #1a5030}
.appr-approve:hover{background:#1a3a28}
.appr-reject{background:#1e0808;color:#d04040;border:0.5px solid #601010}
.appr-reject:hover{background:#2a1010}
.badge{font-size:10px;padding:3px 8px;border-radius:4px}
.badge-pend{background:#1e1408;color:#d08820}
.badge-appr{background:#0d2218;color:#30b878}
.badge-rej{background:#1e0808;color:#d04040}

/* add buttons */
.add-btn{font-size:11px;padding:5px 12px;background:transparent;border:0.5px solid #2a2d48;border-radius:6px;color:#555a7a;cursor:pointer;transition:all .15s;margin-top:10px}
.add-btn:hover{background:#1a1c2e;color:#aaa;border-color:#4a4d68}

.empty{font-size:12px;color:#3a3f5a;text-align:center;padding:20px 0;font-style:italic}

/* forecast bar */
.forecast-wrap{margin-top:14px}
.forecast-track{height:12px;background:#1a1c2a;border-radius:6px;overflow:hidden;position:relative;margin-bottom:6px}
.forecast-spent{height:100%;border-radius:6px 0 0 6px;background:#7090f0;display:inline-block}
.forecast-committed{height:100%;background:#d08820;display:inline-block}
.forecast-remaining{height:100%;background:#1e2030;flex:1;display:inline-block}
.forecast-overrun{height:100%;background:#d04040;display:inline-block}
.forecast-labels{display:flex;gap:14px;font-size:10px;color:#555a7a;flex-wrap:wrap}
.fl-dot{width:8px;height:8px;border-radius:2px;display:inline-block;margin-right:4px}

.footer{background:#090910;border-top:1px solid #1e2030;padding:10px 24px;display:flex;justify-content:space-between;align-items:center;font-size:11px;color:#3a3f5a;margin-top:24px}
.avatar{width:24px;height:24px;border-radius:50%;border:1.5px solid #0e0e14;display:flex;align-items:center;justify-content:center;font-size:9px;font-weight:500;margin-left:-5px}

.blue{color:#7090f0}.green{color:#30b878}.amber{color:#d08820}.red{color:#d04040}.muted{color:#555a7a}
</style>
</head>
<body>

<div class="nav">
  <div class="nav-left">
    <div class="nav-icon">
      <svg viewBox="0 0 15 15" fill="none">
        <rect x="1" y="8" width="3" height="6" fill="#7090f0" rx="1"/>
        <rect x="6" y="5" width="3" height="9" fill="#7090f0" rx="1"/>
        <rect x="11" y="1" width="3" height="13" fill="#d08820" rx="1"/>
      </svg>
    </div>
    <div>
      <div class="nav-title" id="proj-title">Feature Film A — Production Budget</div>
      <div class="nav-sub" id="last-updated">Live tracking · Updated just now</div>
    </div>
  </div>
  <div class="nav-right">
    <span class="pill pill-blue" id="week-pill">Week 14 of 22</span>
    <span class="pill" id="status-pill">—</span>
    <span class="pill pill-warn" id="overrun-pill" style="display:none">Overrun risk</span>
  </div>
</div>

<div class="tabs">
  <div class="tab active" onclick="switchTab('overview',this)">Overview</div>
  <div class="tab" onclick="switchTab('approvals',this)">Approvals <span id="appr-count" style="font-size:10px;background:#2a1e08;color:#d08820;padding:1px 5px;border-radius:10px;margin-left:4px;"></span></div>
  <div class="tab" onclick="switchTab('settings',this)">Settings</div>
</div>

<!-- OVERVIEW TAB -->
<div id="tab-overview" class="main">
  <div class="kpis">
    <div class="kpi"><div class="kpi-label">Total budget</div><div class="kpi-val blue" id="k-budget">$0</div><div class="kpi-sub">Approved · locked</div></div>
    <div class="kpi"><div class="kpi-label">Spent to date</div><div class="kpi-val" id="k-spent">$0</div><div class="kpi-sub" id="k-spent-pct">0% of budget</div></div>
    <div class="kpi"><div class="kpi-label">Committed</div><div class="kpi-val amber" id="k-committed">$0</div><div class="kpi-sub">POs &amp; contracts</div></div>
    <div class="kpi"><div class="kpi-label">Remaining</div><div class="kpi-val" id="k-remaining">$0</div><div class="kpi-sub" id="k-remaining-pct">—</div></div>
    <div class="kpi"><div class="kpi-label">Forecast final</div><div class="kpi-val" id="k-forecast">$0</div><div class="kpi-sub" id="k-forecast-sub">—</div></div>
  </div>

  <div class="card" style="margin-bottom:16px;">
    <div class="card-title">Budget utilisation</div>
    <div class="forecast-wrap">
      <div class="forecast-track">
        <span class="forecast-spent" id="fbar-spent" style="width:0%"></span><span class="forecast-committed" id="fbar-committed" style="width:0%"></span><span class="forecast-overrun" id="fbar-overrun" style="width:0%"></span>
      </div>
      <div class="forecast-labels">
        <span><span class="fl-dot" style="background:#7090f0"></span>Spent</span>
        <span><span class="fl-dot" style="background:#d08820"></span>Committed</span>
        <span><span class="fl-dot" style="background:#d04040"></span>Overrun</span>
        <span><span class="fl-dot" style="background:#1e2030"></span>Remaining</span>
      </div>
    </div>
  </div>

  <div class="grid2">
    <div class="card">
      <div style="display:flex;align-items:center;justify-content:space-between;margin-bottom:14px;">
        <div class="card-title" style="margin-bottom:0">Spend by department</div>
        <button class="add-btn" onclick="openModal('expense')">+ Log expense</button>
      </div>
      <div id="dept-list"></div>
      <div style="display:flex;gap:16px;margin-top:10px;font-size:10px;color:#3a3f5a;">
        <span style="display:flex;align-items:center;gap:4px;"><span style="width:10px;height:4px;background:#7090f0;border-radius:2px;display:inline-block;"></span>Actual</span>
        <span style="display:flex;align-items:center;gap:4px;"><span style="width:2px;height:12px;background:#3a3f5a;display:inline-block;"></span>Budget line</span>
      </div>
    </div>

    <div>
      <div class="card" style="margin-bottom:16px;">
        <div style="display:flex;align-items:center;justify-content:space-between;margin-bottom:14px;">
          <div class="card-title" style="margin-bottom:0">Recent activity</div>
          <button class="add-btn" onclick="openModal('activity')">+ Add note</button>
        </div>
        <div id="activity-list"><div class="empty">No activity yet.</div></div>
      </div>
    </div>
  </div>
</div>

<!-- APPROVALS TAB -->
<div id="tab-approvals" class="main" style="display:none">
  <div class="card">
    <div style="display:flex;align-items:center;justify-content:space-between;margin-bottom:16px;">
      <div class="card-title" style="margin-bottom:0">Approval requests</div>
      <button class="add-btn" onclick="openModal('approval')">+ Request approval</button>
    </div>
    <div id="approvals-list"><div class="empty">No pending approvals.</div></div>
  </div>
</div>

<!-- SETTINGS TAB -->
<div id="tab-settings" class="main" style="display:none">
  <div class="card" style="max-width:520px">
    <div class="card-title">Project settings</div>
    <div class="form-row"><label>Project name</label><input id="set-name" value="Feature Film A" oninput="updateSettings()"></div>
    <div class="form-row"><label>Total budget ($)</label><input id="set-budget" type="number" value="4200000" oninput="updateSettings()"></div>
    <div class="form-row"><label>Current week</label><input id="set-week" type="number" value="14" min="1" oninput="updateSettings()"></div>
    <div class="form-row"><label>Total weeks</label><input id="set-weeks" type="number" value="22" min="1" oninput="updateSettings()"></div>
    <div style="margin-top:16px;padding-top:16px;border-top:0.5px solid #1e2030;">
      <div class="card-title" style="margin-bottom:12px;">Department budgets ($)</div>
      <div id="dept-settings"></div>
    </div>
  </div>
</div>

<!-- MODAL -->
<div class="modal-bg" id="modal-bg" onclick="closeModalBg(event)">
  <div class="modal" id="modal-box">
    <h3 id="modal-title">Add</h3>
    <div id="modal-body"></div>
  </div>
</div>

<div class="footer">
  <span id="footer-note">Production Budget Tool · AI-powered forecasting · all figures in USD</span>
  <div style="display:flex;align-items:center;gap:8px;">
    <span style="font-size:10px;color:#3a3f5a;">Finance &amp; production aligned</span>
    <div style="display:flex;">
      <div class="avatar" style="background:#2a3580;color:#7090f0;">JH</div>
      <div class="avatar" style="background:#0d2218;color:#30b878;">MO</div>
      <div class="avatar" style="background:#2a1e08;color:#d08820;">SR</div>
    </div>
  </div>
</div>

<script>
const DEPTS = [
  { id:'camera',   name:'Camera & grip',          budget:400000,  spent:248000 },
  { id:'art',      name:'Art & production design', budget:360000,  spent:390000 },
  { id:'locations',name:'Locations',               budget:320000,  spent:176000 },
  { id:'cast',     name:'Cast & talent',           budget:1300000, spent:832000 },
  { id:'vfx',      name:'VFX',                     budget:800000,  spent:328000 },
  { id:'post',     name:'Post production',         budget:500000,  spent:110000 },
  { id:'crew',     name:'Crew & labour',           budget:520000,  spent:614000 },
];

let settings = { name:'Feature Film A', budget:4200000, week:14, weeks:22 };
let committed = 890200;

let activities = [
  { color:'#d04040', text:'Art dept PO #1142 flagged — $42,000 exceeds line budget by 18%', time:'Today · 08:42 AM · flagged by AI' },
  { color:'#30b878', text:'VFX milestone payment approved — $85,000 released to vendor', time:'Yesterday · 4:11 PM · J. Hartley' },
  { color:'#d08820', text:'Crew overtime logged — 3 shoot days, est. $28,400 additional cost', time:'Yesterday · 11:30 AM · auto-imported' },
  { color:'#7090f0', text:'Location hold released — $12,000 committed cost cleared', time:'Apr 5 · 2:00 PM · M. Osei' },
];

let approvals = [
  { id:1, label:'Set build extension — Stage 4', amount:42000, dept:'art', status:'pending' },
  { id:2, label:'Stunt coordinator day rate uplift', amount:8500, dept:'crew', status:'approved' },
  { id:3, label:'Additional camera package — Day 68', amount:19200, dept:'camera', status:'rejected' },
  { id:4, label:'Post sound — additional mix days', amount:14000, dept:'post', status:'pending' },
];
let nextApprId = 5;

function fmt(n){ return '$' + Math.round(n).toLocaleString(); }
function pct(a,b){ return b ? Math.round(a/b*100) : 0; }

function totalSpent(){ return DEPTS.reduce((s,d)=>s+d.spent,0); }

function render(){
  const budget = settings.budget;
  const spent = totalSpent();
  const remain = Math.max(0, budget - spent - committed);
  const forecast = spent + committed + remain * 0.9;
  const overrun = Math.max(0, forecast - budget);

  document.getElementById('proj-title').textContent = settings.name + ' — Production Budget';
  document.getElementById('week-pill').textContent = 'Week ' + settings.week + ' of ' + settings.weeks;

  document.getElementById('k-budget').textContent = fmt(budget);
  document.getElementById('k-spent').textContent = fmt(spent);
  document.getElementById('k-spent-pct').textContent = pct(spent,budget) + '% of budget';
  document.getElementById('k-committed').textContent = fmt(committed);

  const remEl = document.getElementById('k-remaining');
  remEl.textContent = fmt(remain);
  remEl.className = 'kpi-val ' + (remain < budget*0.1 ? 'red' : remain < budget*0.2 ? 'amber' : 'green');
  document.getElementById('k-remaining-pct').textContent = pct(remain,budget) + '% of budget';

  const fcEl = document.getElementById('k-forecast');
  fcEl.textContent = fmt(forecast);
  fcEl.className = 'kpi-val ' + (overrun > 0 ? 'red' : 'green');
  document.getElementById('k-forecast-sub').textContent = overrun > 0 ? '+' + fmt(overrun) + ' overrun risk' : 'Within budget';

  const spentPct = Math.min(pct(spent,budget),100);
  const commPct  = Math.min(pct(committed,budget), 100 - spentPct);
  const ovPct    = Math.min(pct(overrun,budget),10);
  document.getElementById('fbar-spent').style.width = spentPct + '%';
  document.getElementById('fbar-committed').style.width = commPct + '%';
  document.getElementById('fbar-overrun').style.width = ovPct + '%';

  const pill = document.getElementById('status-pill');
  const op = document.getElementById('overrun-pill');
  if(overrun > 0){
    pill.className='pill pill-warn'; pill.textContent='Over budget';
    op.style.display=''; op.textContent = fmt(overrun) + ' risk';
  } else if(pct(spent,budget) < 60){
    pill.className='pill pill-ok'; pill.textContent='On track'; op.style.display='none';
  } else {
    pill.className='pill pill-ok'; pill.textContent='On track'; op.style.display='none';
  }

  renderDepts();
  renderActivity();
  renderApprovals();
  renderDeptSettings();
  document.getElementById('last-updated').textContent = 'Live tracking · Updated just now';
}

function renderDepts(){
  const maxBudget = Math.max(...DEPTS.map(d=>d.budget));
  const html = DEPTS.map(d => {
    const pctSpent = pct(d.spent, d.budget);
    const budgetLinePos = pct(d.budget, maxBudget);
    const barWidth = Math.min(pct(d.spent, maxBudget), 100);
    let color = '#7090f0';
    let pctColor = 'muted';
    if(pctSpent > 100){ color='#d04040'; pctColor='red'; }
    else if(pctSpent > 80){ color='#d08820'; pctColor='amber'; }
    else if(pctSpent < 50){ color='#30b878'; pctColor='green'; }
    return `<div class="dept-row" onclick="openDeptEdit('${d.id}')">
      <div class="dept-name">${d.name}</div>
      <div class="dept-track">
        <div class="dept-fill" style="width:${barWidth}%;background:${color};"></div>
        <div class="dept-budget-line" style="left:${budgetLinePos}%;"></div>
      </div>
      <div class="dept-vals">${fmt(d.spent)} / ${fmt(d.budget)}</div>
      <div class="dept-pct ${pctColor}">${pctSpent}%</div>
    </div>`;
  }).join('');
  document.getElementById('dept-list').innerHTML = html;
}

function renderActivity(){
  const el = document.getElementById('activity-list');
  if(!activities.length){ el.innerHTML='<div class="empty">No activity yet.</div>'; return; }
  el.innerHTML = activities.slice(0,6).map((a,i) =>
    `<div class="activity-row">
      <div class="adot" style="background:${a.color};"></div>
      <div style="flex:1"><div class="atext">${a.text}</div><div class="atime">${a.time}</div></div>
      <div class="adel" onclick="removeActivity(${i})">✕</div>
    </div>`
  ).join('');
}

function removeActivity(i){ activities.splice(i,1); renderActivity(); }

function renderApprovals(){
  const pending = approvals.filter(a=>a.status==='pending').length;
  document.getElementById('appr-count').textContent = pending || '';
  const el = document.getElementById('approvals-list');
  if(!approvals.length){ el.innerHTML='<div class="empty">No approval requests.</div>'; return; }
  el.innerHTML = approvals.map(a => {
    const amtColor = a.status==='rejected'?'red': a.status==='approved'?'green':'amber';
    const actions = a.status==='pending'
      ? `<button class="appr-btn appr-approve" onclick="setApproval(${a.id},'approved')">Approve</button>
         <button class="appr-btn appr-reject" onclick="setApproval(${a.id},'rejected')">Reject</button>`
      : `<span class="badge badge-${a.status==='approved'?'appr':'rej'}">${a.status}</span>`;
    return `<div class="appr-row">
      <div class="appr-label">${a.label}</div>
      <div class="appr-amount ${amtColor}">${fmt(a.amount)}</div>
      <div class="appr-actions">${actions}</div>
    </div>`;
  }).join('');
}

function setApproval(id, status){
  const a = approvals.find(x=>x.id===id);
  if(!a) return;
  a.status = status;
  if(status==='approved'){
    const d = DEPTS.find(x=>x.id===a.dept);
    if(d) d.spent += a.amount;
    committed = Math.max(0, committed - a.amount);
    activities.unshift({color:'#30b878', text: a.label + ' approved — ' + fmt(a.amount) + ' added to spend', time:'Just now'});
  } else {
    activities.unshift({color:'#d04040', text: a.label + ' rejected', time:'Just now'});
  }
  render();
}

function renderDeptSettings(){
  document.getElementById('dept-settings').innerHTML = DEPTS.map(d =>
    `<div class="form-row" style="display:flex;gap:10px;align-items:center;">
      <label style="min-width:180px;font-size:12px;color:#8890b0;">${d.name}</label>
      <input type="number" value="${d.budget}" style="flex:1;" oninput="updateDeptBudget('${d.id}',this.value)">
    </div>`
  ).join('');
}

function updateDeptBudget(id, val){
  const d = DEPTS.find(x=>x.id===id);
  if(d){ d.budget = Number(val)||0; render(); }
}

function updateSettings(){
  settings.name   = document.getElementById('set-name').value;
  settings.budget = Number(document.getElementById('set-budget').value)||0;
  settings.week   = Number(document.getElementById('set-week').value)||1;
  settings.weeks  = Number(document.getElementById('set-weeks').value)||1;
  render();
}

// ── MODAL ──
let modalMode = '';
function openModal(mode){
  modalMode = mode;
  const title = document.getElementById('modal-title');
  const body  = document.getElementById('modal-body');
  if(mode==='expense'){
    title.textContent = 'Log expense';
    body.innerHTML = `
      <div class="form-row"><label>Department</label>
        <select id="m-dept">${DEPTS.map(d=>`<option value="${d.id}">${d.name}</option>`).join('')}</select></div>
      <div class="form-row"><label>Description</label><input id="m-desc" placeholder="e.g. Camera rental day 42"></div>
      <div class="form-row"><label>Amount ($)</label><input id="m-amount" type="number" placeholder="0"></div>
      <div class="form-row"><label>Type</label>
        <select id="m-type"><option value="spent">Actual spend</option><option value="committed">Committed / PO</option></select></div>
      <div class="form-actions">
        <button class="btn-cancel" onclick="closeModal()">Cancel</button>
        <button class="btn-primary" onclick="submitExpense()">Log expense</button>
      </div>`;
  } else if(mode==='activity'){
    title.textContent = 'Add activity note';
    body.innerHTML = `
      <div class="form-row"><label>Note</label><input id="m-note" placeholder="What happened?"></div>
      <div class="form-row"><label>Type</label>
        <select id="m-note-type">
          <option value="#7090f0">Info</option>
          <option value="#30b878">Approved / resolved</option>
          <option value="#d08820">Warning</option>
          <option value="#d04040">Issue / flagged</option>
        </select></div>
      <div class="form-actions">
        <button class="btn-cancel" onclick="closeModal()">Cancel</button>
        <button class="btn-primary" onclick="submitActivity()">Add note</button>
      </div>`;
  } else if(mode==='approval'){
    title.textContent = 'Request approval';
    body.innerHTML = `
      <div class="form-row"><label>Description</label><input id="m-alabel" placeholder="e.g. Additional VFX days"></div>
      <div class="form-row"><label>Department</label>
        <select id="m-adept">${DEPTS.map(d=>`<option value="${d.id}">${d.name}</option>`).join('')}</select></div>
      <div class="form-row"><label>Amount ($)</label><input id="m-aamount" type="number" placeholder="0"></div>
      <div class="form-actions">
        <button class="btn-cancel" onclick="closeModal()">Cancel</button>
        <button class="btn-primary" onclick="submitApproval()">Submit request</button>
      </div>`;
  } else if(mode==='dept'){
    title.textContent = 'Edit department spend';
  }
  document.getElementById('modal-bg').classList.add('open');
}

function openDeptEdit(id){
  const d = DEPTS.find(x=>x.id===id);
  if(!d) return;
  modalMode = 'dept-edit';
  document.getElementById('modal-title').textContent = d.name;
  document.getElementById('modal-body').innerHTML = `
    <div class="form-row"><label>Budget ($)</label><input id="m-de-budget" type="number" value="${d.budget}"></div>
    <div class="form-row"><label>Spent to date ($)</label><input id="m-de-spent" type="number" value="${d.spent}"></div>
    <div class="form-actions">
      <button class="btn-cancel" onclick="closeModal()">Cancel</button>
      <button class="btn-primary" onclick="saveDeptEdit('${id}')">Save</button>
    </div>`;
  document.getElementById('modal-bg').classList.add('open');
}

function saveDeptEdit(id){
  const d = DEPTS.find(x=>x.id===id);
  d.budget = Number(document.getElementById('m-de-budget').value)||0;
  d.spent  = Number(document.getElementById('m-de-spent').value)||0;
  closeModal(); render();
}

function submitExpense(){
  const dept   = document.getElementById('m-dept').value;
  const desc   = document.getElementById('m-desc').value.trim();
  const amount = Number(document.getElementById('m-amount').value)||0;
  const type   = document.getElementById('m-type').value;
  if(!desc||!amount){ alert('Please fill in all fields.'); return; }
  const d = DEPTS.find(x=>x.id===dept);
  if(type==='spent'){ d.spent += amount; }
  else { committed += amount; }
  activities.unshift({ color: type==='spent'?'#7090f0':'#d08820', text: desc + ' — ' + fmt(amount) + ' (' + d.name + ')', time: 'Just now' });
  closeModal(); render();
}

function submitActivity(){
  const note  = document.getElementById('m-note').value.trim();
  const color = document.getElementById('m-note-type').value;
  if(!note){ alert('Please enter a note.'); return; }
  activities.unshift({ color, text: note, time: 'Just now' });
  closeModal(); renderActivity();
}

function submitApproval(){
  const label  = document.getElementById('m-alabel').value.trim();
  const dept   = document.getElementById('m-adept').value;
  const amount = Number(document.getElementById('m-aamount').value)||0;
  if(!label||!amount){ alert('Please fill in all fields.'); return; }
  approvals.unshift({ id: nextApprId++, label, amount, dept, status:'pending' });
  committed += amount;
  activities.unshift({ color:'#d08820', text: 'Approval requested: ' + label + ' — ' + fmt(amount), time:'Just now' });
  closeModal(); render();
}

function closeModal(){ document.getElementById('modal-bg').classList.remove('open'); }
function closeModalBg(e){ if(e.target===document.getElementById('modal-bg')) closeModal(); }

function switchTab(name, el){
  document.querySelectorAll('.tab').forEach(t=>t.classList.remove('active'));
  el.classList.add('active');
  ['overview','approvals','settings'].forEach(t=>{
    document.getElementById('tab-'+t).style.display = t===name?'':'none';
  });
}

render();
</script>
</body>
</html>
