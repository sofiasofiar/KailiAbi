<!DOCTYPE html>
<html lang="et">
<head>
  <meta charset="UTF-8">
  <title>Sõna abi</title>
</head>
<body>

<h2>Sõna kontroll ja sünonüümid</h2>

<input id="word" placeholder="Sisesta sõna..." />
<button onclick="checkWord()">Kontrolli</button>

<div id="result"></div>

<script>
function checkWord() {
  const word = document.getElementById("word").value;
  const resultDiv = document.getElementById("result");

  resultDiv.innerHTML = "";

  if (word.length < 2) {
    resultDiv.innerHTML = "Liiga lühike sõna";
    return;
  }

  resultDiv.innerHTML = `<b>${word}</b> võib olla sõna`;

  const synonyms = {
    "hea": ["tore", "kena", "meeldiv"],
    "halb": ["kehv", "vilets"]
  };

  if (synonyms[word]) {
    resultDiv.innerHTML += "<br><br>Sünonüümid: " + synonyms[word].join(", ");
  } else {
    resultDiv.innerHTML += "<br><br>Sünonüüme ei leitud";
  }
}
</script>

</body>
</html>
