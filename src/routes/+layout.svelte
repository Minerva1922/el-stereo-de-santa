<script>
    import "../app.css";
</script>

<main>
    <slot />
</main>


<section>
    <h1>El Stereo de Santa</h1>
</section>

<style>
     h1 {
         color: #CC1C1C;
         font-size: 40px;
         text-align: center;
     }

     section {
         background-color: #FEF9E2;
         width: 324px;
         height: 778px;
         margin-top: 67px;
         display: flex;
         justify-content: center;
         position: absolute;
         margin-left: 48px;
         border-radius: 25px;
         border: 5px solid #CC1C1C;
     }
     main {
        width: 16px;
        height: 16px;
     }

</style>