
<template>
  <header class="navbar">
    <img alt="logo pizzeria" src="../assets/logo.png" class="logo">
  </header>
  <body>
    <div class="div-banner">
      <img alt="immagine banner" src="../assets/banner.png" class="banner">
      <h1>DAR PIZZAROLO ROMANO</h1>
      <h3>La Miglior Pizza De Roma</h3>
    </div>
    <div id="lista-pizze">
      <div class="info-pizza">
        <img alt="immagine margherita" src="../assets/margherita.png" class="pizze">
        <div class="list-right">
          <p>
            MARGHERITA
          </p>
          <p>
            pomodoro, mozzarella, basilico fresco, olio
          </p>
          <P CLASS="prezzo">
            5,5€
          </P>
        </div>
      </div>
      <div class="info-pizza">
        <img alt="immagine capricciosa" src="../assets/capricciosa.png" class="pizze">
        <div class="list-right">
          <p>
            CAPRICCIOSA
          </p>
          <p>
            pomodoro, mozzarella, prosciutto crudo, funghi, olive nere, carciofini e uova
          </p>
          <P CLASS="prezzo">
            7€
          </P>
        </div>
      </div>
      <div class="info-pizza">
        <img alt="immagine boscaiola" src="../assets/boscaiola.png" class="pizze">
        <div class="list-right">
          <p>
            BOSCAIOLA
          </p>
          <p>
            funghi champignon, salsiccia, mozzarella e olio
          </p>
          <P CLASS="prezzo">
            6,5€
          </P>
        </div>
      </div>
      <div class="info-pizza">
        <img alt="immagine crostino" src="../assets/crostino.png" class="pizze">
        <div class="list-right">
          <p>
            CROSTINO
          </p>
          <p>
            prosciutto cotto, mozzarella e olio
          </p>
          <P CLASS="prezzo">
            6€
          </P>
        </div>
      </div>
      <div class="info-pizza">
        <img alt="immagine marinara" src="../assets/marinara.png" class="pizze">
        <div class="list-right">
          <p>
            MARINARA
          </p>
          <p>
            pomodoro, origano, peperoncino e olio
          </p>
          <P CLASS="prezzo">
            4,5€
          </P>
        </div>
      </div>
      <div class="info-pizza">
        <img alt="immagine napoli" src="../assets/napoli.png" class="pizze">
        <div class="list-right">
          <p>
            NAPOLI
          </p>
          <p>
            pomodoro, alici e mozzarella 
          </p>
          <P CLASS="prezzo">
            6€
          </P>
        </div>
      </div>
    </div>
    <div class="button">
      <button @click="mostra('div-form')" class="ordina-ora">ORDINA ORA</button>
    </div>
    <div id="div-form">
      <form class="form-ordine">
        <label class="nome">Nome<input type="text" placeholder="Mario"></label><br>
        <label class="cognome">Cognome<input type="text"  placeholder="Rossi"></label><br>
        <label class="email">Email<input type="email"  placeholder="example@gmail.com"></label><br>
        <label class="Cellulare">Cellulare<input type="number" placeholder="3278695789"></label><br>
        <label class="indirizzo">Indirizzo<input type="text" placeholder="via tal dei tali 107, roma"></label><br>
        <label class="testo">Ordine<input type="text" placeholder="Margerita, Diavola"></label><br>
        <button>INVIA ORDINE</button><!--aggiungere messaggio ordine inviato-->
      </form>
    </div>  
  </body>
  <footer>
    <h4>DAR PIZZAROLO ROMANO</h4>
    <h4>DARPIZZAROLOROMANO@gmail.com</h4>
    <h3>3274598765</h3>
  </footer>
</template>

<script>
import '../assets/styles/components/homepage.scss'
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  methods: {
    mostra(id) {
      var divform = document.getElementById(id);
      if (divform.style.display === "none") {
        divform.style.display = "block";
      } else {
        divform.style.display = "none";
      }
    }
  }
}
</script>