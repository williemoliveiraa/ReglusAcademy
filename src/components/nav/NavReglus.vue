<template>
    <div id="raiz">
        <nav class="listasOpcoes">
            <div class="lista">
                <img :src="logo" class="logo">
                <ul>
                    <li>
                        <router-link to="/">Home</router-link>
                    </li>
                    <li>
                        <router-link to="/introducaoaprogramacao">Funcionalidades</router-link>
                    </li>
                    <li>
                        <router-link to="/agenda">Recursos</router-link>
                    </li>
                    <li>Organização</li>
                </ul>
            </div>

            <div class="lista">
                <ul>
                    <li>Sobre Nós</li>
                    <div class="div"></div>
                    <li>
                        <router-link to="/login">Fazer Login</router-link>
                    </li>
                    <li>
                        <router-link to="/redirecionarlogin" id="btnCadastro">USE GRATUITAMENTE</router-link>
                    </li>
                </ul>
            </div>
        </nav>
    </div>
</template>

<script>
export default {
    name: "NavReglus",
    data() {
        return {
            logo: require("@/assets/logoreglus.png"),
        };
    }
}
</script>

<style>
#raiz {
    padding: 0em 1.5em;
}

.logo {
    width: 150px;
}

.listasOpcoes {
    font-weight: bold;
    display: flex;
    justify-content: space-between;
}

ul {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 1.5em;
}

a {
    text-decoration: none;
    color: black;
}

.lista {
    display: flex;
}

.div {
    height: 2em;
    width: 1px;
    background-color: black;
}

#btnCadastro a {
    color: #fff;
}

#btnCadastro {
    color: #fff;
    background-color: #000;
    padding: 0.5em;
}
</style>