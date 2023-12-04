<script>
  import fondo from "$lib/img/fondo.png";
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
      <a href="/editar_lista_repro">Editar Playlist</a>
      <a href="/programar_horarios">Programar horarios</a>
      <a href="/reproducción">Reproducción</a>
    </div>
{/if}

<div class="img-fondo">
    <img class="img-fondo" src={fondo} alt="img-fondo"/>
</div>

  
<style>
  
  button {
    color: #0C483F;
    background: #CC1C1C;
    border: none;
    border-radius: 15px;
    height: 60px;
    width: 70px;
    margin: 10px;
    justify-content: space-between;
    display: flex;
  }

    .menu-container {
    position: absolute;
    top: 80px;
    left: 10px;
    background-color: #FEF9E2;
    border: 2px solid #CC1C1C;
    border-radius: 5px;
    padding: 10px;
    z-index: 1;
  }

  .menu-container a {
    display: block;
    padding: 8px;
    text-decoration: none;
    color: #0C483F;
    margin-bottom: 8px;
  }

  .img-fondo {
        width: 100%;
        margin: 0;
        object-fit: cover;
        background-repeat: no-repeat;
    }
  

</style>
