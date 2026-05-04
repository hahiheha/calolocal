<!DOCTYPE html>
<html lang="vi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>CaloLocal</title>
<style>
  /* ── RESET & BASE ─────────────────────────────── */
  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
  :root {
    --green: #16a34a;
    --green-light: #dcfce7;
    --green-dark: #14532d;
    --green-mid: #22c55e;
    --amber: #d97706;
    --amber-light: #fef3c7;
    --red: #dc2626;
    --red-light: #fee2e2;
    --blue: #2563eb;
    --blue-light: #dbeafe;
    --gray-50: #f9fafb;
    --gray-100: #f3f4f6;
    --gray-200: #e5e7eb;
    --gray-400: #9ca3af;
    --gray-600: #4b5563;
    --gray-800: #1f2937;
    --gray-900: #111827;
    --white: #ffffff;
    --radius-sm: 8px;
    --radius-md: 12px;
    --radius-lg: 18px;
    --radius-xl: 24px;
    --shadow-sm: 0 1px 3px rgba(0,0,0,0.08), 0 1px 2px rgba(0,0,0,0.04);
    --shadow-md: 0 4px 16px rgba(0,0,0,0.10), 0 2px 6px rgba(0,0,0,0.06);
  }
  html { font-size: 16px; }
  body {
    font-family: 'Segoe UI', system-ui, -apple-system, sans-serif;
    background: #f0fdf4;
    color: var(--gray-900);
    min-height: 100vh;
    padding-bottom: 80px;
  }

  /* ── LAYOUT ───────────────────────────────────── */
  .app { max-width: 430px; margin: 0 auto; padding: 0 16px; }

  /* ── TOP BAR ──────────────────────────────────── */
  .topbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px 0 12px;
  }
  .logo { font-size: 22px; font-weight: 700; letter-spacing: -0.5px; color: var(--gray-900); }
  .logo span { color: var(--green); }
  .date-badge {
    font-size: 12px;
    color: var(--gray-600);
    background: var(--white);
    border: 1px solid var(--gray-200);
    border-radius: 20px;
    padding: 4px 12px;
  }

  /* ── SCREENS ──────────────────────────────────── */
  .screen { display: none; }
  .screen.active { display: block; }

  /* ── BOTTOM NAV ───────────────────────────────── */
  .bottom-nav {
    position: fixed;
    bottom: 0; left: 0; right: 0;
    background: var(--white);
    border-top: 1px solid var(--gray-200);
    display: flex;
    justify-content: space-around;
    padding: 8px 0 12px;
    z-index: 100;
    box-shadow: 0 -4px 20px rgba(0,0,0,0.06);
  }
  .nav-item {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 3px;
    cursor: pointer;
    padding: 4px 16px;
    border-radius: var(--radius-sm);
    transition: background 0.15s;
    border: none;
    background: transparent;
    color: var(--gray-400);
    font-size: 11px;
    font-weight: 500;
  }
  .nav-item.active { color: var(--green); }
  .nav-item svg { width: 22px; height: 22px; }
  .nav-dot {
    width: 4px; height: 4px;
    border-radius: 50%;
    background: var(--green);
    margin-top: 2px;
    opacity: 0;
    transition: opacity 0.15s;
  }
  .nav-item.active .nav-dot { opacity: 1; }

  /* ── CARDS ────────────────────────────────────── */
  .card {
    background: var(--white);
    border-radius: var(--radius-lg);
    padding: 16px 18px;
    margin-bottom: 12px;
    box-shadow: var(--shadow-sm);
    border: 1px solid var(--gray-100);
  }
  .card-title {
    font-size: 13px;
    font-weight: 600;
    color: var(--gray-600);
    text-transform: uppercase;
    letter-spacing: 0.5px;
    margin-bottom: 12px;
  }

  /* ── STREAK CARD ──────────────────────────────── */
  .streak-card {
    background: linear-gradient(135deg, #052e16 0%, #14532d 100%);
    color: white;
    border-radius: var(--radius-xl);
    padding: 20px;
    margin-bottom: 12px;
    box-shadow: var(--shadow-md);
    position: relative;
    overflow: hidden;
  }
  .streak-card::before {
    content: '';
    position: absolute;
    top: -30px; right: -30px;
    width: 120px; height: 120px;
    border-radius: 50%;
    background: rgba(255,255,255,0.04);
  }
  .streak-card::after {
    content: '';
    position: absolute;
    bottom: -20px; left: 40px;
    width: 80px; height: 80px;
    border-radius: 50%;
    background: rgba(255,255,255,0.03);
  }
  .streak-top { display: flex; align-items: center; justify-content: space-between; }
  .streak-left { display: flex; align-items: center; gap: 12px; }
  .streak-fire { font-size: 36px; line-height: 1; }
  .streak-number { font-size: 44px; font-weight: 800; line-height: 1; }
  .streak-label { font-size: 12px; opacity: 0.7; margin-top: 2px; }
  .streak-right { text-align: right; }
  .level-badge {
    display: inline-block;
    background: rgba(255,255,255,0.15);
    border: 1px solid rgba(255,255,255,0.2);
    border-radius: 20px;
    padding: 4px 12px;
    font-size: 12px;
    font-weight: 600;
  }
  .freeze-info { font-size: 11px; opacity: 0.6; margin-top: 6px; }
  .week-dots { display: flex; gap: 6px; margin-top: 16px; }
  .week-dot-wrap { flex: 1; text-align: center; }
  .week-dot {
    width: 32px; height: 8px;
    border-radius: 4px;
    background: rgba(255,255,255,0.15);
    margin: 0 auto 4px;
    transition: background 0.2s;
  }
  .week-dot.done { background: var(--green-mid); }
  .week-dot.today { background: #fbbf24; }
  .week-dot.missed { background: rgba(255,255,255,0.08); }
  .week-day { font-size: 10px; opacity: 0.5; }

  /* ── CALO RING ────────────────────────────────── */
  .calo-section { display: flex; align-items: center; gap: 16px; }
  .ring-wrap { position: relative; width: 100px; height: 100px; flex-shrink: 0; }
  .ring-wrap svg { transform: rotate(-90deg); }
  .ring-center {
    position: absolute; top: 50%; left: 50%;
    transform: translate(-50%, -50%);
    text-align: center;
  }
  .ring-num { font-size: 20px; font-weight: 700; line-height: 1; }
  .ring-sub { font-size: 10px; color: var(--gray-400); }
  .macro-pills { display: flex; flex-direction: column; gap: 6px; flex: 1; }
  .macro-pill { display: flex; align-items: center; gap: 8px; }
  .macro-bar-wrap { flex: 1; height: 6px; background: var(--gray-100); border-radius: 3px; overflow: hidden; }
  .macro-bar { height: 100%; border-radius: 3px; transition: width 0.5s; }
  .macro-label { font-size: 11px; color: var(--gray-600); width: 56px; }
  .macro-val { font-size: 11px; font-weight: 600; width: 32px; text-align: right; }

  /* ── FORGIVENESS BANNER ───────────────────────── */
  .forgive-banner {
    background: linear-gradient(135deg, #f0fdf4, #dcfce7);
    border: 1px solid #bbf7d0;
    border-radius: var(--radius-md);
    padding: 12px 14px;
    margin-bottom: 12px;
    display: flex;
    gap: 10px;
    align-items: flex-start;
  }
  .forgive-icon { font-size: 18px; flex-shrink: 0; }
  .forgive-text { font-size: 13px; color: #15803d; line-height: 1.5; }

  /* ── MEAL CARDS ───────────────────────────────── */
  .meal-entry {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    padding: 10px 0;
    border-bottom: 1px solid var(--gray-100);
  }
  .meal-entry:last-child { border-bottom: none; }
  .meal-name { font-size: 14px; font-weight: 500; }
  .meal-time { font-size: 11px; color: var(--gray-400); margin-top: 2px; }
  .meal-right { text-align: right; }
  .meal-calo { font-size: 14px; font-weight: 600; }
  .mqs-pill {
    display: inline-block;
    font-size: 10px;
    font-weight: 700;
    padding: 2px 7px;
    border-radius: 20px;
    margin-top: 3px;
  }
  .mqs-high { background: var(--green-light); color: #15803d; }
  .mqs-mid  { background: var(--amber-light); color: #92400e; }
  .mqs-low  { background: var(--red-light); color: #991b1b; }
  .empty-log {
    text-align: center;
    padding: 24px 0;
    color: var(--gray-400);
    font-size: 14px;
  }
  .empty-icon { font-size: 32px; margin-bottom: 8px; }

  /* ── BUTTONS ──────────────────────────────────── */
  .btn {
    display: block; width: 100%;
    padding: 13px;
    border: none; border-radius: var(--radius-md);
    font-size: 15px; font-weight: 600;
    cursor: pointer;
    transition: all 0.15s;
    letter-spacing: -0.2px;
  }
  .btn-green { background: var(--green); color: white; }
  .btn-green:hover { background: #15803d; transform: translateY(-1px); box-shadow: 0 4px 12px rgba(22,163,74,0.3); }
  .btn-green:active { transform: translateY(0); }
  .btn-outline {
    background: transparent;
    border: 1.5px solid var(--gray-200);
    color: var(--gray-600);
    font-weight: 500;
    margin-top: 8px;
  }
  .btn-outline:hover { background: var(--gray-50); border-color: var(--gray-300); }
  .btn-sm {
    display: inline-block; width: auto;
    padding: 7px 16px;
    font-size: 13px;
  }

  /* ── LOG SCREEN ───────────────────────────────── */
  .mode-tabs { display: flex; gap: 4px; background: var(--gray-100); border-radius: var(--radius-sm); padding: 3px; margin-bottom: 16px; }
  .mode-tab {
    flex: 1; padding: 8px; text-align: center;
    font-size: 13px; font-weight: 500;
    border-radius: 7px; cursor: pointer;
    border: none; background: transparent;
    color: var(--gray-600); transition: all 0.15s;
  }
  .mode-tab.active { background: var(--white); color: var(--gray-900); box-shadow: var(--shadow-sm); }
  .log-panel { display: none; }
  .log-panel.active { display: block; }
  textarea {
    width: 100%; padding: 12px 14px;
    border: 1.5px solid var(--gray-200);
    border-radius: var(--radius-md);
    font-size: 14px; font-family: inherit;
    resize: none; height: 90px;
    color: var(--gray-900);
    background: var(--white);
    outline: none; transition: border 0.15s;
    line-height: 1.5;
  }
  textarea:focus { border-color: var(--green); }
  textarea::placeholder { color: var(--gray-400); }

  /* ── STREET FOOD LIST ─────────────────────────── */
  .sf-search {
    width: 100%; padding: 10px 14px;
    border: 1.5px solid var(--gray-200);
    border-radius: var(--radius-md);
    font-size: 14px; font-family: inherit;
    margin-bottom: 10px; outline: none;
    transition: border 0.15s; color: var(--gray-900);
  }
  .sf-search:focus { border-color: var(--green); }
  .sf-list { max-height: 320px; overflow-y: auto; }
  .sf-item {
    display: flex; justify-content: space-between;
    align-items: center; padding: 11px 0;
    border-bottom: 1px solid var(--gray-100);
    cursor: pointer; transition: background 0.1s;
    gap: 8px;
  }
  .sf-item:hover { background: var(--gray-50); margin: 0 -4px; padding: 11px 4px; border-radius: 6px; }
  .sf-item:last-child { border-bottom: none; }
  .sf-name { font-size: 14px; font-weight: 500; }
  .sf-meta { font-size: 11px; color: var(--gray-400); margin-top: 2px; }
  .sf-calo { font-size: 14px; font-weight: 700; color: var(--green); white-space: nowrap; }
  .sf-add-btn {
    width: 28px; height: 28px;
    border-radius: 50%; background: var(--green-light);
    color: var(--green); border: none; cursor: pointer;
    font-size: 18px; font-weight: 700;
    display: flex; align-items: center; justify-content: center;
    flex-shrink: 0; transition: all 0.15s;
  }
  .sf-add-btn:hover { background: var(--green); color: white; }

  /* ── RESULT CARD ──────────────────────────────── */
  .result-card {
    background: var(--gray-50);
    border: 1.5px solid var(--green);
    border-radius: var(--radius-md);
    padding: 14px; margin: 12px 0;
  }
  .result-header { display: flex; justify-content: space-between; align-items: center; margin-bottom: 10px; }
  .result-title { font-size: 13px; font-weight: 700; color: var(--green); }
  .result-row { display: flex; justify-content: space-between; font-size: 13px; padding: 5px 0; border-bottom: 1px solid var(--gray-200); }
  .result-row:last-of-type { border-bottom: none; }
  .result-total { display: flex; justify-content: space-between; font-size: 15px; font-weight: 700; margin-top: 10px; padding-top: 10px; border-top: 1.5px solid var(--gray-200); }
  .mqs-score-wrap { margin-top: 12px; }
  .mqs-score-label { display: flex; justify-content: space-between; font-size: 12px; color: var(--gray-600); margin-bottom: 5px; }
  .mqs-track { height: 10px; background: var(--gray-200); border-radius: 5px; overflow: hidden; }
  .mqs-fill { height: 100%; border-radius: 5px; transition: width 0.6s cubic-bezier(0.34, 1.56, 0.64, 1); }
  .forgive-result { background: #f0fdf4; border-radius: var(--radius-sm); padding: 10px 12px; margin-top: 10px; font-size: 12px; color: #15803d; line-height: 1.5; }

  /* ── STATS SCREEN ─────────────────────────────── */
  .bio-card {
    background: linear-gradient(135deg, #052e16, #064e3b);
    color: white;
    border-radius: var(--radius-xl);
    padding: 20px;
    margin-bottom: 12px;
    box-shadow: var(--shadow-md);
  }
  .bio-age { font-size: 52px; font-weight: 800; line-height: 1; }
  .bio-label { font-size: 13px; opacity: 0.7; margin-top: 4px; }
  .bio-note { font-size: 12px; opacity: 0.85; margin-top: 12px; line-height: 1.5; }
  .stat-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 8px; margin-bottom: 12px; }
  .stat-cell { background: var(--white); border-radius: var(--radius-md); padding: 14px; border: 1px solid var(--gray-100); }
  .stat-v { font-size: 24px; font-weight: 700; line-height: 1; }
  .stat-k { font-size: 11px; color: var(--gray-400); margin-top: 4px; }
  .bar-chart { display: flex; align-items: flex-end; gap: 6px; height: 80px; padding-bottom: 4px; }
  .bar-col { flex: 1; display: flex; flex-direction: column; align-items: center; gap: 4px; }
  .bar-body { width: 100%; border-radius: 4px 4px 0 0; min-height: 4px; transition: height 0.4s; }
  .bar-day { font-size: 10px; color: var(--gray-400); }
  .chart-goal-line {
    border-top: 1.5px dashed var(--gray-300);
    position: relative;
    margin: 0 0 6px 0;
  }
  .chart-goal-line span { position: absolute; right: 0; top: -18px; font-size: 10px; color: var(--gray-400); }

  /* ── ONBOARDING SCREEN ────────────────────────── */
  .onboard-wrap { padding: 20px 0; }
  .onboard-title { font-size: 26px; font-weight: 800; letter-spacing: -0.5px; margin-bottom: 6px; }
  .onboard-sub { font-size: 15px; color: var(--gray-600); margin-bottom: 28px; line-height: 1.5; }
  .form-group { margin-bottom: 16px; }
  .form-label { font-size: 13px; font-weight: 600; color: var(--gray-700); margin-bottom: 6px; display: block; }
  .form-input {
    width: 100%; padding: 11px 14px;
    border: 1.5px solid var(--gray-200);
    border-radius: var(--radius-md);
    font-size: 15px; font-family: inherit;
    outline: none; transition: border 0.15s;
    color: var(--gray-900);
  }
  .form-input:focus { border-color: var(--green); }
  .form-row { display: grid; grid-template-columns: 1fr 1fr; gap: 10px; }
  .goal-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 8px; margin-top: 6px; }
  .goal-btn {
    padding: 12px 8px; border: 1.5px solid var(--gray-200);
    border-radius: var(--radius-md); background: var(--white);
    cursor: pointer; text-align: center; transition: all 0.15s;
    font-size: 13px; font-weight: 500; color: var(--gray-700);
  }
  .goal-btn:hover { border-color: var(--green); color: var(--green); }
  .goal-btn.selected { border-color: var(--green); background: var(--green-light); color: var(--green); font-weight: 600; }
  .goal-icon { font-size: 20px; display: block; margin-bottom: 4px; }

  /* ── TOAST ────────────────────────────────────── */
  .toast {
    position: fixed; bottom: 90px; left: 50%; transform: translateX(-50%) translateY(20px);
    background: var(--gray-900); color: white;
    padding: 10px 20px; border-radius: 20px;
    font-size: 13px; font-weight: 500;
    opacity: 0; transition: all 0.3s;
    z-index: 200; white-space: nowrap;
    box-shadow: var(--shadow-md);
  }
  .toast.show { opacity: 1; transform: translateX(-50%) translateY(0); }

  /* ── MODAL ────────────────────────────────────── */
  .modal-overlay {
    display: none; position: fixed;
    inset: 0; background: rgba(0,0,0,0.4);
    z-index: 300; align-items: flex-end; justify-content: center;
  }
  .modal-overlay.open { display: flex; }
  .modal {
    background: var(--white);
    border-radius: var(--radius-xl) var(--radius-xl) 0 0;
    padding: 24px 20px 36px;
    width: 100%; max-width: 430px;
    max-height: 80vh; overflow-y: auto;
    animation: slideUp 0.25s ease;
  }
  @keyframes slideUp { from { transform: translateY(40px); opacity: 0; } to { transform: translateY(0); opacity: 1; } }
  .modal-handle { width: 36px; height: 4px; background: var(--gray-200); border-radius: 2px; margin: 0 auto 20px; }
  .modal-title { font-size: 18px; font-weight: 700; margin-bottom: 16px; }

  /* ── QUANTITY SELECTOR ────────────────────────── */
  .qty-row { display: flex; gap: 8px; margin-bottom: 12px; }
  .qty-btn {
    flex: 1; padding: 10px;
    border: 1.5px solid var(--gray-200);
    border-radius: var(--radius-sm);
    background: var(--white); cursor: pointer;
    font-size: 13px; font-weight: 500; color: var(--gray-700);
    transition: all 0.15s;
  }
  .qty-btn.active { border-color: var(--green); background: var(--green-light); color: var(--green); }

  /* ── SECTION HEADER ───────────────────────────── */
  .section-header { display: flex; justify-content: space-between; align-items: center; margin-bottom: 10px; }
  .section-title { font-size: 15px; font-weight: 700; color: var(--gray-900); }
  .section-action { font-size: 12px; color: var(--green); cursor: pointer; font-weight: 500; }

  /* ── SCROLLBAR ────────────────────────────────── */
  .sf-list::-webkit-scrollbar { width: 4px; }
  .sf-list::-webkit-scrollbar-track { background: transparent; }
  .sf-list::-webkit-scrollbar-thumb { background: var(--gray-200); border-radius: 2px; }
</style>
</head>
<body>

<div class="app">
  <div class="topbar">
    <div class="logo">Calo<span>Local</span></div>
    <div class="date-badge" id="date-display"></div>
  </div>

  <!-- ═══ SCREEN: ONBOARDING ═══ -->
  <div id="screen-onboard" class="screen active">
    <div class="onboard-wrap">
      <div class="onboard-title">Chào mừng! 👋</div>
      <div class="onboard-sub">CaloLocal giúp bạn theo dõi dinh dưỡng theo cách của người Việt — không áp lực, không phán xét.</div>
      <div class="form-group">
        <label class="form-label">Tên của bạn</label>
        <input class="form-input" id="ob-name" type="text" placeholder="Nguyễn Thị An">
      </div>
      <div class="form-row">
        <div class="form-group">
          <label class="form-label">Tuổi</label>
          <input class="form-input" id="ob-age" type="number" placeholder="23" min="14" max="80">
        </div>
        <div class="form-group">
          <label class="form-label">Giới tính</label>
          <select class="form-input" id="ob-gender">
            <option value="female">Nữ</option>
            <option value="male">Nam</option>
          </select>
        </div>
      </div>
      <div class="form-row">
        <div class="form-group">
          <label class="form-label">Cân nặng (kg)</label>
          <input class="form-input" id="ob-weight" type="number" placeholder="55">
        </div>
        <div class="form-group">
          <label class="form-label">Chiều cao (cm)</label>
          <input class="form-input" id="ob-height" type="number" placeholder="162">
        </div>
      </div>
      <div class="form-group">
        <label class="form-label">Mục tiêu của bạn</label>
        <div class="goal-grid" id="goal-grid">
          <button class="goal-btn" data-goal="lose" onclick="selectGoal(this)"><span class="goal-icon">📉</span>Giảm cân</button>
          <button class="goal-btn" data-goal="maintain" onclick="selectGoal(this)"><span class="goal-icon">⚖️</span>Duy trì</button>
          <button class="goal-btn" data-goal="gain" onclick="selectGoal(this)"><span class="goal-icon">💪</span>Tăng cơ</button>
          <button class="goal-btn" data-goal="health" onclick="selectGoal(this)"><span class="goal-icon">🌿</span>Ăn lành mạnh</button>
        </div>
      </div>
      <button class="btn btn-green" onclick="completeOnboarding()">Bắt đầu theo dõi →</button>
    </div>
  </div>

  <!-- ═══ SCREEN: HOME ═══ -->
  <div id="screen-home" class="screen">
    <!-- Streak Card -->
    <div class="streak-card">
      <div class="streak-top">
        <div class="streak-left">
          <div class="streak-fire">🔥</div>
          <div>
            <div class="streak-number" id="streak-num">0</div>
            <div class="streak-label">ngày liên tiếp</div>
          </div>
        </div>
        <div class="streak-right">
          <div class="level-badge" id="level-badge">Mầm xanh 🌱</div>
          <div class="freeze-info">❄️ <span id="freeze-count">1</span> lượt streak freeze</div>
        </div>
      </div>
      <div class="week-dots" id="week-dots"></div>
    </div>

    <!-- Forgiveness Banner (shown when needed) -->
    <div class="forgive-banner" id="forgive-banner" style="display:none">
      <div class="forgive-icon">💚</div>
      <div class="forgive-text" id="forgive-text"></div>
    </div>

    <!-- Calo Ring -->
    <div class="card">
      <div class="calo-section">
        <div class="ring-wrap">
          <svg width="100" height="100" viewBox="0 0 100 100">
            <circle cx="50" cy="50" r="40" fill="none" stroke="#e5e7eb" stroke-width="10"/>
            <circle id="ring-circle" cx="50" cy="50" r="40" fill="none" stroke="#16a34a" stroke-width="10"
              stroke-dasharray="251" stroke-dashoffset="251" stroke-linecap="round"
              style="transition: stroke-dashoffset 0.6s cubic-bezier(0.34,1.2,0.64,1)"/>
          </svg>
          <div class="ring-center">
            <div class="ring-num" id="ring-ate">0</div>
            <div class="ring-sub">/ <span id="ring-goal">1800</span></div>
          </div>
        </div>
        <div class="macro-pills">
          <div class="macro-pill">
            <div class="macro-label" style="color:#2563eb">Protein</div>
            <div class="macro-bar-wrap"><div class="macro-bar" id="bar-protein" style="background:#2563eb; width:0%"></div></div>
            <div class="macro-val" id="val-protein" style="color:#2563eb">0g</div>
          </div>
          <div class="macro-pill">
            <div class="macro-label" style="color:#d97706">Carbs</div>
            <div class="macro-bar-wrap"><div class="macro-bar" id="bar-carbs" style="background:#d97706; width:0%"></div></div>
            <div class="macro-val" id="val-carbs" style="color:#d97706">0g</div>
          </div>
          <div class="macro-pill">
            <div class="macro-label" style="color:#dc2626">Chất béo</div>
            <div class="macro-bar-wrap"><div class="macro-bar" id="bar-fat" style="background:#dc2626; width:0%"></div></div>
            <div class="macro-val" id="val-fat" style="color:#dc2626">0g</div>
          </div>
          <div style="font-size:11px; color:var(--gray-400); margin-top:2px">
            Còn <strong id="remaining-calo" style="color:var(--green)">0</strong> calo hôm nay
          </div>
        </div>
      </div>
    </div>

    <!-- Meal Log -->
    <div class="section-header">
      <div class="section-title">Bữa ăn hôm nay</div>
      <div class="section-action" onclick="switchTab('log')">+ Thêm món</div>
    </div>
    <div class="card" id="meal-log-card">
      <div class="empty-log" id="empty-log">
        <div class="empty-icon">🍜</div>
        Chưa có bữa nào hôm nay<br>
        <span style="font-size:12px;color:var(--gray-400)">Nhấn "+ Thêm món" để bắt đầu</span>
      </div>
      <div id="meal-entries"></div>
    </div>

    <button class="btn btn-green" onclick="switchTab('log')">🍽️ Ghi bữa ăn mới</button>
  </div>

  <!-- ═══ SCREEN: LOG ═══ -->
  <div id="screen-log" class="screen">
    <div class="card">
      <div class="mode-tabs">
        <button class="mode-tab active" onclick="setLogMode('text', this)">✏️ Gõ tên</button>
        <button class="mode-tab" onclick="setLogMode('street', this)">🛵 Vỉa hè</button>
        <button class="mode-tab" onclick="setLogMode('manual', this)">🔢 Tự nhập</button>
      </div>

      <!-- Text mode -->
      <div id="log-text" class="log-panel active">
        <textarea id="food-text-input" placeholder="VD: Bún bò Huế 1 tô&#10;Hoặc: Cơm gà + canh cải + nước ngọt&#10;Nhập bất kỳ món gì bạn đã ăn..."></textarea>
        <button class="btn btn-green" style="margin-top:10px" onclick="analyzeTextInput()">Tính dinh dưỡng</button>
      </div>

      <!-- Street food mode -->
      <div id="log-street" class="log-panel">
        <input class="sf-search" id="sf-search" type="text" placeholder="🔍 Tìm món vỉa hè... (bún, bánh mì, xôi...)" oninput="filterStreetFood()">
        <div class="sf-list" id="sf-list"></div>
      </div>

      <!-- Manual mode -->
      <div id="log-manual" class="log-panel">
        <div class="form-group">
          <label class="form-label">Tên món</label>
          <input class="form-input" id="manual-name" type="text" placeholder="Tên món ăn">
        </div>
        <div class="form-row">
          <div class="form-group">
            <label class="form-label">Calo</label>
            <input class="form-input" id="manual-calo" type="number" placeholder="500">
          </div>
          <div class="form-group">
            <label class="form-label">Protein (g)</label>
            <input class="form-input" id="manual-protein" type="number" placeholder="20">
          </div>
        </div>
        <div class="form-row">
          <div class="form-group">
            <label class="form-label">Carbs (g)</label>
            <input class="form-input" id="manual-carbs" type="number" placeholder="60">
          </div>
          <div class="form-group">
            <label class="form-label">Chất béo (g)</label>
            <input class="form-input" id="manual-fat" type="number" placeholder="15">
          </div>
        </div>
        <button class="btn btn-green" onclick="addManualEntry()">Ghi vào nhật ký</button>
      </div>

      <!-- Result (shared) -->
      <div id="log-result" style="display:none"></div>
    </div>
  </div>

  <!-- ═══ SCREEN: STATS ═══ -->
  <div id="screen-stats" class="screen">
    <!-- Bio Age -->
    <div class="bio-card">
      <div class="bio-age" id="bio-age">--</div>
      <div class="bio-label">Tuổi sinh học ước tính</div>
      <div class="bio-note" id="bio-note">Hãy ghi lại bữa ăn trong 3 ngày để tính tuổi sinh học của bạn.</div>
    </div>

    <!-- Stats Grid -->
    <div class="stat-grid">
      <div class="stat-cell">
        <div class="stat-v" id="stat-streak">0 🔥</div>
        <div class="stat-k">Streak hiện tại</div>
      </div>
      <div class="stat-cell">
        <div class="stat-v" id="stat-avg-calo">--</div>
        <div class="stat-k">Calo TB / ngày</div>
      </div>
      <div class="stat-cell">
        <div class="stat-v" id="stat-avg-mqs" style="color:var(--green)">--</div>
        <div class="stat-k">MQS trung bình</div>
      </div>
      <div class="stat-cell">
        <div class="stat-v" id="stat-total-logs">0</div>
        <div class="stat-k">Bữa đã ghi</div>
      </div>
    </div>

    <!-- Weekly chart -->
    <div class="card">
      <div class="card-title">Calo 7 ngày gần nhất</div>
      <div class="chart-goal-line"><span>Mục tiêu</span></div>
      <div class="bar-chart" id="week-chart"></div>
    </div>

    <!-- MQS breakdown -->
    <div class="card">
      <div class="card-title">Phân tích chất lượng bữa ăn</div>
      <div id="mqs-breakdown">
        <div style="text-align:center;color:var(--gray-400);font-size:14px;padding:16px 0">
          Chưa có dữ liệu. Hãy ghi thêm bữa ăn!
        </div>
      </div>
    </div>

    <!-- Reset button -->
    <button class="btn btn-outline" onclick="confirmReset()">🗑️ Xoá toàn bộ dữ liệu</button>
  </div>
</div>

<!-- Bottom Nav -->
<nav class="bottom-nav">
  <button class="nav-item active" id="nav-home" onclick="switchTab('home')">
    <svg fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M3 12l2-2m0 0l7-7 7 7M5 10v10a1 1 0 001 1h3m10-11l2 2m-2-2v10a1 1 0 01-1 1h-3m-6 0a1 1 0 001-1v-4a1 1 0 011-1h2a1 1 0 011 1v4a1 1 0 001 1m-6 0h6"/></svg>
    Hôm nay
    <div class="nav-dot"></div>
  </button>
  <button class="nav-item" id="nav-log" onclick="switchTab('log')">
    <svg fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M12 4v16m8-8H4"/></svg>
    Ghi món
    <div class="nav-dot"></div>
  </button>
  <button class="nav-item" id="nav-stats" onclick="switchTab('stats')">
    <svg fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path d="M9 19v-6a2 2 0 00-2-2H5a2 2 0 00-2 2v6a2 2 0 002 2h2a2 2 0 002-2zm0 0V9a2 2 0 012-2h2a2 2 0 012 2v10m-6 0a2 2 0 002 2h2a2 2 0 002-2m0 0V5a2 2 0 012-2h2a2 2 0 012 2v14a2 2 0 01-2 2h-2a2 2 0 01-2-2z"/></svg>
    Thống kê
    <div class="nav-dot"></div>
  </button>
</nav>

<!-- Toast -->
<div class="toast" id="toast"></div>

<!-- Confirm Modal -->
<div class="modal-overlay" id="modal-confirm">
  <div class="modal">
    <div class="modal-handle"></div>
    <div class="modal-title" id="modal-title">Xác nhận</div>
    <div id="modal-body" style="font-size:14px;color:var(--gray-600);margin-bottom:20px;line-height:1.6"></div>
    <button class="btn btn-green" id="modal-ok" onclick="closeModal()">Xác nhận</button>
    <button class="btn btn-outline" onclick="closeModal()">Huỷ</button>
  </div>
</div>

<script>
// ══════════════════════════════════════════
// DATA — Vietnamese street food database
// ══════════════════════════════════════════
const STREET_FOODS = [
  // Phở & bún
  {name:"Phở bò Hà Nội",cat:"Phở & bún",calo:450,p:28,c:55,f:11,region:"HN"},
  {name:"Phở gà Hà Nội",cat:"Phở & bún",calo:380,p:24,c:50,f:8,region:"HN"},
  {name:"Phở bò Sài Gòn",cat:"Phở & bún",calo:520,p:30,c:60,f:13,region:"HCM"},
  {name:"Bún bò Huế",cat:"Phở & bún",calo:520,p:32,c:62,f:14,region:"Trung"},
  {name:"Bún riêu cua",cat:"Phở & bún",calo:420,p:24,c:52,f:10,region:"HN"},
  {name:"Bún chả Hà Nội",cat:"Phở & bún",calo:560,p:36,c:58,f:18,region:"HN"},
  {name:"Bún thịt nướng",cat:"Phở & bún",calo:480,p:28,c:56,f:14,region:"HCM"},
  {name:"Bún mắm",cat:"Phở & bún",calo:490,p:26,c:58,f:15,region:"HCM"},
  {name:"Hủ tiếu",cat:"Phở & bún",calo:420,p:22,c:52,f:12,region:"HCM"},
  {name:"Miến gà",cat:"Phở & bún",calo:360,p:20,c:48,f:8,region:"HN"},
  // Cơm
  {name:"Cơm gà xối mỡ",cat:"Cơm",calo:680,p:38,c:72,f:24,region:"HCM"},
  {name:"Cơm tấm sườn bì",cat:"Cơm",calo:720,p:38,c:75,f:28,region:"HCM"},
  {name:"Cơm rang trứng",cat:"Cơm",calo:520,p:18,c:70,f:18,region:"ALL"},
  {name:"Cơm bình dân 3 món",cat:"Cơm",calo:580,p:30,c:68,f:20,region:"ALL"},
  {name:"Cơm chiên dương châu",cat:"Cơm",calo:620,p:22,c:78,f:22,region:"ALL"},
  // Bánh mì & xôi
  {name:"Bánh mì thịt vỉa hè",cat:"Bánh mì & xôi",calo:380,p:18,c:42,f:14,region:"ALL"},
  {name:"Bánh mì trứng",cat:"Bánh mì & xôi",calo:320,p:14,c:40,f:12,region:"ALL"},
  {name:"Bánh mì pate",cat:"Bánh mì & xôi",calo:350,p:16,c:38,f:16,region:"ALL"},
  {name:"Xôi xéo",cat:"Bánh mì & xôi",calo:320,p:8,c:58,f:8,region:"HN"},
  {name:"Xôi gà",cat:"Bánh mì & xôi",calo:420,p:22,c:56,f:12,region:"ALL"},
  {name:"Xôi chiên phồng",cat:"Bánh mì & xôi",calo:280,p:6,c:48,f:8,region:"HCM"},
  // Bánh
  {name:"Bánh cuốn nhân thịt",cat:"Bánh",calo:280,p:12,c:38,f:8,region:"HN"},
  {name:"Bánh khọt",cat:"Bánh",calo:320,p:14,c:36,f:14,region:"HCM"},
  {name:"Bánh xèo nhỏ",cat:"Bánh",calo:180,p:8,c:20,f:8,region:"Trung"},
  {name:"Bánh căn",cat:"Bánh",calo:220,p:10,c:28,f:8,region:"Trung"},
  {name:"Bánh tráng trộn",cat:"Bánh",calo:260,p:8,c:40,f:8,region:"HCM"},
  // Đồ nhậu & ăn vặt
  {name:"Ốc luộc (phần)",cat:"Ăn vặt",calo:140,p:18,c:8,f:3,region:"ALL"},
  {name:"Ngô nướng bơ",cat:"Ăn vặt",calo:180,p:4,c:32,f:5,region:"ALL"},
  {name:"Khoai lang nướng",cat:"Ăn vặt",calo:130,p:2,c:30,f:1,region:"ALL"},
  {name:"Bắp xào",cat:"Ăn vặt",calo:210,p:5,c:38,f:5,region:"ALL"},
  // Đồ uống
  {name:"Trà sữa trân châu (vừa)",cat:"Đồ uống",calo:380,p:3,c:68,f:10,region:"ALL"},
  {name:"Trà sữa trân châu (lớn)",cat:"Đồ uống",calo:520,p:4,c:90,f:14,region:"ALL"},
  {name:"Cà phê sữa đá",cat:"Đồ uống",calo:130,p:3,c:22,f:4,region:"ALL"},
  {name:"Nước mía",cat:"Đồ uống",calo:160,p:1,c:40,f:0,region:"ALL"},
  {name:"Sinh tố bơ",cat:"Đồ uống",calo:280,p:4,c:28,f:16,region:"ALL"},
  {name:"Trà đá (không đường)",cat:"Đồ uống",calo:5,p:0,c:1,f:0,region:"ALL"},
  {name:"Nước ngọt lon",cat:"Đồ uống",calo:140,p:0,c:36,f:0,region:"ALL"},
  // Súp & lẩu
  {name:"Lẩu thái 1 người",cat:"Lẩu & súp",calo:480,p:28,c:36,f:22,region:"ALL"},
  {name:"Cháo gà",cat:"Lẩu & súp",calo:240,p:16,c:36,f:4,region:"ALL"},
  {name:"Súp cua",cat:"Lẩu & súp",calo:180,p:12,c:24,f:4,region:"ALL"},
];

// Simple keyword-to-nutrition estimator for text input (V1 no-AI version)
const TEXT_ESTIMATES = {
  "phở": {calo:450,p:28,c:55,f:11},
  "bún bò": {calo:520,p:32,c:62,f:14},
  "bún riêu": {calo:420,p:24,c:52,f:10},
  "bún chả": {calo:560,p:36,c:58,f:18},
  "bún thịt": {calo:480,p:28,c:56,f:14},
  "bánh mì": {calo:360,p:16,c:40,f:13},
  "cơm tấm": {calo:720,p:38,c:75,f:28},
  "cơm gà": {calo:680,p:38,c:72,f:24},
  "cơm rang": {calo:520,p:18,c:70,f:18},
  "cơm": {calo:580,p:28,c:68,f:18},
  "xôi": {calo:340,p:10,c:58,f:8},
  "bánh cuốn": {calo:280,p:12,c:38,f:8},
  "trà sữa": {calo:400,p:3,c:72,f:11},
  "cà phê sữa": {calo:130,p:3,c:22,f:4},
  "ốc": {calo:140,p:18,c:8,f:3},
  "lẩu": {calo:480,p:28,c:36,f:22},
  "cháo": {calo:240,p:16,c:36,f:4},
  "hủ tiếu": {calo:420,p:22,c:52,f:12},
  "miến": {calo:360,p:20,c:48,f:8},
};

// ══════════════════════════════════════════
// STATE — read from localStorage
// ══════════════════════════════════════════
function loadState() {
  return JSON.parse(localStorage.getItem('calolocal_v1') || 'null');
}
function saveState(s) {
  localStorage.setItem('calolocal_v1', JSON.stringify(s));
}
function getToday() {
  return new Date().toISOString().split('T')[0];
}
function initState() {
  return {
    profile: null,         // {name, age, gender, weight, height, goal, tdee}
    streak: 0,
    streakFreezes: 1,
    lastLogDate: null,
    weekLog: {},           // { "2025-01-01": [{name, calo, p, c, f, mqs, time}] }
    totalLogs: 0,
  };
}

let STATE = loadState() || initState();

// ══════════════════════════════════════════
// TDEE CALCULATOR
// ══════════════════════════════════════════
function calcTDEE(profile) {
  // Mifflin-St Jeor
  let bmr;
  if (profile.gender === 'male') {
    bmr = 10 * profile.weight + 6.25 * profile.height - 5 * profile.age + 5;
  } else {
    bmr = 10 * profile.weight + 6.25 * profile.height - 5 * profile.age - 161;
  }
  const tdee = Math.round(bmr * 1.4); // lightly active
  if (profile.goal === 'lose') return Math.round(tdee * 0.8);
  if (profile.goal === 'gain') return Math.round(tdee * 1.1);
  return tdee;
}

// ══════════════════════════════════════════
// MQS — Meal Quality Score 0–100
// ══════════════════════════════════════════
function calcMQS(calo, p, c, f) {
  if (calo <= 0) return 50;
  const proteinPct = (p * 4) / calo;
  const carbPct = (c * 4) / calo;
  const fatPct = (f * 9) / calo;
  // Ideal: protein 25–35%, carb 40–55%, fat 20–35%
  const pScore = proteinPct >= 0.25 && proteinPct <= 0.40 ? 35 : Math.max(0, 35 - Math.abs(proteinPct - 0.30) * 200);
  const cScore = carbPct >= 0.40 && carbPct <= 0.55 ? 35 : Math.max(0, 35 - Math.abs(carbPct - 0.48) * 200);
  const fScore = fatPct >= 0.20 && fatPct <= 0.35 ? 30 : Math.max(0, 30 - Math.abs(fatPct - 0.27) * 150);
  return Math.min(100, Math.max(0, Math.round(pScore + cScore + fScore)));
}

function mqsClass(mqs) {
  if (mqs >= 65) return 'mqs-high';
  if (mqs >= 40) return 'mqs-mid';
  return 'mqs-low';
}
function mqsLabel(mqs) {
  if (mqs >= 65) return '👍 Tốt';
  if (mqs >= 40) return '😐 Trung bình';
  return '⚠️ Thấp';
}

// ══════════════════════════════════════════
// FORGIVENESS MESSAGES
// ══════════════════════════════════════════
function getForgivenessMsg(totalCalo, goal, mqsAvg) {
  const over = totalCalo > goal * 1.15;
  const under = totalCalo < goal * 0.6;
  if (over && mqsAvg < 50) return "Hôm nay bạn đã sống đúng nghĩa! 🌟 Ngày mai chọn thêm rau và protein là cân bằng lại rồi. Mỗi ngày là một trang mới.";
  if (over) return "Ăn nhiều hơn hôm nay không sao cả 💚 MQS của bạn vẫn tốt — chứng tỏ bạn chọn đồ ăn lành mạnh. Tiếp tục nhé!";
  if (under) return "Bạn ăn hơi ít hôm nay 🍜 Hãy bổ sung thêm bữa phụ — cơ thể cần đủ năng lượng để hoạt động tốt nhất!";
  if (mqsAvg < 45) return "MQS hôm nay hơi thấp — thêm rau hoặc protein vào bữa tới là lên ngay! 💪 Bạn đang học cách ăn thông minh hơn mỗi ngày.";
  return "Tuyệt vời! 🎯 Hôm nay bạn đang ăn rất khoa học. Cứ giữ đà này nhé!";
}

// ══════════════════════════════════════════
// STREAK LOGIC
// ══════════════════════════════════════════
function updateStreak() {
  const today = getToday();
  const yesterday = new Date(Date.now() - 86400000).toISOString().split('T')[0];
  const last = STATE.lastLogDate;

  if (last === today) return; // already counted today
  if (last === yesterday) {
    STATE.streak += 1;
  } else if (last && last !== yesterday && STATE.streakFreezes > 0) {
    STATE.streakFreezes -= 1;
    STATE.streak += 1;
    showToast("❄️ Streak Freeze đã được dùng! Streak giữ nguyên.");
  } else if (!last) {
    STATE.streak = 1;
  } else {
    STATE.streak = 1; // reset
    showToast("Streak đã reset. Bắt đầu chuỗi mới từ hôm nay! 💪");
  }
  STATE.lastLogDate = today;
  saveState(STATE);
}

function getLevel(streak) {
  if (streak >= 100) return "Huyền thoại 🏆";
  if (streak >= 50) return "Chuyên gia 💎";
  if (streak >= 30) return "Rau trưởng thành 🌿";
  if (streak >= 14) return "Rau xanh 🥦";
  if (streak >= 7)  return "Mầm lớn 🌱";
  return "Mầm xanh 🌱";
}

// ══════════════════════════════════════════
// RENDER FUNCTIONS
// ══════════════════════════════════════════
function renderHome() {
  if (!STATE.profile) return;
  const today = getToday();
  const todayMeals = STATE.weekLog[today] || [];
  const goal = STATE.profile.tdee;

  // Streak
  document.getElementById('streak-num').textContent = STATE.streak;
  document.getElementById('level-badge').textContent = getLevel(STATE.streak);
  document.getElementById('freeze-count').textContent = STATE.streakFreezes;

  // Week dots
  const dots = document.getElementById('week-dots');
  const days = ['T2','T3','T4','T5','T6','T7','CN'];
  const weekDates = [];
  for (let i = 6; i >= 0; i--) {
    const d = new Date(Date.now() - i * 86400000).toISOString().split('T')[0];
    weekDates.push(d);
  }
  dots.innerHTML = weekDates.map((d, i) => {
    const isToday = d === today;
    const hasLog = STATE.weekLog[d] && STATE.weekLog[d].length > 0;
    const cls = isToday ? (hasLog ? 'done today' : 'today') : (hasLog ? 'done' : 'missed');
    return `<div class="week-dot-wrap"><div class="week-dot ${cls}"></div><div class="week-day">${days[i]}</div></div>`;
  }).join('');

  // Totals
  let totalCalo = 0, totalP = 0, totalC = 0, totalF = 0;
  todayMeals.forEach(m => { totalCalo += m.calo; totalP += m.p; totalC += m.c; totalF += m.f; });

  // Ring
  const pct = Math.min(1, totalCalo / goal);
  const circumference = 251;
  const offset = circumference - (pct * circumference);
  document.getElementById('ring-circle').style.strokeDashoffset = offset;
  const ringColor = totalCalo > goal * 1.1 ? '#dc2626' : totalCalo > goal * 0.9 ? '#f59e0b' : '#16a34a';
  document.getElementById('ring-circle').style.stroke = ringColor;
  document.getElementById('ring-ate').textContent = totalCalo;
  document.getElementById('ring-goal').textContent = goal;
  document.getElementById('remaining-calo').textContent = Math.max(0, goal - totalCalo);

  // Macro bars — targets: protein 25%, carbs 50%, fat 25% of TDEE
  const pGoal = Math.round((goal * 0.25) / 4);
  const cGoal = Math.round((goal * 0.50) / 4);
  const fGoal = Math.round((goal * 0.25) / 9);
  document.getElementById('bar-protein').style.width = Math.min(100, Math.round(totalP / pGoal * 100)) + '%';
  document.getElementById('bar-carbs').style.width = Math.min(100, Math.round(totalC / cGoal * 100)) + '%';
  document.getElementById('bar-fat').style.width = Math.min(100, Math.round(totalF / fGoal * 100)) + '%';
  document.getElementById('val-protein').textContent = totalP + 'g';
  document.getElementById('val-carbs').textContent = totalC + 'g';
  document.getElementById('val-fat').textContent = totalF + 'g';

  // Meals list
  const entriesEl = document.getElementById('meal-entries');
  const emptyEl = document.getElementById('empty-log');
  if (todayMeals.length === 0) {
    emptyEl.style.display = 'block';
    entriesEl.innerHTML = '';
  } else {
    emptyEl.style.display = 'none';
    entriesEl.innerHTML = todayMeals.map(m => `
      <div class="meal-entry">
        <div>
          <div class="meal-name">${m.name}</div>
          <div class="meal-time">${m.time}</div>
        </div>
        <div class="meal-right">
          <div class="meal-calo">${m.calo} calo</div>
          <div class="mqs-pill ${mqsClass(m.mqs)}">MQS ${m.mqs}</div>
        </div>
      </div>`).join('');
  }

  // Forgiveness banner
  const banner = document.getElementById('forgive-banner');
  if (todayMeals.length >= 2) {
    const avgMQS = Math.round(todayMeals.reduce((s, m) => s + m.mqs, 0) / todayMeals.length);
    banner.style.display = 'flex';
    document.getElementById('forgive-text').textContent = getForgivenessMsg(totalCalo, goal, avgMQS);
  } else {
    banner.style.display = 'none';
  }
}

function renderStats() {
  const today = getToday();
  const allDates = Object.keys(STATE.weekLog);
  const allMeals = allDates.flatMap(d => STATE.weekLog[d]);

  document.getElementById('stat-streak').textContent = STATE.streak + ' 🔥';
  document.getElementById('stat-total-logs').textContent = STATE.totalLogs;

  if (allMeals.length > 0) {
    const avgCalo = Math.round(allMeals.reduce((s, m) => s + m.calo, 0) / allDates.length);
    const avgMQS = Math.round(allMeals.reduce((s, m) => s + m.mqs, 0) / allMeals.length);
    document.getElementById('stat-avg-calo').textContent = avgCalo;
    document.getElementById('stat-avg-mqs').textContent = avgMQS + '/100';

    // Bio age calculation
    const profile = STATE.profile;
    if (profile && allDates.length >= 3) {
      const goalCalo = profile.tdee;
      const caloDiff = Math.abs(avgCalo - goalCalo) / goalCalo;
      const mqsBonus = (avgMQS - 50) / 50;
      const bioOffset = caloDiff * 4 - mqsBonus * 3;
      const bioAge = Math.round((profile.age + bioOffset) * 10) / 10;
      document.getElementById('bio-age').textContent = bioAge.toFixed(1);
      const diff = (bioAge - profile.age).toFixed(1);
      document.getElementById('bio-note').textContent = diff < 0
        ? `✨ Thấp hơn tuổi thật ${Math.abs(diff)} năm — bạn đang ăn uống tốt hơn hầu hết nhóm tuổi của mình!`
        : diff > 1
        ? `💪 Cao hơn tuổi thật ${diff} năm — hãy cải thiện chất lượng bữa ăn (MQS) và ăn đúng lượng calo hơn.`
        : `✅ Gần bằng tuổi thật — bạn đang đi đúng hướng!`;
    }

    // MQS breakdown
    const high = allMeals.filter(m => m.mqs >= 65).length;
    const mid = allMeals.filter(m => m.mqs >= 40 && m.mqs < 65).length;
    const low = allMeals.filter(m => m.mqs < 40).length;
    const total = allMeals.length;
    document.getElementById('mqs-breakdown').innerHTML = `
      <div style="display:flex;flex-direction:column;gap:10px">
        <div>
          <div style="display:flex;justify-content:space-between;font-size:12px;margin-bottom:4px">
            <span style="color:#15803d">👍 Tốt (MQS ≥ 65)</span><span style="font-weight:600">${high} bữa (${Math.round(high/total*100)}%)</span>
          </div>
          <div style="height:8px;background:var(--gray-100);border-radius:4px"><div style="height:100%;border-radius:4px;background:#16a34a;width:${Math.round(high/total*100)}%;transition:width 0.5s"></div></div>
        </div>
        <div>
          <div style="display:flex;justify-content:space-between;font-size:12px;margin-bottom:4px">
            <span style="color:#92400e">😐 Trung bình (40–64)</span><span style="font-weight:600">${mid} bữa (${Math.round(mid/total*100)}%)</span>
          </div>
          <div style="height:8px;background:var(--gray-100);border-radius:4px"><div style="height:100%;border-radius:4px;background:#d97706;width:${Math.round(mid/total*100)}%;transition:width 0.5s"></div></div>
        </div>
        <div>
          <div style="display:flex;justify-content:space-between;font-size:12px;margin-bottom:4px">
            <span style="color:#991b1b">⚠️ Thấp (< 40)</span><span style="font-weight:600">${low} bữa (${Math.round(low/total*100)}%)</span>
          </div>
          <div style="height:8px;background:var(--gray-100);border-radius:4px"><div style="height:100%;border-radius:4px;background:#dc2626;width:${Math.round(low/total*100)}%;transition:width 0.5s"></div></div>
        </div>
      </div>`;
  }

  // Weekly bar chart
  const chart = document.getElementById('week-chart');
  const goalCalo = STATE.profile ? STATE.profile.tdee : 1800;
  const weekDates = [];
  for (let i = 6; i >= 0; i--) {
    weekDates.push(new Date(Date.now() - i * 86400000).toISOString().split('T')[0]);
  }
  const days = ['T2','T3','T4','T5','T6','T7','CN'];
  const weekCals = weekDates.map(d => (STATE.weekLog[d] || []).reduce((s, m) => s + m.calo, 0));
  const maxCal = Math.max(...weekCals, goalCalo);
  chart.innerHTML = weekDates.map((d, i) => {
    const calo = weekCals[i];
    const h = calo > 0 ? Math.max(8, Math.round((calo / maxCal) * 72)) : 4;
    const color = calo === 0 ? '#e5e7eb' : calo > goalCalo * 1.1 ? '#dc2626' : calo > goalCalo * 0.85 ? '#16a34a' : '#93c5fd';
    return `<div class="bar-col"><div class="bar-body" style="height:${h}px;background:${color}"></div><div class="bar-day">${days[i]}</div></div>`;
  }).join('');
}

// ══════════════════════════════════════════
// LOGGING — add a meal
// ══════════════════════════════════════════
function logMeal(name, calo, p, c, f) {
  const today = getToday();
  const mqs = calcMQS(calo, p, c, f);
  const now = new Date();
  const time = now.toLocaleTimeString('vi', {hour:'2-digit', minute:'2-digit'});
  const entry = {name, calo, p, c, f, mqs, time};

  if (!STATE.weekLog[today]) STATE.weekLog[today] = [];
  STATE.weekLog[today].push(entry);
  STATE.totalLogs += 1;
  updateStreak();
  saveState(STATE);
  renderHome();
  return mqs;
}

function addManualEntry() {
  const name = document.getElementById('manual-name').value.trim() || 'Món ăn';
  const calo = parseInt(document.getElementById('manual-calo').value) || 0;
  const p = parseInt(document.getElementById('manual-protein').value) || 0;
  const c = parseInt(document.getElementById('manual-carbs').value) || 0;
  const f = parseInt(document.getElementById('manual-fat').value) || 0;
  if (calo <= 0) { showToast("Vui lòng nhập số calo!"); return; }
  const mqs = logMeal(name, calo, p, c, f);
  showLogResult([{name, calo, p, c, f, mqs}], "Đã ghi thành công! 🎉");
  document.getElementById('manual-name').value = '';
  document.getElementById('manual-calo').value = '';
  document.getElementById('manual-protein').value = '';
  document.getElementById('manual-carbs').value = '';
  document.getElementById('manual-fat').value = '';
}

// ── Text input analysis (keyword matching, no AI) ──
function analyzeTextInput() {
  const text = document.getElementById('food-text-input').value.trim().toLowerCase();
  if (!text) { showToast("Hãy nhập tên món ăn!"); return; }

  let matched = [];
  // Try to match from our text estimates
  for (const [keyword, data] of Object.entries(TEXT_ESTIMATES)) {
    if (text.includes(keyword)) {
      matched.push({name: keyword.charAt(0).toUpperCase() + keyword.slice(1), ...data, mqs: calcMQS(data.calo, data.p, data.c, data.f)});
    }
  }
  // Also check street food names
  STREET_FOODS.forEach(sf => {
    if (text.includes(sf.name.toLowerCase()) && !matched.find(m => m.name === sf.name)) {
      matched.push({name: sf.name, calo: sf.calo, p: sf.p, c: sf.c, f: sf.f, mqs: calcMQS(sf.calo, sf.p, sf.c, sf.f)});
    }
  });

  if (matched.length === 0) {
    // Default estimate
    matched = [{name: "Bữa ăn ước tính", calo: 450, p: 20, c: 55, f: 14, mqs: 58}];
    showToast("Không nhận ra món — đã ước tính 450 calo");
  }

  // Log all matched items
  matched.forEach(m => logMeal(m.name, m.calo, m.p, m.c, m.f));
  showLogResult(matched, "Đã phân tích và ghi thành công! ✅");
  document.getElementById('food-text-input').value = '';
}

// ── Show result card ──
function showLogResult(meals, headline) {
  const totalCalo = meals.reduce((s, m) => s + m.calo, 0);
  const totalP = meals.reduce((s, m) => s + m.p, 0);
  const totalC = meals.reduce((s, m) => s + m.c, 0);
  const totalF = meals.reduce((s, m) => s + m.f, 0);
  const avgMQS = Math.round(meals.reduce((s, m) => s + m.mqs, 0) / meals.length);
  const mqsColor = avgMQS >= 65 ? '#16a34a' : avgMQS >= 40 ? '#d97706' : '#dc2626';
  const forgivenessMsg = getForgivenessMsg(totalCalo, STATE.profile ? STATE.profile.tdee / 3 : 600, avgMQS);

  const rows = meals.map(m => `<div class="result-row"><span>${m.name}</span><span>${m.calo} calo · MQS <span class="mqs-pill ${mqsClass(m.mqs)}" style="font-size:10px">${m.mqs}</span></span></div>`).join('');

  document.getElementById('log-result').style.display = 'block';
  document.getElementById('log-result').innerHTML = `
    <div class="result-card">
      <div class="result-header">
        <div class="result-title">${headline}</div>
      </div>
      ${rows}
      ${meals.length > 1 ? `<div class="result-total"><span>Tổng calo</span><span>${totalCalo} calo</span></div>` : ''}
      <div class="mqs-score-wrap">
        <div class="mqs-score-label"><span>Meal Quality Score</span><span style="color:${mqsColor};font-weight:700">${avgMQS}/100</span></div>
        <div class="mqs-track"><div class="mqs-fill" style="width:${avgMQS}%;background:${mqsColor}"></div></div>
      </div>
      <div class="forgive-result">💬 ${forgivenessMsg}</div>
      <div style="margin-top:10px;display:flex;gap:8px">
        <div style="flex:1;text-align:center;background:var(--blue-light);border-radius:8px;padding:8px">
          <div style="font-size:16px;font-weight:700;color:var(--blue)">${totalP}g</div>
          <div style="font-size:10px;color:#1d4ed8">Protein</div>
        </div>
        <div style="flex:1;text-align:center;background:var(--amber-light);border-radius:8px;padding:8px">
          <div style="font-size:16px;font-weight:700;color:var(--amber)">${totalC}g</div>
          <div style="font-size:10px;color:#92400e">Carbs</div>
        </div>
        <div style="flex:1;text-align:center;background:var(--red-light);border-radius:8px;padding:8px">
          <div style="font-size:16px;font-weight:700;color:var(--red)">${totalF}g</div>
          <div style="font-size:10px;color:#991b1b">Chất béo</div>
        </div>
      </div>
    </div>
    <button class="btn btn-green" onclick="goHome()">← Về trang chính</button>`;
}

// ══════════════════════════════════════════
// STREET FOOD
// ══════════════════════════════════════════
let sfFiltered = [...STREET_FOODS];

function renderStreetFood(list) {
  const el = document.getElementById('sf-list');
  if (list.length === 0) {
    el.innerHTML = '<div style="text-align:center;color:var(--gray-400);padding:20px;font-size:14px">Không tìm thấy món này</div>';
    return;
  }
  el.innerHTML = list.map((f, i) => `
    <div class="sf-item" onclick="addStreetFood(${STREET_FOODS.indexOf(f)})">
      <div>
        <div class="sf-name">${f.name}</div>
        <div class="sf-meta">${f.cat} · P:${f.p}g C:${f.c}g F:${f.f}g · MQS ${calcMQS(f.calo, f.p, f.c, f.f)}</div>
      </div>
      <span class="sf-calo">${f.calo} calo</span>
      <button class="sf-add-btn" onclick="event.stopPropagation();addStreetFood(${STREET_FOODS.indexOf(f)})">+</button>
    </div>`).join('');
}

function filterStreetFood() {
  const q = document.getElementById('sf-search').value.toLowerCase();
  sfFiltered = q ? STREET_FOODS.filter(f => f.name.toLowerCase().includes(q) || f.cat.toLowerCase().includes(q)) : [...STREET_FOODS];
  renderStreetFood(sfFiltered);
}

function addStreetFood(idx) {
  const f = STREET_FOODS[idx];
  logMeal(f.name, f.calo, f.p, f.c, f.f);
  showLogResult([{name: f.name, calo: f.calo, p: f.p, c: f.c, f: f.f, mqs: calcMQS(f.calo, f.p, f.c, f.f)}], `${f.name} đã được ghi! 🎉`);
}

// ══════════════════════════════════════════
// NAVIGATION
// ══════════════════════════════════════════
function switchTab(tab) {
  ['home','log','stats'].forEach(t => {
    document.getElementById('screen-' + t).classList.remove('active');
    document.getElementById('nav-' + t).classList.remove('active');
  });
  document.getElementById('screen-' + tab).classList.add('active');
  document.getElementById('nav-' + tab).classList.add('active');
  if (tab === 'home') renderHome();
  if (tab === 'stats') renderStats();
  if (tab === 'log') {
    document.getElementById('log-result').style.display = 'none';
    renderStreetFood(STREET_FOODS);
  }
}

function goHome() {
  switchTab('home');
}

function setLogMode(mode, btn) {
  document.querySelectorAll('.mode-tab').forEach(t => t.classList.remove('active'));
  btn.classList.add('active');
  document.querySelectorAll('.log-panel').forEach(p => p.classList.remove('active'));
  document.getElementById('log-' + mode).classList.add('active');
  document.getElementById('log-result').style.display = 'none';
}

// ══════════════════════════════════════════
// ONBOARDING
// ══════════════════════════════════════════
let selectedGoal = 'health';
function selectGoal(btn) {
  document.querySelectorAll('.goal-btn').forEach(b => b.classList.remove('selected'));
  btn.classList.add('selected');
  selectedGoal = btn.dataset.goal;
}

function completeOnboarding() {
  const name = document.getElementById('ob-name').value.trim() || 'Bạn';
  const age = parseInt(document.getElementById('ob-age').value) || 22;
  const gender = document.getElementById('ob-gender').value;
  const weight = parseFloat(document.getElementById('ob-weight').value) || 55;
  const height = parseFloat(document.getElementById('ob-height').value) || 162;
  const profile = {name, age, gender, weight, height, goal: selectedGoal};
  profile.tdee = calcTDEE(profile);
  STATE.profile = profile;
  saveState(STATE);
  // Show main app
  document.getElementById('screen-onboard').classList.remove('active');
  switchTab('home');
  showToast(`Chào ${name}! Mục tiêu calo của bạn: ${profile.tdee} calo/ngày 🎯`);
}

// ══════════════════════════════════════════
// UTILITIES
// ══════════════════════════════════════════
function showToast(msg) {
  const t = document.getElementById('toast');
  t.textContent = msg;
  t.classList.add('show');
  setTimeout(() => t.classList.remove('show'), 3000);
}

function confirmReset() {
  document.getElementById('modal-title').textContent = 'Xoá toàn bộ dữ liệu?';
  document.getElementById('modal-body').textContent = 'Hành động này sẽ xoá tất cả streak, nhật ký bữa ăn và hồ sơ của bạn. Không thể khôi phục.';
  document.getElementById('modal-ok').onclick = function() {
    localStorage.removeItem('calolocal_v1');
    STATE = initState();
    closeModal();
    location.reload();
  };
  document.getElementById('modal-confirm').classList.add('open');
}
function closeModal() {
  document.getElementById('modal-confirm').classList.remove('open');
}
document.getElementById('modal-confirm').addEventListener('click', function(e) {
  if (e.target === this) closeModal();
});

// ══════════════════════════════════════════
// INIT
// ══════════════════════════════════════════
document.getElementById('date-display').textContent = new Date().toLocaleDateString('vi', {weekday:'short', day:'numeric', month:'short'});

// Route to correct screen
if (STATE.profile) {
  document.getElementById('screen-onboard').classList.remove('active');
  switchTab('home');
} else {
  document.getElementById('screen-onboard').classList.add('active');
}
</script>
</body>
</html>
