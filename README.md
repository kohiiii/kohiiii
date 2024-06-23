<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Domande e Risposte</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
            padding: 20px;
        }
        #faq-container {
            max-width: 600px;
            margin: 0 auto;
        }
        .question {
            cursor: pointer;
            padding: 10px;
            background-color: #f2f2f2;
            margin-bottom: 5px;
        }
        .answer {
            display: none;
            padding: 10px;
            background-color: #e0e0e0;
        }
    </style>
</head>
<body>

    <div id="faq-container">
        <div class="question" onclick="toggleAnswer('answer1')">Come posso iniziare?</div>
        <div class="answer" id="answer1">Puoi iniziare creando una nuova pagina HTML e aggiungendo il tuo contenuto. Puoi anche utilizzare un framework come Bootstrap per uno stile più rapido.</div>

        <div class="question" onclick="toggleAnswer('answer2')">Quali sono le migliori pratiche per la progettazione di siti web?</div>
        <div class="answer" id="answer2">Le migliori pratiche includono la progettazione responsive, l'ottimizzazione delle immagini, l'accessibilità e la scelta di colori e font coerenti.</div>

        <!-- Aggiungi altre domande e risposte secondo necessità -->

    </div>

    <script>
        function toggleAnswer(answerId) {
            var answer = document.getElementById(answerId);
            if (answer.style.display === 'block') {
                answer.style.display = 'none';
            } else {
                answer.style.display = 'block';
            }
        }
    </script>

</body>
</html>
