<script>

export default {
  name: 'App',
  data() {
    return {
      titulo1: "CEDULA DE INDENTIDAD",
      titulo2: "REPUBLICA DE CHILE",
      titulo3: "SERVICIO DE REGISTRO CIVIL E IDENTIFICACIÓN",
      titulo4: "APELLIDOS",
      titulo5: "NOMBRES",
      titulo6: "NACIONALIDAD",
      titulo7: "SEXO",
      titulo8: "FECHA DE NACIMIENTO",
      titulo9: "NÙMERO DOCUMENTO",
      titulo10: "FECHA DE EMISIÒN",
      titulo11: "FECHA DE VENCIMIENTO",
      titulo12: "FIRMA DEL TITULAR",
      run: "RUN 22.222.222-2",
      apellidos: "MUSK",
      nombres: "ELON REEVE",
      nacionalidad: "SUDAFRICANO",
      sexo: "M",
      fechaDeNacimiento: "28 JUN 1971",
      numeroDeDocumento: "222.222.222",
      fechaDeEmision: "01 ENE 2025",
      fechaDeVencimiento: "01 ENE 2030",
      firmaTitular: "X Æ A-12"

    }
  },

};
</script>

<template>
  <div class="carnet">
    <aside>
      <div>
        <span>{{ titulo1 }}</span>
        <img width="40" src="./assets/img/chile_bandera.png" alt="" />
      </div>
      <img src="./assets/img/foto_elon.jpg" alt="" />
      <p>{{ run }}</p>
    </aside>
    <main>
      <header>
        <p>{{ titulo2 }}</p>
        <span>{{ titulo3 }}</span>
      </header>
      <section>
        <article>
          <header>{{ titulo4 }}</header>
          <span>{{ apellidos }}</span>
        </article>
        <article>
          <header>{{ titulo5 }}</header>
          <span>{{ nombres }}</span>
        </article>

        <div class="grid-2-colums">
          <article>
            <header>{{ titulo6 }}</header>
            <span>{{ nacionalidad }}</span>
          </article>
          <article>
            <header>{{ titulo7 }}</header>
            <span>{{ sexo }}</span>
          </article>
        </div>
        <div class="grid-2-colums">
          <article>
            <header>{{ titulo8 }}</header>
            <span>{{ fechaDeNacimiento }} </span>
          </article>
          <article>
            <header>{{ titulo9 }}</header>
            <span>{{ numeroDeDocumento }}</span>
          </article>
        </div>
        <div class="grid-2-colums">
          <article>
            <header>{{ titulo10 }}</header>
            <span>{{ fechaDeEmision }}</span>
          </article>
          <article>
            <header>{{ titulo11 }}</header>
            <span>{{ fechaDeVencimiento }}</span>
          </article>
        </div>
        <article>
          <header>{{ titulo12 }}</header>
          <span>{{ firmaTitular }}</span>
        </article>
      </section>
    </main>
  </div>
</template>
<style>
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

aside>img {
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