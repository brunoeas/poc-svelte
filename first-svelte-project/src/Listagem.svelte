<script>
  export let data = [];
</script>

<style>
  .table {
    width: 100%;
    height: 100%;
    border-radius: 10px;
    background-color: white;
  }

  .table-head-col {
    height: 40px;
    font-size: 1.5rem;
    border-bottom: 0.5px solid rgb(0, 0, 0, 0.5);
    display: flex;
    align-items: center;
    justify-content: space-around;
    flex: 1;
  }

  .table-head-row,
  .table-body-row {
    display: flex;
    flex-direction: row;
    width: 100%;
    justify-content: space-around;
    align-items: center;
  }

  .table-body-row {
    border-bottom: 0.5px solid rgb(0, 0, 0, 0.2);
  }

  .table-body-col {
    height: 30px;
    padding: 10px;
  }
</style>

<div class="table">

  <div class="table-head">
    <div class="table-head-row">
      <div class="table-head-col">Usuário</div>

      <div class="table-head-col">E-mail</div>
    </div>
  </div>

  <div class="table-body">
    {#each data as { nome, email }}
      <div class="table-body-row">
        <div class="table-body-col">{nome}</div>

        <div class="table-body-col">{email}</div>
      </div>
    {/each}
  </div>

</div>
