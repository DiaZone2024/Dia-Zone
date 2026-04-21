<!DOCTYPE html>
<html lang="my">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
  <title>Dia Zone - Login</title>
  
  <script src="https://www.gstatic.com/firebasejs/9.22.1/firebase-app-compat.js"></script>
  <script src="https://www.gstatic.com/firebasejs/9.22.1/firebase-auth-compat.js"></script>
  <script src="https://www.gstatic.com/firebasejs/9.22.1/firebase-database-compat.js"></script>
  <script src="https://telegram.org/js/telegram-web-app.js?62"></script>
  <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,400;14..32,500;14..32,600;14..32,700;14..32,800&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      background: linear-gradient(145deg, #0b0c1a 0%, #11132a 100%);
      font-family: 'Inter', 'Poppins', 'Myanmar Text', sans-serif;
      min-height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 2rem 1rem;
      background-image: url('image/layla.jpg');
      background-size: cover;
      background-position: center;
      background-attachment: fixed;
    }

    .login-card {
      max-width: 520px;
      width: 100%;
      background: rgba(18, 22, 48, 0.85);
      backdrop-filter: blur(12px);
      border-radius: 2rem;
      border: 1px solid rgba(255, 215, 0, 0.25);
      box-shadow: 0 30px 50px rgba(0, 0, 0, 0.5);
      padding: 2rem 2rem 2.5rem;
    }

    h1 {
      font-size: 2rem;
      font-weight: 800;
      background: linear-gradient(120deg, #FFF8E7, #FFE6A3);
      -webkit-background-clip: text;
      background-clip: text;
      color: transparent;
      margin-bottom: 1.5rem;
      text-align: center;
    }

    .input-group {
      margin-bottom: 1.25rem;
    }

    label {
      display: block;
      font-weight: 600;
      font-size: 0.85rem;
      color: #b9c3ff;
      margin-bottom: 0.4rem;
    }

    input {
      width: 100%;
      padding: 0.85rem 1rem;
      border: 1.5px solid rgba(255, 215, 0, 0.3);
      border-radius: 1rem;
      font-size: 0.95rem;
      font-family: inherit;
      background: rgba(10, 12, 28, 0.7);
      color: #f1f5f9;
      transition: all 0.2s;
    }

    input:focus {
      border-color: #FFC857;
      outline: none;
      box-shadow: 0 0 0 3px rgba(255, 200, 87, 0.2);
    }

    input::placeholder {
      color: #6c72a5;
    }

    .btn-primary {
      width: 100%;
      background: linear-gradient(95deg, #FFC857, #FFAE2B);
      color: #12142e;
      font-weight: 800;
      padding: 0.85rem;
      border: none;
      border-radius: 2rem;
      font-size: 1rem;
      cursor: pointer;
      margin-top: 0.5rem;
      font-family: inherit;
      transition: all 0.2s;
    }

    .btn-primary:hover {
      transform: scale(0.98);
      background: linear-gradient(95deg, #FFD46E, #FFB83B);
    }

    .btn-primary:disabled {
      opacity: 0.6;
      cursor: not-allowed;
      transform: none;
    }

    .register-link {
      text-align: center;
      margin-top: 1.5rem;
      font-size: 0.9rem;
      color: #9ba3e0;
    }

    .register-link a {
      color: #FFC857;
      font-weight: 700;
      text-decoration: none;
      cursor: pointer;
    }

    .register-link a:hover {
      text-decoration: underline;
    }

    hr {
      margin: 1.5rem 0;
      border-color: rgba(255, 215, 0, 0.1);
    }

    .error-box {
      background: rgba(255, 70, 70, 0.15);
      border: 1px solid rgba(255, 110, 110, 0.4);
      border-radius: 1rem;
      padding: 0.8rem 1rem;
      margin-top: 1rem;
      font-size: 0.85rem;
      color: #ffaeae;
      display: none;
    }

    .error-box.show {
      display: block;
    }

    small {
      display: block;
      margin-top: 1rem;
      text-align: center;
      color: #6c72a5;
      font-size: 0.7rem;
    }
  </style>
</head>
<body>
<div class="login-card">
  <h1><i class="fas fa-gem"></i> Dia Zone</h1>
  <form id="loginForm">
    <div class="input-group">
      <label><i class="fas fa-envelope"></i> Email</label>
      <input type="email" id="email" placeholder="your@email.com" autocomplete="off">
    </div>
    <div class="input-group">
      <label><i class="fas fa-lock"></i> Password</label>
      <input type="password" id="password" placeholder="Password">
    </div>
    <button type="submit" class="btn-primary" id="loginBtn">Login</button>
  </form>
  <div class="register-link">Don't have an account? <a href="#" id="registerRedirect">Register</a></div>
  <hr>
  <div id="errorMessage" class="error-box"></div>
  <small>Dia Zone • Secure Account</small>
</div>

<script>
  // Firebase Configuration
  const firebaseConfig = {
    apiKey: "AIzaSyCZridqu0bhTRM5mzbRdfJxWic4xcG7rg4",
  authDomain: "dia-zone.firebaseapp.com",
  databaseURL: "https://dia-zone-default-rtdb.asia-southeast1.firebasedatabase.app",
  projectId: "dia-zone",
  storageBucket: "dia-zone.firebasestorage.app",
  messagingSenderId: "954378673786",
  appId: "1:954378673786:web:fe6ab648f60eb5207665c3"
};

  if (!firebase.apps.length) {
    firebase.initializeApp(firebaseConfig);
  }
  const auth = firebase.auth();
  const db = firebase.database();

  const loginForm = document.getElementById('loginForm');
  const errorDiv = document.getElementById('errorMessage');
  const loginBtn = document.getElementById('loginBtn');

  loginForm.addEventListener('submit', async (e) => {
    e.preventDefault();
    const email = document.getElementById('email').value.trim();
    const password = document.getElementById('password').value;

    errorDiv.classList.remove('show');
    
    if (!email || !password) {
      showError('Please enter both email and password');
      return;
    }

    loginBtn.disabled = true;
    loginBtn.innerText = 'Logging in...';

    try {
      const userCredential = await auth.signInWithEmailAndPassword(email, password);
      const user = userCredential.user;
      
      const snapshot = await db.ref('users/' + user.uid).once('value');
      
      if (!snapshot.exists()) {
        showError('User data not found. Please contact support.');
        await auth.signOut();
        return;
      }
      
      const userData = snapshot.val();
      
      if (userData.status === 'Suspended') {
        showError('Your account has been suspended. Please contact admin.');
        await auth.signOut();
        return;
      }
      
      userData.id = user.uid;
      userData.userId = user.uid;
      localStorage.setItem('diaZoneUser', JSON.stringify(userData));
      sessionStorage.setItem('diaZoneUser', JSON.stringify(userData));
      
      window.location.href = 'dashboard.html';
      
    } catch (error) {
      console.error('Login error:', error);
      let errorMsg = 'Invalid email or password';
      if (error.code === 'auth/user-not-found') {
        errorMsg = 'No account found with this email. Please register first.';
      } else if (error.code === 'auth/wrong-password') {
        errorMsg = 'Incorrect password. Please try again.';
      } else if (error.code === 'auth/invalid-email') {
        errorMsg = 'Invalid email format.';
      } else if (error.code === 'auth/too-many-requests') {
        errorMsg = 'Too many failed attempts. Please try again later.';
      }
      showError(errorMsg);
      loginBtn.disabled = false;
      loginBtn.innerText = 'Login';
    }
  });

  function showError(msg) {
    errorDiv.innerHTML = `<i class="fas fa-exclamation-circle"></i> ${msg}`;
    errorDiv.classList.add('show');
    setTimeout(() => {
      if (loginBtn.disabled) {
        loginBtn.disabled = false;
        loginBtn.innerText = 'Login';
      }
    }, 3000);
  }

  document.getElementById('registerRedirect').addEventListener('click', (e) => {
    e.preventDefault();
    window.location.href = 'register.html';
  });
</script>
</body>
</html>
