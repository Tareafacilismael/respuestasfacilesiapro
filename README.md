# respuestasfacilesiapro
Este repositorio genera respuestas inteligentes con ia  claras y sencillas.
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Preguntas y Respuestas para Secundaria</title>
  <style>
    body { font-family: Arial, sans-serif; background: #f5f7fa; padding: 2em; }
    #container { max-width: 420px; margin: auto; background: white; border-radius: 10px; box-shadow: 0 2px 8px rgba(0,0,0,0.1); padding: 2em; }
    input, button, textarea { font-size: 1em; width: 100%; margin: 1em 0; padding: 0.5em; border-radius: 5px; border: 1px solid #ccc; }
    button { background: #4CAF50; color: white; border: none; cursor: pointer; }
    button:hover { background: #45a049; }
    #answer { margin-top: 1em; font-size: 1.1em; background: #eaf7e1; padding: 1em; border-radius: 5px; }
  </style>
</head>
<body>
  <div id="container">
    <h2>Haz tu pregunta</h2>
    <textarea id="question" rows="3" placeholder="Escribe tu pregunta aquí..."></textarea>
    <button onclick="answerQuestion()">Responder</button>
    <div id="answer"></div>
  </div>
  <script>
    function answerQuestion() {
      const question = document.getElementById('question').value.toLowerCase();
      let answer = "¡Pregunta interesante! Aunque es difícil, aquí tienes una explicación sencilla: ";

      // Respuestas fáciles para ejemplos comunes
      if (question.includes("agua")) {
        answer = "El agua es un líquido transparente que forma ríos, lagos y mares. Es fundamental para la vida.";
      } else if (question.includes("multiplicación")) {
        answer = "La multiplicación es una operación matemática que consiste en sumar un número varias veces. Por ejemplo, 3 x 4 = 12.";
      } else if (question.includes("planeta")) {
        answer = "Un planeta es un cuerpo celeste que gira alrededor de una estrella, como la Tierra alrededor del Sol.";
      } else if (question.includes("fracción")) {
        answer = "Una fracción representa una parte de un todo. Por ejemplo, 1/2 significa una mitad.";
      } else if (question.includes("historia")) {
        answer = "La historia es la ciencia que estudia los hechos del pasado y nos ayuda a entender el presente.";
      } else if (question.includes("adn")) {
        answer = "El ADN es una molécula que contiene la información genética de los seres vivos. Es como el manual de instrucciones de nuestro cuerpo.";
      } else if (question.includes("física cuántica")) {
        answer = "La física cuántica estudia las partículas muy pequeñas, como los átomos. Aunque es compleja, ayuda a entender cómo funciona el universo a nivel microscópico.";
      } else if (question.includes("teoría de la relatividad")) {
        answer = "La teoría de la relatividad explica cómo el espacio y el tiempo pueden cambiar según la velocidad y la gravedad. Fue desarrollada por Albert Einstein.";
      } else if (question.includes("ecuación")) {
        answer = "Una ecuación es una igualdad matemática donde hay una incógnita que debemos encontrar. Por ejemplo: x + 2 = 5.";
      } else if (question.includes("literatura")) {
        answer = "La literatura es el arte de escribir y leer textos. Incluye cuentos, novelas, poemas y más.";
      } else if (question.includes("ecosistema")) {
        answer = "Un ecosistema es un conjunto de seres vivos y el lugar donde viven, como un bosque o un lago.";
      } else if (question.includes("fotosíntesis")) {
        answer = "La fotosíntesis es el proceso por el cual las plantas crean su alimento usando la luz del sol.";
      } else if (question.includes("matemáticas avanzadas")) {
        answer = "Las matemáticas avanzadas incluyen temas como álgebra, geometría y cálculo. Nos ayudan a resolver problemas más complejos.";
      } else if (question.includes("filosofía")) {
        answer = "La filosofía es el estudio de preguntas profundas sobre la vida, la existencia, el conocimiento y los valores.";
      } else {
        // Si la pregunta es difícil y no está en la lista
        answer += "Intenta buscar información en libros o preguntar a un profesor. Siempre es bueno seguir aprendiendo y preguntar sin miedo.";
      }

      document.getElementById('answer').innerText = answer;
    }
  </script>
</body>
</html>
