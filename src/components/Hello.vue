  <template>
    <div class="hello">
      <div class="menu">
        
        <div class="icones">
          <div class="logo"><img src="../assets/logo.svg"></div>
          <div class="procura"><img src="../assets/menu.svg"></div>
          <div class="lupa"><img src="../assets/lupa.svg"></div>
        </div>
      </div>
        <h2 class="text">De tanto ganhar meias de Natal, <br>tio-avô ganha livro e tenta calçá-lo</br></h2>
        <img src="../assets/livros.jpg" class="livro">
        <p class="corpo">Foi uma cena estranha no Natal antecipado da família Siqueira, na zona norte do Rio de Janeiro. Bem mais estranha do que a Tia Julinha perguntando à sobrinha Cássia pela 76º vez quando ela ia se casar. Ou o cunhado Valcir tentando entoar Então é Natal, da Simone. Eram quase onze da noite quando o tio-avô Onofre, de 77 anos, ganhou seu presente. Abriu e era um um livro, a biografia de Jô Soares, que sua irmã Olga comprara com ótimo preço na Saraiva. Onofre olhou, olhou e olhou o livro por muitos minutos. Os parentes imaginaram que ele estava emocionado. De repente Onofre se sentou, tirou seu sapato e colocou o livro perto do pé. A família demorou a entender: ele estava tentando calçar o livro. Resultado das meias que ganhou nos últimos 17 anos.</p>
      <div class="rodape">
        <h3 class="rodape-comentario">Comentários</h3>
          <hr align="center">
          <div v-for="dialogo in usuario.conversa">
            <p>{{dialogo}}</p>
          </div>

        <ul>
          <li>
            <img src="../assets/profile.svg"></li>
            <label>
              
              <input placeholder="Digite um comentario:" type="text" name="author" maxlength="50" required="">
            </label>
            <button v-on:click>{{Envio}}</button>
          <li>
            <img src="../assets/profile2.svg">
                <h4 class="coment">
                  <p class="nomes">
                    Camila RJ
                  </p>
                  "Eu teria feito o mesmo sinceramente. Papai Noel nunca me deu oq eu pedi"
                </h4>
          </li>
          <li>
            <img src="../assets/profile3.svg">
              <h4 class="coment">
                <p class="nomes">
                  Joaquim Campinas
                </p>
                 "kkkkkkkkkkkkkkkkkkkk rindo até 2049. Muito engraçado!!!!!"
              </h4>

          </li>
        </ul>
      
      </div>

    </div>

  </template>

  <script>
  export default {
    name: 'hello',
    data () {
      return {
        Envio: 'Enviar',
        usuario:'',
        user:{
          conversa:[''],
        
        }  
      }
        
    },
    methodos:{
      adcdialogo(Envio){
        return this.user.conversa.push(this.usuario),
                this.Envio=''
      }
    }
      
  }

  </script>

  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style>

  body{
  }

  div.menu{ 
            height: 56px;
            padding: 0 16px 0 24px;
            background-color: #000000;

  }

  
  .logo{
        width: 126px;
        height: 33px;
        margin: auto;
        padding: 10px 0 0 10px;
        
  }
  .procura{ 
          width: 32.09px;
          height: 19.4px;
          margin-right: 20px;
          margin-top: -23px;


  }

  .lupa{  
          width: 23.8px;
          height: 23.77px;
          margin-left: 90%;
          margin-top: -20px;
          

  }
  
  .text{ 
        font-family: 'Open Sans, Bold';
        font-size: 18px; 
        text-align: center;}

  .livro{
          width: 90%;  
  }

  .corpo{
        font-family: 'Open Sans, Regular';
        font-size: 14px;
        margin: 15px;
        text-align: justify;

  }

  .rodape{
    min-height: 70vh;
  }
 

  .rodape-comentario{
                    font-family: 'Open Sans, Bold';
                    text-align:left;
                    font-size: 1em;
                    margin-left: 14px;
                    height: 5px;
  }

  hr{ 
      size: 1px;
      width: 93%;


  }

  ul{
    list-style: none;
    width: 90%;
    height: 250px;
    padding-left: 13px;
    margin:2px 10px;
  }

  li{
    display: flex;
    width: 116%;
    height: 64px;
    margin-left: -55px;
    padding-bottom: 30px;
    min-width: 100px;
 +    min-height: 20%;
  }

  .coment{ 
          font-family: 'Open Sans, Bold';
          font-size:0.80em;
          width: 180px;
          text-align: left;
          color: #979797;
          margin: 2px;
       }

  input{padding: 6px;
    border: 1px solid #ccc;
    box-sizing: border-box;
    width: 90%;
    background: #f9f9f9;
    font-size: 15px;}

  .nomes{
          font-weight: bold;
          color: #000000;
          margin: 3px;
}

  
label{ 
font-weight: 700;
    margin-right: 18%;
    display: inline-block;
    font-size:0.76em }


                              @media (min-width: 1088px){
                              .text{
                                font-size:24px;
                              }

                              .livro{
                                width: 180vh;
                              }
                              hr{
                                width: 98%;
                              }

                              .corpo{
                                font-size: 20px;
                              }

                              .rodape-comentario{
                                font-size: 18px;
                              }

                              .coment{
                                font-size: 16px;
                                width: 50%;
                              }

                            }
  </style>
