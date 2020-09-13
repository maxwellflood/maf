<script>

</script>

<nav>
    <div class="nav-wrapper">
        <p>Work</p>
        <div class="menu">
            <div class="menu-btn"></div>
        </div>
        <p>Profile</p>
    </div>
</nav>

<style>
    nav{
        position: fixed;
        top: 0;
        padding: 24px 32px;
        width: 100%;
        /* background-color: var(--white); */
        z-index: 100;
    }
    .nav-wrapper{
        width: 100%;
        height: 32px;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    p{
        font-family: var(--roslindale);
        font-style: normal;
        font-weight: light;
        font-size: 24px;
        line-height: 1;
    }
    .menu{
        width:32px;
        height: 32px;
        display: flex;
        justify-content: center;
        align-items: center;
        cursor: pointer;
    }
    .menu-btn{
        width: 4px;
        height: 4px;
        background-color: var(--black);
        border-radius: 50%;
        transition: 0.2s ease;
    }
    .menu:hover > .menu-btn{
        width: 8px;
        height: 8px;
    }

</style>