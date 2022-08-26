<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <script src="https://kit.fontawesome.com/8400bb1863.js" crossorigin="anonymous"></script>
    <link rel="stylesheet" href="style.css">
    <title>Page Academia - VidioAula</title>
</head>
<body>
    <header>
        <div class="menu-content">
           <h1 class="logo"> AcademiaInfinity</h1>
           <nav class="header-menu"> 
            <ul class="list-itens">
                <li><a href="#">home</a></li>
                <li><a href="#">serviços</a></li>
                <li><a href="#">aulas</a></li>
                <li><a href="#">agenda</a></li>
                <li><a href="#">contato</a></li>
                <li><a href="#"><i class="fa-brands fa-facebook-f"></i></a></li>
                <li><a href="#"><i class="fa-brands fa-instagram"></i></a></li>
            </ul>
           </nav>
        </div>
    </header>
    <main>
        <div class="main-content">
            <h1 class="primary-text">Malhar não fica mais fácil, você que fica melhor!</h1>
            <h2 class="second-text">SE INSCREVA E MUDE SUA VIDA</h2>
            <div class="btns">
              <button class="btn-exp">Agendar aula experimental</button>
              <button class="btn-personal">Contactar personal trainer</button>  
            </div>
        </div>
    </main>
</body>
</html>

@import url('https://fonts.googleapis.com/css2?family=Lato:wght@400;700&display=swap');

/*Zerando o CSS*/

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}


/* fundo-tela*/

html{
    width: 100vw;
    height: 100vh;
    font-size: 62.5%;
    color: white;
    font-family: 'Lato', sans-serif;
}

body{
    background: linear-gradient(rgba(17, 17, 17, 0.8 ), rgba(20, 20, 20, 1)), url(/img/acad.jpg);
    background-position: center center;
    background-size: cover;
    background-position-y: 0px;
    background-repeat: no-repeat;
}

/*menu - header */

header{
    width: 100%;
    height: 7vh;
    background-color: rgba(22, 22, 22, 0.2);
}

.menu-content {
    text-transform: uppercase;
    height: 100%;
    display: flex;
    justify-content: space-around;
    align-items: center;
    font-size: 1.8rem;
}

.logo {
    font-size: 1.8rem;
    letter-spacing: 0.4rem;
    cursor: pointer;
}

.menu-content .list-itens {
    display: flex;
    list-style: none;
    gap: 10px;
}

.menu-content .list-itens a {
    text-decoration: none;
    color: white;
    padding: 1.5rem;
    transform: 2ms ease-in;
    position: relative;
}


.menu-content .list-itens a:before {
    content: ' ';
    position: absolute;
    bottom: 0px;
    left: 0px;
    width: 0px;
    height: 1px;
    background-color: rgb(255, 238, 0);
    transition: all 1.5s ease;
}

.menu-content .list-itens a:hover:before {
    width: 100%;
}

/* Centro - Conteudo ´rincipal*/

main{
    height: 93vh;
    display: flex;
    justify-content: center;
    align-items: center;
}

.main-content {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

/* texto conteudo ´principal*/

.primary-text {
    width: 850px;
    font-size: 5rem;
    margin-bottom: 2rem;
    text-align: center;
}

.second-text {
    margin-bottom: 7rem;
    font-size: 2rem;
    color: rgb(165, 165, 165);
    text-transform: uppercase;
}

/*botões*/


.btns{
    display: flex;
    justify-content: center;
    gap: 20px;
}

.btns button {
    width: 250px;
    height: 60px;
    cursor: pointer;
    border: 1px solid white;
    color: white;
    text-transform: uppercase;
    background-color: transparent;
    font-weight: bold;
    letter-spacing: 0.2rem;
    border-radius: 20px;
    position: relative;
    transition: 1.5s;
}

.btns button:hover{
    color: rgb(255, 238, 0);
    border: none;
}

.btns button:before {
    content: ' ';
    border-radius: 20px;
    bottom: 0;
    left: 0;
    position: absolute;
    width: 0%;
    height: 60px;
    background-color: rgb(61, 61, 61);
    z-index: -1;
    transition: 1s;
}

.btns button:hover:before {
    width: 100%;
}
