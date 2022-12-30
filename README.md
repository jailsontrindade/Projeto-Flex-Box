<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maxmum-scale=1, user-scable=no">
    <title>Contato</title>
    <link rel="stylesheet" href="css/styles.css">
</head>
<body>
    <div id="main-container">
        <!-- Informações de Endereço -->
        <div id="address-container">
            <div class="fade"></div>
            <div id="address-content">
              <h2><ion-icon name="navigate-outline"></ion-icon> Endereço</h2>
              <p>Rua das Flores, 133</p>
              <h2><ion-icon name="call-outline"></ion-icon> Telefone</h2>
              <p>(71)99999-9999</p>
              <h2><ion-icon name="mail-outline"></ion-icon> E-mail</h2>
              <p>meuemail@email.com</p>
            </div>  
        </div>
        <!-- Formulário Para Contato -->
        <div id="form-container">
            <h2>Nos mande uma Mensagem</h2>
            <form id="contact-form">
                <label for="name">Name:</label>
                <input type="text" name="name" placeholder="Digite seu nome">
                <label for="email">E-mail:</label>
                <input type="email" name="email" placeholder="Digite seu e-mail">
                <label for="phone">Telefone:</label>
                <input type="text" name="phone" placeholder="Digite seu Telefone">
                <label for="msg">Sua Mensagem:</label>
                <textarea name="msg" placeholder="Como podemos te ajudar"></textarea>
                <input type="submit" value="Enviar Mensagem">
            </form>
        </div>
    </div>
    <script type="module" src="https://unpkg.com/ionicons@5.5.2/dist/ionicons/ionicons.esm.js"></script>
</body>
</html>

____________________________________________________________________________________________________________________________________________________________________

/* GERAL */

* {
    margin: 0;
    padding: 0;
    font-family: Arial;
    box-sizing: border-box;  
}

/* CONTAINERS */

#main-container {
    display: flex;
    flex-direction: row;
    height: 100vh; /* view height */
}

#address-container, #form-container {
    flex: 1 1 0;
    height: 100%;
    text-align: center;
}

/* ADDRESS CONTAINER */

#address-container {
    background-image: url('../css/Nova\ York.jpg.jpg');
    background-size: cover;
    background-position-x: -400px;
    color: #fff;
    position: relative;
}

.fade {
    width: 100%;
    height: 100%;
    background: #000;
    opacity: .7;
}

#address-content {
    position: absolute;
    top: 25vh;
    left: 35%;
    width: 300px;
    border: 7px solid yellowgreen;
    border-radius: 20%;
    border-top: 20px;
}


#address-content h2 {
    color: #00ad5e;
    margin-bottom: 15px;
    position: relative;
    padding-left: 18px;
}

#address-content ion-icon {
    position: relative;
    top: 2px;
    left: 0;
}

#address-content p {
    font-weight: bold;
    margin-bottom: 70px;
}

/* FORM CONTAINER */
#form-container {
    padding-top: 60px;
    text-align: center;
}

#form-container h2 {
    color: #888;
    margin-bottom: 50px;
    font-size: 30px;
}

#contact-form {
    width: 500px;
    margin-left: auto;
    margin-right: auto;
    text-align: left;
}

#contact-form input,
#contact-form label,
#contact-form textarea {
    display: block;
    padding: 10px;
    border: 1px solid #eee;
    width: 100%;
    color: #aaa;
}

#contact-form label {
    color: #999;
    font-weight: bold;
    border-bottom: none;
}

#contact-form input {
    margin-bottom: 15px;
}

#contact-form input::placeholder,
#contact-form textarea::placeholder {
    color: #bbb;
}

#contact-form input[type="submit"] {
    background-color: #00ad5e;
    color: #FFF;
    font-size: 16px;
    font-weight: bold;
    cursor: pointer;
    width: 300px;
    margin: 30px auto;
    border: 2px solid transparent;
    transition: .5s;
}

#contact-form input[type="submit"]:hover {
    border-color: #00ad5e;
    color: #00ad5e;
    background-color: #FFF;
}
