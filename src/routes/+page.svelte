<script>
  let showMenu = false;

  function toggleMenu() {
    showMenu = !showMenu;
  }
</script>

<button on:click={toggleMenu}>
  <svg xmlns="http://www.w3.org/2000/svg" width="36" height="36" fill="currentColor" class="bi bi-list" viewBox="0 0 16 16">
    <path fill-rule="evenodd" d="M2.5 12a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5zm0-4a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5zm0-4a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5z"/>
  </svg>
</button>

{#if showMenu}
  <div class="menu-container">
    <a href="/">Editar Playlist</a>
    <a href="/">Programar horarios</a>
    <a href="/">Opción 3</a>
  </div>
{/if}

<style>
  button {
    color: #0C483F;
    background: #CC1C1C;
    border: none;
    border-radius: 15px;
    height: 60px;
    width: 70px;
    margin: 10px; /* Ajusta el margen según tus necesidades */
  }

  .menu-container {
    position: absolute;
    top: 80px; /* Ajusta la posición vertical según tus necesidades */
    left: 10px; /* Ajusta la posición horizontal según tus necesidades */
    background-color: #FEF9E2;
    border: 1px solid #CC1C1C;
    border-radius: 5px;
    padding: 10px;
    z-index: 1;
  }

  .menu-container a {
    display: block;
    padding: 8px;
    text-decoration: none;
    color: #0C483F;
    margin-bottom: 8px; /* Agrega espacio entre enlaces */
  }
</style>
