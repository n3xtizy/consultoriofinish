<template>
  <div class="container">
    <h1 class="titulo" >Lista de Médicos</h1>
    <div class="control">
      <input class="input" type="busca-medico" placeholder="Buscar Médico">

      <router-link class="link-cad" to="/medico/cadastrar">
        <button class="button is-info is-outlined btn-cadastrar">Cadastrar</button>
      </router-link>

    </div>
    <div class="table-medicos">
      <table class="table">
        <thead>
        <tr>
          <th>Id</th>
          <th>Nome</th>
          <th>CRM</th>
          <th>Especialidade</th>
          <th>% Participação</th>
          <th>Valor Consulta</th>
          <th>Celular</th>
          <th>Opções</th>
        </tr>
        </thead>
        <tbody>
        <tr>
          <th>1</th>
          <td>AA bb</td>
          <td>9999999</td>
          <td>Pediatra</td>
          <td>15</td>
          <td>310,00</td>
          <td>(45)99999-9999</td>
          <td>
            <router-link to="/medico/detalhar">
              <button class="button is-info">Detalhar</button>
            </router-link>
          </td>
        </tr>
        <tr>
          <th>2</th>
          <td>CC dd</td>
          <td>45547854</td>
          <td>Cardiologista</td>
          <td>20</td>
          <td>290,00</td>
          <td>(45)99999-99999</td>
          <td>
            <router-link to="/medico/detalhar">
              <button class="button is-info">Detalhar</button>
            </router-link>
          </td>
        </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>

<script>
export default {
  name: "medico"
}
</script>

<style lang="scss">
@import "~bulma/bulma.sass";
.titulo{
  font-size: 30px;
  margin-top: 0px;
  margin-outside: 10px;
}
.input{
  width: 60%;
}
.table-medicos{
  margin-top: 60px;
}
.table{
  width: 91.4%;
  border-style: solid;
  border-color: darkgrey;
  border-width: 1px;
}
.link-cad{
  width: 30%;

}
.btn-cadastrar{
  width: 100%;
  height: 100%;
  margin-left: 20px;
  background-color: green;
  color: white;
  border-radius: 5px;
  border-width: 0px;
  font-size: 17px;
}
.control{
  display: flex;
  margin-top: 20px;
  width: 100%;
  flex-direction: row;
}
</style>