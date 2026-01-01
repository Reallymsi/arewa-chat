<!DOCTYPE html>
<html lang="ha">
<head>
<meta charset="UTF-8">
<title>Arewa Chat</title>

<style>
body{
  font-family: Arial, sans-serif;
  background:#f2f2f2;
  padding:15px;
}
h2,h3{text-align:center}
input,button{
  width:100%;
  padding:10px;
  margin:5px 0;
}
#chat{display:none}
#messages div{
  background:#fff;
  margin:5px 0;
  padding:8px;
  border-radius:5px;
}
</style>
</head>

<body>

<h2>Arewa Chat</h2>

<div id="login">
  <input id="username" placeholder="Username (sunan da ake gani)">
  <input id="email" placeholder="Email">
  <input id="password" type="password" placeholder="Password">
  <button onclick="login()">Shiga / Register</button>
</div>

<div id="chat">
  <h3>Public Group</h3>
  <div id="messages"></div>
  <input id="msg" placeholder="Rubuta sako...">
  <button onclick="send()">Tura</button>
</div>

<script type="module">
import { initializeApp } from "https://www.gstatic.com/firebasejs/9.23.0/firebase-app.js";
import { getAuth, onAuthStateChanged,
signInWithEmailAndPassword,
createUserWithEmailAndPassword } 
from "https://www.gstatic.com/firebasejs/9.23.0/firebase-auth.js";

import { getDatabase, ref, set, push, onChildAdded }
from "https://www.gstatic.com/firebasejs/9.23.0/firebase-database.js";

const firebaseConfig = {
  // Import the functions you need from the SDKs you need
import { initializeApp } from "firebase/app";
import { getAnalytics } from "firebase/analytics";
// TODO: Add SDKs for Firebase products that you want to use
// https://firebase.google.com/docs/web/setup#available-libraries

// Your web app's Firebase configuration
// For Firebase JS SDK v7.20.0 and later, measurementId is optional
const firebaseConfig = {
  apiKey: "AIzaSyCQfNybkBGJ4ULqkfJLYtsrzoUkWpLne1Y",
  authDomain: "arewa-chat-2e5c7.firebaseapp.com",
  projectId: "arewa-chat-2e5c7",
  storageBucket: "arewa-chat-2e5c7.firebasestorage.app",
  messagingSenderId: "980052769046",
  appId: "1:980052769046:web:e1ce6f72577bf3a8db7837",
  measurementId: "G-VTQ04C5H37"
};

// Initialize Firebase
const app = initializeApp(firebaseConfig);
const analytics = getAnalytics(app);

const app = initializeApp(firebaseConfig);
const auth = getAuth(app);
const db = getDatabase(app);

window.login = async () => {
  const u = username.value.trim();
  const e = email.value.trim();
  const p = password.value;

  if(!u||!e||!p){alert("Cika dukkan bayanai");return;}

  try{
    const res = await signInWithEmailAndPassword(auth,e,p);
    await set(ref(db,"users/"+res.user.uid),{username:u});
  }catch{
    const res = await createUserWithEmailAndPassword(auth,e,p);
    await set(ref(db,"users/"+res.user.uid),{username:u});
  }
};

let myUID="";
onAuthStateChanged(auth,user=>{
  if(user){
    myUID=user.uid;
    login.style.display="none";
    chat.style.display="block";
  }
});

window.send = ()=>{
  if(!msg.value)return;
  push(ref(db,"public"),{
    text:msg.value,
    uid:myUID,
    time:Date.now()
  });
  msg.value="";
};

onChildAdded(ref(db,"public"),snap=>{
  const d=snap.val();
  const div=document.createElement("div");
  div.textContent=d.text;
  messages.appendChild(div);
});
</script>

</body>
</html>
