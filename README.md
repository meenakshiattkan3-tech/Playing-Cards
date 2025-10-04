# Playing-Cards
A simple webpage that displays a set of playing cards using HTML5 and CSS3 Flexbox. This project demonstrates how to structure and style elements with modern Flexbox properties to create clean, responsive layouts.
** start of index.html **

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Playing Cards</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <main id="playing-cards">
    <div class="card">
      <div class="left">♠</div>
      <div class="middle">
        <div>Ace</div>
        <div>♠</div>
      </div>
      <div class="right">♠</div>
    </div>
    <div class="card">
      <div class="left">♥</div>
      <div class="middle">
        <div>Queen</div>
        <div>♥</div>
      </div>
      <div class="right">♥</div>
    </div>
    <div class="card">
      <div class="left">♦</div>
      <div class="middle">
        <div>10</div>
        <div>♦</div>
      </div>
      <div class="right">♦</div>
    </div>
  </main>
</body>
</html>



** end of index.html **

** start of styles.css **

#playing-cards {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  gap: 20px;
  padding: 20px;
  background-color: #f0f0f0;
}

.card {
  display: flex;
  justify-content: space-between;
  width: 150px;
  height: 200px;
  background-color: white;
  border: 2px solid #ccc;
  border-radius: 10px;
  padding: 10px;
  box-shadow: 2px 2px 8px rgba(0,0,0,0.1);
}

.left {
  align-self: flex-start;
  font-size: 20px;
}

.middle {
  align-self: center;
  display: flex;
  flex-direction: column;
  align-items: center;
  font-size: 18px;
}

.right {
  align-self: flex-end;
  font-size: 20px;
}





** end of styles.css **
