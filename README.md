# P.i-DE-PARANGOLE-COM-OUTROS
TURMA EI-31

Relatorio: 
Boa tarde, bom dia e boa noite, ai ai ai começar esse projetinho do PI.

Primeiro buscamos uma base visualmente bonita é funcional, achamos um video no YouTube é decidimos organizar o nosso PI através da base do site ensinada pelo video.

Link do video: https://youtu.be/zi3tKRp0fIY

Lets bora explicar o que cada parte do código faz, primeiro vamos fazer essa parte visual para agradar o público e tal.

<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" contente="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <title>SRSCJF-IF</title>
</head>
<body>
    
</body>
</html>

Esse é o nosso início meio triste, mas é isso.

Iniciamos montando uma base de código para fazer as demais importações, já lincamos também ao css e decidimos colocar uma compatibilidade a internet explore nunca se sabe de onde será acessado é as maquinas do ifba usa como navegador padrão.

O código ensinado faz bastante uso do nav. Uma breve explicação do que é: O Elemento HTML de Navegação ( <nav> ) representa uma seção de uma página que aponta para outras páginas ou para outras áreas da página, ou seja, uma seção com links de navegação.

Bom então no body (parte que vai ficar visível no código obvio né) trabalharemos assim, invés de ir para outra página com links vamos usar a mesma pagina apenas ocorrendo transição, onde o usuário pode ir ao sobre, suporte, contato e outros sem sair da página inicial. Essa é uma base, esta com lista é com links, mas futuramente vamos tirar: 

<body>
    <nav class="nav">
        <div class="nav-logo">
            <p>SRSCJF-IF</p>
        </div>
        <div class="nav-menu">
            <ul>
                <li><a href="#" class="link">Inicio</a></li>
                <li><a href="#" class="link">Sobre</a></li>
                <li><a href="#" class="link">Não definido</a></li>
                <li><a href="#" class="link">Suporte</a></li>
            </ul>
        </div>
    </nav> 

Então agora é necessário criar os botões de login e de cadastro, vale ressaltar que eles irão ficar na parte superior à direita. 

        <div class="nav-button">
            <button class="btn" id="loginBtn">Login</button>
            <button class="btn" id="registroBtn">Cadastre-se</button>
        </div>
        <div class="nav-menu-btn">
            <i class="bx bx-menu" onclick="menuFunction()"></i>
        </div>

Breve explicação sobre p "i" usado: A tag <i> pode representar uma parte do texto com uma diferença semântica, na qual a representação tipográfica padrão é no tipo itálico. Isso significa que os navegadores continuarão a apresentar o conteúdo em itálico, mas, conforme o definido, isso não é mais requerido.

onclick executa determinada funcionalidade quando um botão é clicado. Nesse caso ele realiza nossa função de transição de página.

Bom por hoje é só.

Código por enquanto:

<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" contente="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <title>SRSCJF-IF</title>
</head>
<body>
    <nav class="nav">
        <div class="nav-logo">
            <p>SRSCJF-IF</p>
        </div>
        <div class="nav-menu">
            <ul>
                <li><a href="#" class="link active">Inicio</a></li>
                <li><a href="#" class="link">Sobre</a></li>
                <li><a href="#" class="link">Não definido</a></li>
                <li><a href="#" class="link">Suporte</a></li>
            </ul>
        </div>
        <div class="nav-button">
            <button class="btn" id="loginBtn">Login</button>
            <button class="btn" id="registroBtn">Cadastre-se</button>
        </div>
        <div class="nav-menu-btn">
            <i class="bx bx-menu" onclick="menuFunction()"></i>
        </div>
    </nav>
</body>
</html>

29/06/2023
Victor Hugo 


Hoje é só dia, cansado demais em pleno recesso tendo que se preocupar com código o Tristeza.

Lets bora.

Agora vamos da continuidade ao código:

Primeiro vamos criar um contêiner (div) para ter dois tipos de div dentro dele, a de login e cadastro.

    <div class="form-box">

                <div class="login-container" id="login">
            <div class="top">
                <span>Não tem uma conta? <a href="#" onclick="()">Cadastre-se</a></span>
                <header>Login</header>
            </div> 

Antes de dar continuidade é necessário explicar o que é span, pois será realizado uso dele: O elemento HTML <span> é um contêiner genérico em linha para conteúdo fraseado, que não representa nada por natureza. Ele pode ser usado para agrupar elementos para fins de estilo (usando os atributos class ou id ), ou para compartilhar valores de atributos como

Dando continuidade ao código só ira ser criado input para pedir as informações do login, vale ressaltar que essa parte ira sofrer bastante alteração já que pode ser necessário criar mais informações no caso o login e cadastro.

            <div class="input-box">
                <input type="text" class="input-field" placeholder="Matrícula">
                <i class="bx bx-user"></i>
            </div>
            <div class="input-box">
                <input type="password" class="input-field" placeholder="Senha">
                <i class="bx bx-lock-alt"></i>
            </div>
            <div class="input-box">
                <input type="submit" class="submit" value="Entrar">
            </div>

Complementos a pagina de login necessária para um código.


            <div class="two-col">
                <div class="one">
                    <input type="checkbox" id="login-check">
                    <label for="login-check">Relembre-me</label>
                </div>
                <div class="two">
                    <label><a href="#">Esqueceu a senha?</a></label>
                </div>
            </div>
        </div>

