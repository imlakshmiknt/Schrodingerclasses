<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8"/>
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Login — Schrödinger Classes</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link href="https://fonts.googleapis.com/css2?family=DM+Serif+Display:ital@0;1&family=DM+Sans:wght@300;400;500;600&family=JetBrains+Mono:wght@400;600&display=swap" rel="stylesheet">
  <style>
    *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
    :root {
      --black: #0a0a0a; --white: #f8f7f4; --cream: #f0ede6;
      --ink: #1a1a1a; --muted: #6b6b6b; --accent: #1a3a5c;
      --accent2: #c8a96e; --border: #e0ddd6;
      --serif: 'DM Serif Display', serif;
      --sans: 'DM Sans', sans-serif;
      --mono: 'JetBrains Mono', monospace;
      --error: #c0392b; --success: #27ae60;
    }
    body {
      background: var(--cream);
      font-family: var(--sans);
      font-weight: 300;
      min-height: 100vh;
      display: grid;
      grid-template-columns: 1fr 1fr;
    }
    /* Left panel */
    .left-panel {
      background: var(--accent);
      padding: 4rem;
      display: flex; flex-direction: column; justify-content: center;
      position: relative; overflow: hidden;
    }
    .left-panel::before {
      content: 'Ψ';
      position: absolute; right: -3rem; bottom: -3rem;
      font-family: var(--serif); font-size: 22rem;
      color: rgba(255,255,255,0.04);
      line-height: 1; pointer-events: none;
    }
    .panel-logo {
      font-family: var(--serif); font-size: 1.6rem;
      color: var(--white); text-decoration: none;
      margin-bottom: 4rem; display: block;
    }
    .panel-logo span { color: var(--accent2); }
    .panel-title {
      font-family: var(--serif); font-size: 2.5rem;
      color: var(--white); line-height: 1.2;
      margin-bottom: 1rem;
    }
    .panel-sub { color: rgba(255,255,255,0.55); font-size: 0.9rem; line-height: 1.7; }
    .panel-features { margin-top: 3rem; display: flex; flex-direction: column; gap: 1rem; }
    .panel-feat {
      display: flex; align-items: center; gap: 0.8rem;
      color: rgba(255,255,255,0.7); font-size: 0.875rem;
    }
    .feat-dot {
      width: 8px; height: 8px;
      background: var(--accent2); border-radius: 50%; flex-shrink: 0;
    }

    /* Right panel — form */
    .right-panel {
      display: flex; flex-direction: column; justify-content: center; align-items: center;
      padding: 4rem 3rem;
    }
    .form-box {
      width: 100%; max-width: 420px;
    }
    .tabs {
      display: flex; gap: 0; margin-bottom: 2.5rem;
      border-bottom: 2px solid var(--border);
    }
    .tab-btn {
      flex: 1; padding: 0.8rem; background: none; border: none;
      font-family: var(--sans); font-size: 0.875rem; font-weight: 500;
      color: var(--muted); cursor: pointer;
      border-bottom: 2px solid transparent; margin-bottom: -2px;
      transition: all 0.2s;
    }
    .tab-btn.active { color: var(--accent); border-bottom-color: var(--accent); font-weight: 600; }
    .form-title {
      font-family: var(--serif); font-size: 1.8rem;
      color: var(--ink); margin-bottom: 0.4rem;
    }
    .form-sub { font-size: 0.83rem; color: var(--muted); margin-bottom: 2rem; }

    .form-group { margin-bottom: 1.3rem; }
    .form-group label {
      display: block; font-size: 0.78rem; font-weight: 500;
      letter-spacing: 0.06em; text-transform: uppercase;
      color: var(--muted); margin-bottom: 0.5rem;
    }
    .form-group input {
      width: 100%; padding: 0.8rem 1rem;
      background: var(--white); border: 1.5px solid var(--border);
      border-radius: 3px; font-family: var(--sans); font-size: 0.9rem;
      color: var(--ink); outline: none;
      transition: border-color 0.2s;
    }
    .form-group input:focus { border-color: var(--accent); }
    .form-group input::placeholder { color: rgba(107,107,107,0.5); }

    .btn-full {
      width: 100%; padding: 0.9rem;
      background: var(--accent); color: var(--white);
      border: none; border-radius: 3px;
      font-family: var(--sans); font-size: 0.9rem; font-weight: 600;
      cursor: pointer; transition: background 0.2s;
      margin-top: 0.5rem;
    }
    .btn-full:hover { background: var(--accent2); color: var(--ink); }
    .btn-full:disabled { opacity: 0.5; cursor: not-allowed; }

    .divider {
      display: flex; align-items: center; gap: 1rem;
      margin: 1.5rem 0; color: var(--muted); font-size: 0.8rem;
    }
    .divider::before, .divider::after {
      content: ''; flex: 1; height: 1px; background: var(--border);
    }

    .btn-google {
      width: 100%; padding: 0.9rem;
      background: var(--white); color: var(--ink);
      border: 1.5px solid var(--border); border-radius: 3px;
      font-family: var(--sans); font-size: 0.9rem; font-weight: 500;
      cursor: pointer; transition: border-color 0.2s;
      display: flex; align-items: center; justify-content: center; gap: 0.7rem;
    }
    .btn-google:hover { border-color: var(--accent); }

    .msg {
      padding: 0.7rem 1rem; border-radius: 3px;
      font-size: 0.83rem; margin-top: 1rem; display: none;
    }
    .msg.error { background: rgba(192,57,43,0.08); color: var(--error); border: 1px solid rgba(192,57,43,0.2); display: block; }
    .msg.success { background: rgba(39,174,96,0.08); color: var(--success); border: 1px solid rgba(39,174,96,0.2); display: block; }

    .form-section { display: none; }
    .form-section.active { display: block; }

    /* Dashboard (shown after login) */
    .dashboard { display: none; }
    .dash-header {
      background: var(--accent); color: var(--white);
      padding: 1.5rem 2rem;
      display: flex; justify-content: space-between; align-items: center;
    }
    .dash-header h2 { font-family: var(--serif); }
    .dash-grid {
      display: grid; grid-template-columns: repeat(3,1fr); gap: 1.5rem;
      padding: 2rem;
    }
    .dash-card {
      background: var(--white); border: 1px solid var(--border);
      border-radius: 4px; padding: 1.5rem; text-decoration: none; color: inherit;
      transition: transform 0.2s;
    }
    .dash-card:hover { transform: translateY(-2px); }
    .dash-icon { font-size: 2rem; margin-bottom: 0.8rem; }
    .dash-card h4 { font-family: var(--serif); margin-bottom: 0.3rem; }
    .dash-card p { font-size: 0.8rem; color: var(--muted); }
    .sign-out-btn {
      background: rgba(255,255,255,0.15); color: var(--white);
      border: 1px solid rgba(255,255,255,0.3); padding: 0.5rem 1.2rem;
      border-radius: 3px; cursor: pointer; font-family: var(--sans); font-size: 0.85rem;
    }

    @media (max-width: 800px) {
      body { grid-template-columns: 1fr; }
      .left-panel { display: none; }
      .right-panel { padding: 3rem 1.5rem; }
    }
  </style>
