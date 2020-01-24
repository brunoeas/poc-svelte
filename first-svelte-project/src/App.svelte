<script>
  import Listagem from './Listagem.svelte';

  const data = [
    { nome: 'Roberto', email: 'robertin@email.com' },
    { nome: 'Carlos', email: 'carlota@email.com' }
  ];
</script>

<style>
  .container-listagem {
    padding: 30px;
    flex: 1;
  }

  .root {
    background-color: #ebebeb;
    width: 100vw;
    height: 100vh;
    display: flex;
  }
</style>

<div class="root">
  <div class="container-listagem">
    <Listagem {data} />
  </div>
</div>
