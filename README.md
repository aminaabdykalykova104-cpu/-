<!DOCTYPE html>
<html lang="kk">
<head>
<meta charset="UTF-8">
<title>Керей мен Жәнібек</title>
<style>
body {
    font-family: Arial, sans-serif;
    text-align: center;
    background-color: #eaf2ff;
}
button {
    margin: 6px;
    padding: 10px 16px;
    background: #2563eb;
    color: white;
    border: none;
    border-radius: 8px;
    cursor: pointer;
}
button:hover {
    background: #1d4ed8;
}
#info {
    margin-top: 15px;
    font-size: 17px;
}
img {
    width: 260px;
    margin-top: 15px;
    border-radius: 10px;
}
</style>
</head>
<body>

<h2>Керей мен Жәнібек</h2>
<p><b>Қазақ хандығының негізін қалаушылар</b></p>

<button onclick="bio()">Кімдер?</button>
<button onclick="facts()">Фактілер</button>
<button onclick="quote()">Сөз</button>
<button onclick="quiz()">Тест</button>
<button onclick="color()">Фон</button>

<div id="info"></div>
<img src="https://share.google/images/v8MaxpB3AYJdkvTWn" alt="Керей мен Жәнібек">

<script>
function bio() {
    document.getElementById("info").innerHTML =
        "<b>Керей мен Жәнібек</b> — XV ғасырда Қазақ хандығын құрған алғашқы хандар. 1465 жылы Шу мен Талас бойында хандық құрды.";
}

function facts() {
    document.getElementById("info").innerHTML =
        "<ul style='text-align:left; display:inline-block'>" +
        "<li>Керей — алғашқы қазақ ханы.</li>" +
        "<li>Жәнібек — оның серігі.</li>" +
        "<li>Қазақ хандығы 1465 жылы құрылды.</li>" +
        "</ul>";
}

function quote() {
    const q = [
        "Бірлік бар жерде — тірлік бар.",
        "Тәуелсіздік — халықтың рухы.",
        "Өткенін білмегеннің — болашағы бұлыңғыр."
    ];
    document.getElementById("info").innerHTML = "<i>" + q[Math.floor(Math.random() * q.lengt