</head>
<body>

<!-- LEFT PANEL -->
<div class="left-panel">
  <a href="index.html" class="panel-logo">Schrödinger<span>Classes</span></a>
  <div class="panel-title">Your Physics<br>Journey Starts<br>Here.</div>
  <p class="panel-sub">Create a free account to access notes, quizzes, mock tests, and track your progress.</p>
  <div class="panel-features">
    <div class="panel-feat"><div class="feat-dot"></div>Full access to Class 11 & 12 notes</div>
    <div class="panel-feat"><div class="feat-dot"></div>JEE & NEET mock tests</div>
    <div class="panel-feat"><div class="feat-dot"></div>Quiz score history & analytics</div>
    <div class="panel-feat"><div class="feat-dot"></div>Interactive physics simulations</div>
    <div class="panel-feat"><div class="feat-dot"></div>100% free — always</div>
  </div>
</div>

<!-- RIGHT PANEL -->
<div class="right-panel">
  <!-- Login/Register Form -->
  <div class="form-box" id="formBox">
    <div class="tabs">
      <button class="tab-btn active" onclick="switchTab('login')">Sign In</button>
      <button class="tab-btn" onclick="switchTab('register')">Register</button>
    </div>

    <!-- LOGIN -->
    <div class="form-section active" id="loginSection">
      <div class="form-title">Welcome back.</div>
      <div class="form-sub">Sign in to your student account.</div>
      <div class="form-group">
        <label>Email Address</label>
        <input type="email" id="loginEmail" placeholder="you@example.com"/>
      </div>
      <div class="form-group">
        <label>Password</label>
        <input type="password" id="loginPass" placeholder="••••••••"/>
      </div>
      <button class="btn-full" id="loginBtn" onclick="doLogin()">Sign In →</button>
      <div class="divider">or</div>
      <button class="btn-google" onclick="doGoogle()">
        <svg width="18" height="18" viewBox="0 0 48 48"><path fill="#4285F4" d="M44.5 20H24v8.5h11.8C34.7 33.9 29.9 37 24 37c-7.2 0-13-5.8-13-13s5.8-13 13-13c3.1 0 5.9 1.1 8.1 2.9l6.4-6.4C34.6 4.1 29.6 2 24 2 11.8 2 2 11.8 2 24s9.8 22 22 22c11 0 21-8 21-22 0-1.3-.2-2.7-.5-4z"/></svg>
        Continue with Google
      </button>
      <div id="loginMsg" class="msg"></div>
    </div>

    <!-- REGISTER -->
    <div class="form-section" id="registerSection">
      <div class="form-title">Join for free.</div>
      <div class="form-sub">Create your student account today.</div>
      <div class="form-group">
        <label>Full Name</label>
        <input type="text" id="regName" placeholder="Your Name"/>
      </div>
      <div class="form-group">
        <label>Email Address</label>
        <input type="email" id="regEmail" placeholder="you@example.com"/>
      </div>
      <div class="form-group">
        <label>Password</label>
        <input type="password" id="regPass" placeholder="Min. 6 characters"/>
      </div>
      <button class="btn-full" id="regBtn" onclick="doRegister()">Create Account →</button>
      <div class="divider">or</div>
      <button class="btn-google" onclick="doGoogle()">
        <svg width="18" height="18" viewBox="0 0 48 48"><path fill="#4285F4" d="M44.5 20H24v8.5h11.8C34.7 33.9 29.9 37 24 37c-7.2 0-13-5.8-13-13s5.8-13 13-13c3.1 0 5.9 1.1 8.1 2.9l6.4-6.4C34.6 4.1 29.6 2 24 2 11.8 2 2 11.8 2 24s9.8 22 22 22c11 0 21-8 21-22 0-1.3-.2-2.7-.5-4z"/></svg>
        Continue with Google
      </button>
      <div id="regMsg" class="msg"></div>
    </div>
  </div>

  <!-- DASHBOARD (shown after login) -->
  <div class="dashboard" id="dashboard" style="width:100%;max-width:600px;">
    <div class="dash-header">
      <h2>Welcome, <span id="dashName">Student</span>! 👋</h2>
      <button class="sign-out-btn" onclick="doSignOut()">Sign Out</button>
    </div>
    <div class="dash-grid">
      <a href="notes.html" class="dash-card">
        <div class="dash-icon">📄</div>
        <h4>My Notes</h4>
        <p>Access all chapter notes</p>
      </a>
      <a href="videos.html" class="dash-card">
        <div class="dash-icon">🎬</div>
        <h4>Video Lectures</h4>
        <p>Watch all physics lectures</p>
      </a>
      <a href="quiz.html" class="dash-card">
        <div class="dash-icon">⚡</div>
        <h4>Practice Quiz</h4>
        <p>Test your concepts</p>
      </a>
      <a href="test.html" class="dash-card">
        <div class="dash-icon">📝</div>
        <h4>Mock Tests</h4>
        <p>JEE / NEET pattern tests</p>
      </a>
      <a href="simulation.html" class="dash-card">
        <div class="dash-icon">🔬</div>
        <h4>Simulations</h4>
        <p>Interactive physics lab</p>
      </a>
      <a href="index.html" class="dash-card">
        <div class="dash-icon">🏠</div>
        <h4>Home</h4>
        <p>Back to homepage</p>
      </a>
    </div>
  </div>
