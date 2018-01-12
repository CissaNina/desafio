  <template>
    <div class="hello">
      <div id="menu">
        <h1>Fakenews</h1>
      </div>
        <h2>De tanto ganhar meias de Natal, tio-avô ganha livro e tenta calçá-lo</h2>
        <img src="../assets/livros.jpg">
        <p>Foi uma cena estranha no Natal antecipado da família Siqueira, na zona norte do Rio de Janeiro. Bem mais estranha do que a Tia Julinha perguntando à sobrina Cássia pela 76a vez quando ela ia se casar. Ou o cunhado Valcir tentando entoar Então é Natal, da Simone. Eram quase onze da noite quando o tio-avô Onofre, de 77 anos, ganhou seu presente. Abriu e era um um livro, a biografia de Jô Soares, que sua irmã Olga comprara com ótimo preço na Saraiva. Onofre olhou, olhou e olhou o livro por muitos minutos. Os parentes imaginaram que ele estava emocionado. De repente Onofre se sentou, tirou seu sapato e colocou o livro perto do pé. A família demorou a entender: ele estava tentando calçar o livro. Resultado das meias que ganhou nos últimos 17 anos.</p>

    </div>

  </template>

  <script>
  export default {
    name: 'hello',
    data () {
      return {
        msg: 'Welcome to Your Vue.js PWA'
      }
    }
  }
  </script>

  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style>

  menu{ 
    margin: 0;
  height: 56px;
  padding: 0 16px 0 24px;
  background-color: #35495E;
  color: #ffffff;

  }
  h1{
    margin: 0;
    padding: 0.25em 0;
    font-size: 1.85em;
    color:blue;
  }

  h2{ 
      font-family: 'Open Sans, Bold';
      font-size: 18px; 
      text-align: center;
      margin-left: 40px;
      margin-right: 50px;}

  img{
    width: 100%;  
  }

  p{
    font-family: 'Open Sans, Regular';
    font-size: 14px;
  }
  ul {
    list-style-type: none;
    padding: 0;
  }

  li {
    display: inline-block;
    margin: 0 10px;
  }

  a {
    color: #35495E;
  }


  </style>
