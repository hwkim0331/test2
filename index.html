<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>분리수거 퀴즈</title>
    <style>
        body { font-family: Arial, sans-serif; text-align: center; margin: 20px; }
        #quiz { display: none; }
        #question { font-size: 24px; color: red; }
        #timer { position: absolute; right: 20px; top: 20px; font-size: 20px; color: red; }
        .answer { display: inline-block; width: 200px; height: 60px; margin: 10px; font-size: 18px; border: 2px solid #333; border-radius: 5px; line-height: 60px; cursor: pointer; }
        .correct { background-color: blue; color: white; }
        .wrong { background-color: red; color: white; }
        #result { margin-top: 20px; font-size: 24px; }
        #startButton, #restartButton { font-size: 24px; padding: 10px 20px; cursor: pointer; }
        h1 { font-size: 36px; margin-bottom: 20px; }
    </style>
</head>
<body>

<h1>분리수거 퀴즈</h1>
<button id="startButton">퀴즈 시작하기</button>
<button id="restartButton" style="display:none;">다시하기</button>

<div id="timer">남은 시간: <span id="time">10</span>초</div>
<div id="quiz">
    <h2 id="question"></h2>
    <img id="image" src="" alt="" style="width:300px; height:auto;">
    <div id="answers"></div>
</div>
<div id="result"></div>

<script>
    const questions = [
        {
            question: "양파 껍질은 어디에 분리수거해야할까?",
            image: "https://example.com/onion.jpg", // 양파 껍질 이미지 URL
            answers: [
                { text: "음식물쓰레기", correct: false },
                { text: "일반쓰레기", correct: true },
                { text: "비닐", correct: false },
                { text: "내 입속", correct: false }
            ]
        },
        {
            question: "소주병은 어디에 분리수거해야할까?",
            image: "https://example.com/soju-bottle.jpg", // 소주병 이미지 URL
            answers: [
                { text: "음식물쓰레기", correct: false },
                { text: "유리", correct: true },
                { text: "캔", correct: false },
                { text: "플라스틱", correct: false }
            ]
        },
        {
            question: "영수증은 어디에 분리수거해야할까?",
            image: "https://example.com/receipt.jpg", // 영수증 이미지 URL
            answers: [
                { text: "일반쓰레기", correct: true },
                { text: "종이", correct: false },
                { text: "비닐", correct: false },
                { text: "내 주머니속", correct: false }
            ]
        },
        {
            question: "고추장은 어디에 분리수거해야할까?",
            image: "https://example.com/gochujang.jpg", // 고추장 이미지 URL
            answers: [
                { text: "음식물 쓰레기", correct: false },
                { text: "일반 쓰레기", correct: true },
                { text: "비닐", correct: false },
                { text: "비빔밥 해먹기", correct: false }
            ]
        },
        {
            question: "책은 어디에 분리수거해야할까?",
            image: "https://example.com/book.jpg", // 책 이미지 URL
            answers: [
                { text: "종이", correct: true },
                { text: "일반쓰레기", correct: false },
                { text: "플라스틱", correct: false },
                { text: "종이와 일반쓰레기 둘 다 해당", correct: false }
            ]
        }
    ];

    let selectedQuestions = [];
    let currentQuestionIndex = 0;
    let score = 0;
    let timer;

    document.getElementById('startButton').addEventListener('click', startQuiz);
    document.getElementById('restartButton').addEventListener('click', restartQuiz);

    function startQuiz() {
        selectedQuestions = [];
        while (selectedQuestions.length < 3) {
            const randomIndex = Math.floor(Math.random() * questions.length);
            if (!selectedQuestions.includes(randomIndex)) {
                selectedQuestions.push(randomIndex);
            }
        }
        currentQuestionIndex = 0;
        score = 0;
        document.getElementById('result').innerHTML = '';
        document.getElementById('quiz').style.display = 'block';
        document.getElementById('restartButton').style.display = 'none'; // 다시하기 버튼 숨김
        displayQuestion();
    }

    function displayQuestion() {
        const currentQuestion = questions[selectedQuestions[currentQuestionIndex]];
        document.getElementById('question').innerText = currentQuestion.question;
        document.getElementById('image').src = currentQuestion.image;
        const answersDiv = document.getElementById('answers');
        answersDiv.innerHTML = '';

        currentQuestion.answers.forEach((answer) => {
            const button = document.createElement('div');
            button.className = 'answer';
            button.innerText = answer.text;
            button.addEventListener('click', () => checkAnswer(answer.correct));
            answersDiv.appendChild(button);
        });

        startTimer();
    }

    function startTimer() {
        let timeLeft = 10;
        document.getElementById('time').innerText = timeLeft;
        clearInterval(timer);
        timer = setInterval(() => {
            timeLeft--;
            document.getElementById('time').innerText = timeLeft;
            if (timeLeft <= 0) {
                clearInterval(timer);
                nextQuestion(false); // 시간 초과로 틀린 처리
            }
        }, 1000);
    }

    function checkAnswer(correct) {
        clearInterval(timer);
        nextQuestion(correct);
    }

    function nextQuestion(correct) {
        const answersDiv = document.getElementById('answers');
        if (correct) {
            score += 30; // 맞으면 30점 추가
            answersDiv.innerHTML = '<div class="correct">정답입니다! ✔️</div>';
        } else {
            answersDiv.innerHTML = '<div class="wrong">틀렸습니다! ❌</div>';
        }

        setTimeout(() => {
            currentQuestionIndex++;
            if (currentQuestionIndex < selectedQuestions.length) {
                displayQuestion();
            } else {
                endQuiz();
            }
        }, 2000); // 2초 후 다음 문제로 넘어감
    }

    function endQuiz() {
        document.getElementById('quiz').style.display = 'none';
        const resultText = document.createElement('div');
        resultText.style.fontSize = '36px';

        if (score === 90) {
            resultText.innerHTML = '<span style="color: red;">100점입니다!</span>';
        } else if (score === 60) {
            resultText.innerHTML = '<span style="color: orange;">60점입니다!</span>';
        } else {
            resultText.innerHTML = '<span style="color: blue;">30점입니다!</span>';
        }

        document.getElementById('result').appendChild(resultText);
        document.getElementById('restartButton').style.display = 'block'; // 다시하기 버튼 보이기
    }

    function restartQuiz() {
        document.getElementById('result').innerHTML = ''; // 결과 초기화
        startQuiz(); // 퀴즈 시작 함수 호출
    }
</script>

</body>
</html>
