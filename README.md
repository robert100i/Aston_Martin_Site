/* RESET */
* {
    font-family: 'Inter', sans-serif;
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

/* BODY */
body {
    background-color: #000;
    color: #FFF;
    width: 100%;
    height: auto;
}

/* HEADER */
.header {
    width: 100%;
    height: 80px;
    background-color: #000;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0 20px;
    position: fixed;
    top: 0;
    left: 0;
    z-index: 1000;
}

.logo {
    width: 80px;
}

.itens-nav {
    display: flex;
    align-items: center;
}

.itens-nav ul {
    display: flex;
    list-style: none;
}

.nav-link {
    text-decoration: none;
    color: #FFF;
    font-size: 16px;
    margin-right: 20px;
}

.button1 {
    border: solid 1px #FFF;
    border-radius: 10px;
    color: #FFF;
    text-decoration: none;
    padding: 8px 22px;
    background: none;
}

/* MENU MOBILE */
.menu-toggle {
    display: none;
    font-size: 28px;
    color: #FFF;
    cursor: pointer;
}

/* SEÇÕES PRINCIPAIS */
.main {
    padding: 100px 20px 20px;
    text-align: center;
}

.section {
    max-width: 1200px;
    margin: 50px auto;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    text-align: left;
}

.box-text1, .box-text2, .box-text3 {
    flex: 1;
    min-width: 300px;
    padding: 20px;
}

.box-text1 h2 {
    font-size: 48px;
}

.car1, .car2, .car3 {
    max-width: 100%;
    height: auto;
    margin-top: 20px;
}

/* BOTÕES */
.button2, .button3 {
    border: solid 1px #FFF;
    border-radius: 10px;
    color: #FFF;
    text-decoration: none;
    padding: 14px 40px;
    font-size: 15px;
    background: none;
}

/* FOOTER */
.footer {
    width: 100%;
    background-color: #FFF;
    color: #000;
    text-align: center;
    padding: 20px;
}

.logo-name {
    max-width: 100px;
    margin-bottom: 20px;
}

.line {
    width: 80%;
    border: solid 2px #A4A4A4;
    margin: 10px auto;
}

/* RESPONSIVO */
@media (max-width: 768px) {
    /* MENU MOBILE */
    .menu-toggle {
        display: block;
    }

    .itens-nav {
        display: none;
        flex-direction: column;
        position: absolute;
        top: 80px;
        left: 0;
        width: 100%;
        background: #000;
        text-align: center;
        padding: 20px 0;
    }

    .itens-nav.active {
        display: flex;
    }

    .itens-nav ul {
        flex-direction: column;
        gap: 15px;
    }

    /* SEÇÕES */
    .section {
        flex-direction: column;
        text-align: center;
    }

    .box-text1, .box-text2, .box-text3 {
        text-align: center;
    }

    /* BOTÕES */
    .button1, .button2, .button3 {
        width: 100%;
        display: block;
        text-align: center;
    }

    /* IMAGENS */
    .car1, .car2, .car3 {
        width: 100%;
    }
}
