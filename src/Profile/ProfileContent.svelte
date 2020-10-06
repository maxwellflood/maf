<script>
    import Subheader from '../Shared/Subheader.svelte'
</script>

<section>
    <div class="wrapper">
        <div class="about-wrapper">
            <Subheader>About</Subheader>
            <span class="divider"></span>
            <p class="large">
                Howdy partner, I’m Maxwell, a designer, creative director and co-founder of London based <a href="https://grotesk.studio/" target="new">Grotesk Studio</a>.
                <br/>
                <br/>
                I relish collaborating with established businesses, start-ups and friends to create engaging and exciting visual experiences.
                <br/>
                <br/>
                I’m primarily interested in working at the intersection of culture, technology and sustainability.
                <br/>
                <br/>
                If you're interested in finding out more about what I do and how I do it, feel free to get in touch any time.
                <br/>
                <br/>
                Until our paths cross again, keep it surreal. 🖖
            </p>
        </div>
        <div class="contact-wrapper">
            <Subheader>Contact</Subheader>
            <p class="large"> <a href="mailto:maxwell@grotesk.studio"> Email </a></p>
            <p class="large"> <a href="https://www.instagram.com/maxwellflood/" target="blank"> Instagram </a></p>
            <p class="large"> <a href="https://twitter.com/maxwellflood" target="blank"> Twitter </a></p>
            <p class="large"> <a href="https://www.linkedin.com/in/maxwellflood/" target="blank"> LinkedIn </a></p>
        </div>
    </div>
</section>

<style>
    section{
        width:100%;
        padding: 64px 64px 400px;
        background-color: var(--white);
    }
    .wrapper{
        margin: auto;
        max-width: 80vw;
        display: flex;
        flex-direction: row;
    }
    .wrapper div:nth-child(even){
        padding-left: 2%;
    }
    .wrapper div:nth-child(odd){
        padding-right: 2%;
    }
    .about-wrapper{
        width: 66.6%;
    }
    .contact-wrapper{
        width: 33.3%;
    }
    p.large > a{
        position: relative;
        text-decoration: none;
        color: var(--black);
    }
    p.large > a:hover{
        color: var(--black);
    }
    p.large > a::before{
        content:"";
        position: absolute;
        width: 100%;
        height: 2px;
        bottom: 0;
        left: 0;
        background-color: var(--black);
        visibility: hidden;
        transform: scaleX(0);
        transform-origin: bottom left;
        transition: all 0.3s ease 0s;
    }
    p.large > a:hover::before{
        visibility: visible;
        transform: scaleX(1);
    }

    p.large > a.inverse::before{
        content:"";
        position: absolute;
        width: 100%;
        height: 2px;
        bottom: 0;
        left: 0;
        background-color: var(--black);
        visibility: hidden;
        transform: scaleX(0);
        transform-origin: bottom left;
        transition: all 0.3s ease 0s;
    }
    p.large > a.inverse:hover::before{
        visibility: visible;
        transform: scaleX(1);
    }

 

    /* --- Mid --- */
    
    @media only screen and (max-width: 1250px) {
        p.large{
            font-size:48px;
            line-height: 56px;
        }

        section{
            width:100%;
            padding: 32px 32px 80px;
            background-color: var(--white);
        }
        .wrapper{
            margin: auto;
            max-width: 100%;
            display: flex;
            flex-direction: row;
        }
    }


    /* --- Mobile --- */
    
    @media only screen and (max-width: 900px) {
        p.large{
            font-size:32px;
            line-height: 40px;
        }

        section{
            width:100%;
            padding: 32px 32px 80px;
            background-color: var(--white);
        }
        .wrapper{
            margin: auto;
            max-width: 100%;
            display: flex;
            flex-direction: column;
        }
        .wrapper div:nth-child(even), .wrapper div:nth-child(odd){
            padding:0 0 64px;
        }

        .about-wrapper{
            width: 100%;
        }
        .contact-wrapper{
            width: 100%;
        }
    }
    

</style>