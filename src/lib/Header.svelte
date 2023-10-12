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
        <h2>Rinto Joseph T R</h2>
        <p>(Big fan of open source)</p>

        <div class="profile-description">
            <p>
                "Loves <span class="highlight">Open Source</span> dev and
                contribution. Always try to adapt with new things in
                <span class="highlight">Web Development</span>
                and try new things to web dev world. Mostly into systems programming
                language such as
                <span class="highlight">Rust 🦀</span>
                programming language , <span class="highlight">Go</span>
                programming language etc.And a
                <span class="highlight">Neo(Vim)</span> user"
            </p>
        </div>
    </div>
    <div class="social-links">
        <a href="https://github.com/rinto11804" target="_blank">
            <img src={GithubLogo} alt="github/rinto11804" />
            Github
        </a>
        <a
            href="https://www.linkedin.com/in/rinto-joseph-t-r-a0921225a/"
            target="_blank"
            rel="linkedin/rintojosephtr"
        >
            <img src={LinkedinLogo} alt="linkedin" />
            <span>Linkedin</span>
        </a>

        <a
            href="https://www.instagram.com/rinto_josephtr/"
            target="_blank"
            rel="instagram/rinto_josephtr"
        >
            <img src={InstagramLogo} alt="instagram" />
            <span>Instagram</span>
        </a>

        <a
            href="https://twitter.com/rinto_joseph_tr/"
            target="_blank"
            rel="twitter/rinto_josephtr"
        >
            <img src={TwitterLogo} alt="twitter" />
            <span>Twitter</span>
        </a>
    </div>
</section>

<style>
    .profile {
        position: absolute;
        top: 10rem;
        height: 20rem;
        min-width: 25rem;
        display: flex;
        flex-direction: column;
        gap: 1.4rem;
        z-index: 2;
    }
    .profile h2 {
        font-size: 2.5rem;
        color: whitesmoke;
    }

    .profile-header > p {
        font-size: 1.3rem;
        font-weight: bolder;
    }
    .social-links {
        font-size: 1.5rem;
        display: flex;
        width: 100%;
        align-items: center;
        justify-content: flex-start;
        gap: 1.5rem;
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
        width: 10rem;
        border-radius: 50%;
        border: 2px solid rgb(255, 255, 255);
    }
    /* background-color: #bdafaf; */

    .profile-header {
        display: flex;
        flex-direction: column;
        gap: 0.5rem;
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
        line-height: 2rem;
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
