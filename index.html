<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ตรรกศาสตร์</title>
<style>
  body {
    font-family: Arial, sans-serif;
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-top: 50px;
  }
  #question {
    font-size: 1.5em;
    margin-bottom: 20px;
  }
  #feedback {
    font-size: 1.2em;
    margin-top: 20px;
  }
  button {
    padding: 10px 20px;
    font-size: 1em;
    background-color: #4CAF50;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    transition: transform 0.2s, background-color 0.2s;
    margin-top: 20px;
  }
  button:hover {
    background-color: #45a049;
  }
  button:active {
    transform: scale(0.95);
  }
  .correct {
    color: green;
  }
  .incorrect {
    color: red;
  }
</style>
</head>
<body>
<h1>เกมตอบปัญหาตรรกศาสตร์</h1>
<div id="question">กดปุ่มเพื่อสุ่มโจทย์ตรรกศาสตร์</div>
<button onclick="generateQuestion()">สุ่มโจทย์</button>
<label for="answer">คำตอบของคุณ (จริง/เท็จ):</label>
<input type="text" id="answer">
<button onclick="checkAnswer()">ตรวจคำตอบ</button>
<div id="feedback"></div>
<div id="score">คะแนนของคุณ: <span id="scoreCount">0</span></div>
<script>
  let score = 0;
  const questions = [
    { text: "จงบอกค่าความจริงของประพจน์ พระอาทิตย์ขึ้นทางทิศตะวันออก", answer: "จริง" },
    { text: "pและq เป็น จริง และ เท็จ ตามลำดับ จงหาค่าความจริงของ (∼p∨q)→p", answer: "จริง" },
    { text: "2 เป็นจำนวนคู่ และ 1 เป็นจำนวนคี่", answer: "จริง" },
    { text: "p,qและr เป็น จริง จริง และ เท็จ ตามลำดับ จงหาค่าความจริงของ p∧q↔r", answer: "เท็จ" },
    { text: "จงบอกค่าความจริงของประพจน์ เดือนมกราคม มี 30 วัน", answer: "เท็จ" },
    { text: "pและq เป็น จริง และ เท็จ ตามลำดับ จงหาค่าความจริงของ p∧q", answer: "เท็จ" },
    { text: "pและq เป็น เท็จ และ จริง ตามลำดับ จงหาค่าความจริงของ p∨q", answer: "จริง" },
    { text: "p,qและr เป็น จริง เท็จ และ จริง ตามลำดับ จงหาค่าความจริงของ p∨r→q", answer: "เท็จ" },
    { text: "p,qและr เป็น เท็จ จริง และ เท็จ ตามลำดับ จงหาค่าความจริงของ ~q↔(p∨r)", answer: "จริง" },
    { text: "จงบอกค่าความจริงของประพจน์ ประเทศไทยมี77จังหวัด", answer: "จริง" },
    { text: "pและq เป็น จริง และ จริง ตามลำดับ จงหาค่าความจริงของp↔q", answer: "จริง" },
    { text: "p,qและr เป็น จริง จริง และ เท็จ ตามลำดับ จงหาค่าความจริงของ (p∧q)∨~r", answer: "จริง" },
    { text: "pและq เป็น เท็จ และ เท็จ ตามลำดับ จงหาค่าความจริงของ ~p∧q", answer: "เท็จ" },
    { text: "p,qและr เป็น เท็จ เท็จ และ จริง ตามลำดับ จงหาค่าความจริงของ p∧(q↔r)", answer: "เท็จ" },
    { text: "pและqเ ป็น จริง และ เท็จ ตามลำดับ จงหาค่าความจริงของ p→q", answer: "เท็จ" },
    { text: "p แทน 0 เป็นจำนวนนับ q แทน 6 เป็นจำนวนเต็ม จงหาค่าความจริงของ p∧q", answer: "เท็จ" },
    { text: "p แทน 1+1=2 , q แทน 2+2=4 จงหาค่าความจริงของ p↔q", answer: "จริง" },
    { text: "p,q,rและs เป็น จริง จริง เท็จ และ เท็จ ตามลำดับ จงหาค่าความจริงของ [(p∨s)↔(q∨r)]→p", answer: "จริง" },
    { text: "p,qและr เป็น จริง จริง และ จริง ตามลำดับ จงหาค่าความจริงของ ~p∨(q→r)", answer: "จริง" },
    { text: "pและq เป็น เท็จ และ จริง ตามลำดับ จงหาค่าความจริงของ ~q→p", answer: "จริง" },
    { text: "p,qและr เป็น จริง เท็จ และ จริง ตามลำดับ จงหาค่าความจริงของ p∧(~q∨r)", answer: "จริง" },
    { text: "p,qและr เป็น เท็จ จริง และ เท็จ ตามลำดับ จงหาค่าความจริงของ (p→q)↔~r", answer: "จริง" },
    { text: "pและq เป็น เท็จ และ เท็จ ตามลำดับ จงหาค่าความจริงของ p↔~q", answer: "เท็จ" },
    { text: "pและq เป็น จริง และ จริง ตามลำดับ จงหาค่าความจริงของ ~(p∧q)", answer: "เท็จ" },
    { text: "pและq เป็น จริง และ เท็จ ตามลำดับ จงหาค่าความจริงของ ~(p∨q)", answer: "เท็จ" },
    { text: "p,qและr เป็น เท็จ จริง และ จริง ตามลำดับ จงหาค่าความจริงของ (p→r)∧q", answer: "จริง" },
    { text: "pและq เป็น เท็จ และ จริง ตามลำดับ จงหาค่าความจริงของ (p→q)∧~q", answer: "เท็จ" },
    { text: "p,qและr เป็น จริง เท็จ และ เท็จ ตามลำดับ จงหาค่าความจริงของ ~(p∨r)↔q", answer: "จริง" },
    { text: "p,qและr เป็น เท็จ จริง และ จริง ตามลำดับ จงหาค่าความจริงของ (q∧r)→p", answer: "เท็จ" },
    { text: "pและq เป็น เท็จ และ เท็จ ตามลำดับ จงหาค่าความจริงของ (p∧q)∨~p", answer: "จริง" },
    { text: "p,qและr เป็น จริง จริง และ เท็จ ตามลำดับ จงหาค่าความจริงของ ~q→(p↔r)", answer: "จริง" },
  ];

  let currentQuestion = null;

  function updateScore(isCorrect) {
    if (isCorrect) {
      score++;
    } else {
      score--;
    }
    document.getElementById("scoreCount").textContent = score;
  }

  function generateQuestion() {
    const randomIndex = Math.floor(Math.random() * questions.length);
    currentQuestion = questions[randomIndex];
    document.getElementById("question").textContent = currentQuestion.text;
    document.getElementById("feedback").textContent = "";
    document.getElementById("answer").value = "";
  }

  function checkAnswer() {
    const userAnswer = document.getElementById("answer").value.trim();
    const feedback = document.getElementById("feedback");
    if (currentQuestion) {
      if (userAnswer === currentQuestion.answer) {
        feedback.textContent = "คำตอบถูกต้อง!";
        feedback.className = "correct";
        updateScore(true);
      } else {
        feedback.textContent = "คำตอบไม่ถูกต้อง ลองใหม่อีกครั้ง!";
        feedback.className = "incorrect";
        updateScore(false);
      }
    } else {
      feedback.textContent = "กรุณาสุ่มโจทย์ก่อน";
      feedback.className = "incorrect";
    }
  }
</script>
</body>
</html>