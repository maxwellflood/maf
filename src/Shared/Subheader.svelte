<script>

</script>

<div>
    <h2><slot/></h2>
    <span class="divider"></span>
</div>


<style>

    h2{
        padding-bottom: 24px;
    }

    .divider{
        display: block;
        width: 100%;
        height: 1px;
        background-color: var(--black);
    }

    div{
        padding-bottom: 64px;
    }

</style>