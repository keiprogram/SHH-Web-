<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>暗記学習アプリ</title>
  <style>
    body {
      font-family: sans-serif;
      background: #f0f4f8;
      color: #333;
      margin: 0;
      padding: 20px;
    }
    .card {
      background: white;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
      max-width: 500px;
      margin: auto;
      text-align: center;
    }
    .word {
      font-size: 24px;
      margin-bottom: 20px;
    }
    button {
      margin: 10px;
      padding: 10px 20px;
      font-size: 16px;
      border-radius: 5px;
      border: none;
      cursor: pointer;
    }
    .correct { background: #4caf50; color: white; }
    .wrong { background: #f44336; color: white; }
    .log, .chat {
      margin-top: 30px;
      max-width: 500px;
      margin-left: auto;
      margin-right: auto;
    }
    .chat textarea {
      width: 100%;
      height: 60px;
      padding: 10px;
    }
    .chat-messages {
      background: #e0f7fa;
      padding: 10px;
      margin-top: 10px;
      min-height: 50px;
      border-radius: 5px;
    }
  </style>
</head>
<body>

<div class="card">
  <div class="word" id="word">Loading...</div>
  <button class="correct" onclick="recordResult(true)">正解！</button>
  <button class="wrong" onclick="recordResult(false)">不正解</button>
</div>

<div class="log">
  <h3>学習ログ</h3>
  <ul id="logList"></ul>
</div>

<div class="chat">
  <h3>みんなのコメント（簡易チャット）</h3>
  <textarea id="chatInput" placeholder="コメントを書いてください…"></textarea><br/>
  <button onclick="addChat()">送信</button>
  <div class="chat-messages" id="chatMessages"></div>
</div>

<script>
const words = [
  { question: "apple", answer: "りんご" },
  { question: "blue", answer: "青" },
  { question: "sun", answer: "太陽" },
  { question: "moon", answer: "月" },
];

let currentIndex = 0;

function showWord() {
  const wordElem = document.getElementById("word");
  if (currentIndex < words.length) {
    wordElem.textContent = `${words[currentIndex].question}（意味は？）`;
  } else {
    wordElem.textContent = "終了しました！お疲れさま！";
  }
}

function recordResult(correct) {
  if (currentIndex >= words.length) return;

  const word = words[currentIndex].question;
  const result = correct ? "○" : "×";
  const log = `${new Date().toLocaleTimeString()} - ${word} : ${result}`;
  
  // 保存と表示
  let logs = JSON.parse(localStorage.getItem("logs") || "[]");
  logs.push(log);
  localStorage.setItem("logs", JSON.stringify(logs));
  displayLogs();

  currentIndex++;
  showWord();
}

function displayLogs() {
  const logList = document.getElementById("logList");
  const logs = JSON.parse(localStorage.getItem("logs") || "[]");
  logList.innerHTML = logs.map(log => `<li>${log}</li>`).join("");
}

function addChat() {
  const input = document.getElementById("chatInput");
  const msg = input.value.trim();
  if (!msg) return;

  let chats = JSON.parse(localStorage.getItem("chats") || "[]");
  chats.push({ text: msg, time: new Date().toLocaleTimeString() });
  localStorage.setItem("chats", JSON.stringify(chats));
  input.value = "";
  displayChat();
}

function displayChat() {
  const msgBox = document.getElementById("chatMessages");
  const chats = JSON.parse(localStorage.getItem("chats") || "[]");
  msgBox.innerHTML = chats.map(c => `<div>🗨️ ${c.time}：${c.text}</div>`).join("");
}

window.onload = () => {
  showWord();
  displayLogs();
  displayChat();
};
</script>

</body>
</html>
