<script>
    import Profile from "../assets/profile-photo.jpg";
    import GithubLogo from "../assets/github.svg";
    import LinkedinLogo from "../assets/linkedin.svg";
    import InstagramLogo from "../assets/instagam.svg";
    import TwitterLogo from "../assets/twitter.svg";

    import { Application } from '@splinetool/runtime';

    let canvas;
    // const app = new Application(canvas);
    // app.load('https://prod.spline.design/ORTIFV2Eg-d00-49/scene.splinecode');


    const social_links = [{
        name:"Github",
        href:"https://github.com/rinto11804",
        logo_src:GithubLogo,
    },
    {
        name:"Linkedin",
        href:"www.linkedin.com/in/rintojosephtr",
        logo_src:LinkedinLogo,
    },
    {
        name:"Instagram",
        href:"https://www.instagram.com/rinto_josephtr/",
        logo_src:InstagramLogo,
    },
    {
        name:"Twitter",
        href:"https://twitter.com/rinto_joseph_tr/",
        logo_src:TwitterLogo
    }
    ]
</script>

<section class="profile">
    <img src={Profile} alt="profile" width="140px" height="140px"/>
    <div class="profile-header">
        <h2>Rinto Joseph TR</h2>
        <p>(Big fan of open source)</p>

        <div class="profile-description">
            <p>
                "Loves <span class="highlight">Open-Source </span> development
                and actively adapt to the latest trends in
                <span class="highlight">Web development</span> and related
                fields, constantly exploring new aspects of the web dev world.
                Primarily focused on systems programming languages such as
                <span class="highlight">Rust</span>
                🦀 and <span class="highlight">Go</span> , and a dedicated user
                of <span class="highlight">NeoVim</span>."
            </p>
        </div>
    </div>
    <div class="social-links">
        {#each social_links as link}
            <a href={link.href} target="_blank" >
                <img src={link.logo_src} alt={link.name} width="20px" height="20px"/>
                <span>{link.name}↗</span>
            </a>
        {/each}
    </div>
</section>

<section class="hero-img">
    <canvas bind:this={canvas}></canvas>
</section>

<style>
    .hero-img {
        width: 50%;
        height: 50vh;
    }
    .profile {
        width: 100%;
        display: flex;
        align-items: flex-start;
        justify-content: center;
        flex-direction: column;
        gap: 1.4rem;
    }
    .profile h2 {
        font-size: 2.5rem;
        text-transform: uppercase;
        letter-spacing: 1px;
        color: whitesmoke;
    }

    .profile-header > p {
        font-size: 1.3rem;
        font-weight: bolder;
    }
    .social-links {
        display: flex;
        width: 100%;
        align-items: center;
        justify-content: flex-start;
        gap: 1.5rem;
        font-size: 1.4rem;
        font-weight: 100;
    }

    .social-links span {
        font-size: 1.4rem;
    }

    .social-links a {
        display: flex;
        gap: 0.35rem;
        align-items: center;
    }

    .social-links a:hover {
        text-decoration: underline;
    }

    .social-links img {
        width: 1rem;
        filter: contrast(0.01);
        cursor: pointer;
    }
    .profile > img {
        aspect-ratio: auto 1;
        margin-left: 0.5rem;
        border-radius: 50%;
        border: 2px solid rgb(255, 255, 255);
    }
    /* background-color: #bdafaf; */

    .profile-header {
        width: 100%;
        display: flex;
        flex-direction: column;
        gap: 1.2rem;
    }
    .highlight {
        font-size: 1.8rem;
        font-weight: bolder;
        color: whitesmoke;
        text-align: center;
        letter-spacing: -1.25px;
        -webkit-text-fill-color: transparent;
        background-image: linear-gradient(141deg, #6262f6, #ff568b);
        -webkit-background-clip: text;
        background-clip: text;
    }

    .profile-description {
        width: 90%;
        font-size: 1.5rem;
        line-height: 2.3rem;
    }

    @media (max-width: 745px) {
        .profile {
            top: 10rem;
            width: 25rem;
        }
        .profile h2 {
            font-size: 1.5rem;
        }
    }
</style>