Agora indo para parte de cadastro, ira ser do mesmo modo, só que será usado uma maior quantidade de div, ressaltando que ira sofrer alterações pelos mesmo motivos anteriores (sei que vocês do meu grupo vão só passar o olho então os motivos é: pode ser necessário pedir mais informações, pode ocorrer de alterar o modo de pedir que eu acho bem difícil, pois input são muito mais interessantes, resumindo situações adversas pode mudar o código nessa parte principalmente). 

Outro ponto que já vai ser adicionado uma função com o nome "login". Meu Deus tenho que explicar isso direito se não vão ficar voando. 

A função login() é um manipulador de eventos chamado quando o botão de login é clicado. Ela ajusta a posição dos elementos de login e registro, alterando suas propriedades da esquerda e direita no CSS para mostrar o formulário de login e ocultar o formulário de registro. Também altera as classes dos botões para realçar visualmente o botão de login selecionado e ajusta a opacidade dos formulários para mostrar ou ocultar corretamente o conteúdo (basicamente um vai ficar mais escuro que o outro).

A função cadastro() é um manipulador de eventos chamado quando o botão de registro é clicado. Ela faz o oposto da função login(), ajustando as posições dos elementos para mostrar o formulário de registro e ocultar o formulário de login. Também altera as classes dos botões para realçar visualmente o botão de registro selecionado e ajusta a opacidade dos formulários.


Código: 
        <div class="register-container" id="register">
            <div class="top">
                <span>Já tem uma conta? <a href="#" onclick="login()">Login</a></span>
                <header>Cadastre-se</header>
            </div>
            <div class="two-forms">
                <div class="input-box">
                    <input type="text" class="input-field" placeholder="Nome">
                    <i class="bx bx-user"></i>
                </div>
                <div class="input-box">
                    <input type="text" class="input-field" placeholder="Matrícula">
                    <i class="bx bx-user"></i>
                </div>
            </div>
            <div class="input-box">
                <input type="text" class="input-field" placeholder="Email">
                <i class="bx bx-envelope"></i>
            </div>
            <div class="input-box">
                <input type="password" class="input-field" placeholder="Senha">
                <i class="bx bx-lock-alt"></i>
            </div>
            <div class="input-box">
                <input type="submit" class="submit" value="Register">
            </div>
            <div class="two-col">
                <div class="one">
                    <input type="checkbox" id="register-check">
                    <label for="register-check"> Relembre-me</label>
                </div>
                <div class="two">
                    <label><a href="#">Termos & condições</a></label>
                </div>
            </div>
        </div>
    </div>
</div>

Bom a parte visual (body) sem css é basicamente isso espero que tenha explicado de um jeito que da entender para todos.

É claro que já estão com suas devidas classes aplicadas, mas no git irei posta o código completo ele dá uma visualização bacana de como fica sem css.

Bom complementando o código principal temos script: <script> O elemento HTML <script> é usado para incluir ou referenciar um script executável. Usado para fazer a ligação entre o JavaScript e o HTML. Sempre que for preciso usar JavaScript no HTML, deve-se colocar a tag <script> no lugar correto.

Primeiro script:

<script>
   
   function menuFunction() {
    var i = document.getElementById("navMenu");
    if(i.className === "nav-menu") {
        i.className += " responsive";
    } else {
        i.className = "nav-menu";
    }
   }
 
</script>

Lembra que chamei essa função no código la em cima então A função menuFunction() é um manipulador de eventos acionado quando o ícone de menu é clicado. Ele obtém o elemento com o ID navMenu e verifica sua classe. Se a classe for igual a "nav-menu", adiciona a classe "responsive" para fazer o menu ficar visível em dispositivos móveis. Caso contrário, remove a classe "responsive" para ocultar o menu.

Segundo script:

<script>
    var a = document.getElementById("loginBtn");
    var b = document.getElementById("registerBtn");
    var x = document.getElementById("login");
    var y = document.getElementById("register");
    function login() {
        x.style.left = "4px";
        y.style.right = "-520px";
        a.className += " white-btn";
        b.className = "btn";
        x.style.opacity = 1;
        y.style.opacity = 0;
    }
    function register() {
        x.style.left = "-510px";
        y.style.right = "5px";
        a.className = "btn";
        b.className += " white-btn";
        x.style.opacity = 0;
        y.style.opacity = 1;
    }

</body>
</html>
    
A variável 'a' é atribuída ao elemento do botão de login com o ID loginBtn.


    
A variável 'b' é atribuída ao elemento do botão de registro com o ID registerBtn.


    
A variável 'x' é atribuída ao elemento do formulário de login com o ID login.


    
A variável 'y' é atribuída ao elemento do formulário de registro com o ID register.

E aí que entre a função já explicada que é login e cadastro, vou da ctrl c + ctrl v:





A função login() é um manipulador de eventos chamado quando o botão de login é clicado. Ela ajusta a posição dos elementos de login e registro, alterando suas propriedades da esquerda e direita no CSS para mostrar o formulário de login e ocultar o formulário de registro. Também altera as classes dos botões para realçar visualmente o botão de login selecionado e ajusta a opacidade dos formulários para mostrar ou ocultar corretamente o conteúdo (basicamente um vai ficar mais escuro que o outro).

A função cadastro() é um manipulador de eventos chamado quando o botão de registro é clicado. Ela faz o oposto da função login(), ajustando as posições dos elementos para mostrar o formulário de registro e ocultar o formulário de login. Também altera as classes dos botões para realçar visualmente o botão de registro selecionado e ajusta a opacidade dos formulários.

Essas funções permitem alternar entre os formulários de login e cadastro quando os botões são clicados.

Então isso e tudo por hoje agora basta explicar o CSS.

Ah só para terminar mesmo.




01/07/2023
Victor hugo
