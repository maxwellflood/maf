<script>

</script>

<div>
    <span class="divider"></span>
    <h2><slot/></h2>
    <!-- <span class="divider"></span> -->
</div>


<style>

    h2{
        padding: 24px 0;
    }

    .divider{
        display: block;
        width: 100%;
        height: 1px;
        background-color: var(--black);
    }

    div{
        padding-bottom: 32px;
    }

    @media only screen and (max-width:900px){
        div{
            padding-bottom: 16px;
        }
    }

</style>