</div>

<!-- Firebase SDK -->
<script type="module">
  import { initializeApp } from "https://www.gstatic.com/firebasejs/10.12.0/firebase-app.js";
  import {
    getAuth, createUserWithEmailAndPassword,
    signInWithEmailAndPassword, signOut,
    GoogleAuthProvider, signInWithPopup,
    onAuthStateChanged, updateProfile
  } from "https://www.gstatic.com/firebasejs/10.12.0/firebase-auth.js";

  // ══════════════════════════════════════════════════
  // 🔧 REPLACE THESE WITH YOUR FIREBASE PROJECT CONFIG
  // Go to: https://console.firebase.google.com
  // Create project → Add web app → Copy config below
  // ══════════════════════════════════════════════════
  const firebaseConfig = {
    apiKey: "AIzaSyDEoABDJODhTt5_QAno68Z3pvc21mwG4Dg",
    authDomain: "schrodinger-classes.firebaseapp.com",
    projectId: "schrodinger-classes",
    storageBucket: "schrodinger-classes.firebasestorage.app",
    messagingSenderId: "753861944994",
    appId: "1:753861944994:web:58b3aaf2eca87f4a7dd9fb",
    measurementId: "G-WDKERR27WW"
  };

  const app = initializeApp(firebaseConfig);
  const auth = getAuth(app);
  const provider = new GoogleAuthProvider();

  function showDash(user) {
    document.getElementById('formBox').style.display = 'none';
    document.getElementById('dashboard').style.display = 'block';
    document.getElementById('dashName').textContent =
      user.displayName ? user.displayName.split(' ')[0] : user.email.split('@')[0];
  }
  function showForm() {
    document.getElementById('formBox').style.display = 'block';
    document.getElementById('dashboard').style.display = 'none';
  }

  onAuthStateChanged(auth, user => { if (user) showDash(user); else showForm(); });

  window.switchTab = (tab) => {
    document.querySelectorAll('.tab-btn').forEach((b,i) =>
      b.classList.toggle('active', (tab==='login'?i===0:i===1)));
    document.getElementById('loginSection').classList.toggle('active', tab==='login');
    document.getElementById('registerSection').classList.toggle('active', tab==='register');
  };

  window.doLogin = async () => {
    const email = document.getElementById('loginEmail').value.trim();
    const pass  = document.getElementById('loginPass').value;
    const msg   = document.getElementById('loginMsg');
    const btn   = document.getElementById('loginBtn');
    if (!email || !pass) { showMsg(msg,'error','Please fill all fields.'); return; }
    btn.disabled = true; btn.textContent = 'Signing in…';
    try {
      await signInWithEmailAndPassword(auth, email, pass);
    } catch(e) {
      showMsg(msg,'error', friendlyError(e.code));
      btn.disabled=false; btn.textContent='Sign In →';
    }
  };

  window.doRegister = async () => {
    const name  = document.getElementById('regName').value.trim();
    const email = document.getElementById('regEmail').value.trim();
    const pass  = document.getElementById('regPass').value;
    const msg   = document.getElementById('regMsg');
    const btn   = document.getElementById('regBtn');
    if (!name||!email||!pass) { showMsg(msg,'error','Please fill all fields.'); return; }
    if (pass.length < 6) { showMsg(msg,'error','Password must be at least 6 characters.'); return; }
    btn.disabled=true; btn.textContent='Creating account…';
    try {
      const cred = await createUserWithEmailAndPassword(auth, email, pass);
      await updateProfile(cred.user, { displayName: name });
    } catch(e) {
      showMsg(msg,'error', friendlyError(e.code));
      btn.disabled=false; btn.textContent='Create Account →';
    }
  };

  window.doGoogle = async () => {
    try { await signInWithPopup(auth, provider); }
    catch(e) { console.error(e); }
  };

  window.doSignOut = async () => { await signOut(auth); };

  function showMsg(el, type, text) {
    el.className='msg '+type; el.textContent=text; el.style.display='block';
  }
  function friendlyError(code) {
    const map = {
      'auth/user-not-found': 'No account found with this email.',
      'auth/wrong-password': 'Incorrect password. Try again.',
      'auth/email-already-in-use': 'This email is already registered. Sign in instead.',
      'auth/invalid-email': 'Please enter a valid email address.',
      'auth/weak-password': 'Password is too weak.',
      'auth/too-many-requests': 'Too many attempts. Please try again later.',
      'auth/configuration-not-found': '⚠️ Firebase not configured yet. See setup instructions.'
    };
    return map[code] || 'Something went wrong. Please try again.';
  }
</script>
</body>
</html>
