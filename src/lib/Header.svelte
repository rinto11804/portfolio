<script>
    import Profile from "../assets/profile-photo.jpg";
    import GithubLogo from "../assets/github.svg";
    import LinkedinLogo from "../assets/linkedin.svg";
    import InstagramLogo from "../assets/instagam.svg";
    import TwitterLogo from "../assets/twitter.svg";
</script>

<section class="profile">
    <img src={Profile} alt="profile" />
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
        <a href="https://github.com/rinto11804" target="_blank">
            <img src={GithubLogo} alt="github/rinto11804" />
            <span>Github↗</span>
        </a>
        <a
            href="https://www.linkedin.com/in/rinto-joseph-t-r-a0921225a/"
            target="_blank"
            rel="linkedin/rintojosephtr"
        >
            <img src={LinkedinLogo} alt="linkedin" />
            <span>Linkedin↗</span>
        </a>

        <a
            href="https://www.instagram.com/rinto_josephtr/"
            target="_blank"
            rel="instagram/rinto_josephtr"
        >
            <img src={InstagramLogo} alt="instagram" />

            <span>Instagram↗</span>
        </a>

        <a
            href="https://twitter.com/rinto_joseph_tr/"
            target="_blank"
            rel="twitter/rinto_josephtr"
        >
            <img src={TwitterLogo} alt="twitter" />
            <span>Twitter↗</span>
        </a>
    </div>
</section>

<style>
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
        width: 8rem;
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
        width: 50%;
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
