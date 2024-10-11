<template>
<div class="carnet">
    <aside>
    <div>
        <span>CEDULA DE INDENTIDAD</span>
        <img width="40" src="../assets/chile_bandera.png" alt="Bandera de Chile" />
    </div>

    <img src="../assets/foto_elon.jpg" alt="Elon Mosk" />
    <p>RUN {{RUN}}</p>
    </aside>

    <main>
    <header>
        <p>REPUBLICA DE CHILE</p>
        <span>SERVICIO DE REGISTRO CIVIL E IDENTIFICACIÓN</span>
    </header>
    <section>
        <article>
        <header>APELLIDOS</header>
        <span>{{ Apellidos }}</span>
        </article>
        <article>
        <header>NOMBRES</header>
        <span>{{Nombres}}</span>
        </article>

        <div class="grid-2-colums">
        <article>
            <header>NACIONALIDAD</header>
            <span>{{Nacionalidad}}</span>
        </article>
        <article>
            <header>SEXO</header>
            <span>{{Sexo}}</span>
        </article>
        </div>
        <div class="grid-2-colums">
        <article>
            <header>FECHA DE NACIMIENTO</header>
            <span>{{Fecha_de_nacimiento}} </span>
        </article>
        <article>
            <header>NÙMERO DOCUMENTO</header>
            <span>{{Número_de_documento}}</span>
        </article>
        </div>
        <div class="grid-2-colums">
        <article>
            <header>FECHA DE EMISIÒN</header>
            <span>{{Fecha_de_emisión}}</span>
        </article>
        <article>
            <header>FECHA DE VENCIMIENTO</header>
            <span>{{Fecha_de_vencimiento}}</span>
        </article>
        </div>
        <article>
        <header>FIRMA DEL TITULAR</header>
        <span>X Æ A-12</span>
        </article>
    </section>
    </main>
</div>
</template>

<script>
export default {
name: "Identificacion",
data() {
    return {
        RUN: '26.876.653-5',
        Apellidos: 'Peñalver Alcalá',
        Nombres: 'Alfredo Enrique',
        Nacionalidad: 'Venezolano',
        Sexo: 'Masculino',
        Fecha_de_nacimiento:'14-12-1990',
        Número_de_documento: '604.345.543',
        Fecha_de_emisión: '13-01-2021',
        Fecha_de_vencimiento: '12-12-2034'
    };
},
};
</script>

<style scoped>
body {
display: flex;
justify-content: center;
align-items: center;
height: 60vh;
font-size: 10px;
font-family: sans-serif;
}

.carnet {
width: 400px;
height: 230px;
background: #c8deed;
border-radius: 20px;
display: grid;
grid-template-columns: 30% 1fr;
padding: 15px;
box-shadow: 0px 0px 10px 2px black;
}

aside div {
display: flex;
}

aside > img {
margin-top: 15px;
width: 100%;
}

aside p {
text-align: center;
font-size: 12px;
font-weight: bold;
}

main {
padding: 0px 14px;
}

main article {
margin: 4px 0px;
}

main article header {
font-weight: bold;
color: #0235a4;
font-size: 8px;
}

main header p {
font-size: 20px;
margin: 0;
font-weight: bold;
color: #0235a4;
}

main header span {
font-size: 8px;
color: #399be1;
}

main section {
margin-top: 10px;
}

main section article span {
font-size: 13px;
font-weight: 600;
}

main section .grid-2-colums {
display: grid;
grid-template-columns: 50% 50%;
}
</style>
