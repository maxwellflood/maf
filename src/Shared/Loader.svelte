<script>

    window.addEventListener('load', function(){
        setTimeout(function(){
            document.querySelector('.loader h1').style.opacity = 0;
        }, 1500)

        setTimeout(function(){
            document.querySelector('.loader').style.height = 0;
        }, 2500)
    })

</script>

<div class="loader">
    <h1>Howdy</h1>
</div>


<style>

    .loader{
        top: 0;
        left: 0;
        position: fixed;
        width: 100vw;
        height: 100vh;
        background-color: var(--black);
        z-index: 100000;
        display: flex;
        justify-content: center;
        align-items: center;
        transition: height 0.3s ease;
        pointer-events: none;
    }

    .loader h1{
        opacity: 1;
        color: var(--white);
        font-size: 12vw;
        transition: opacity 0.3s ease;
    }
    

</style>