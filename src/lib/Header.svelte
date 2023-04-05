<script>
    import Profile from "../assets/profile-photo.jpg";
    import GithubLogo from "../assets/github.svg";
    import LinkedinLogo from "../assets/linkedin.svg";
    import InstagramLogo from "../assets/instagam.svg";
</script>

<div class="profile">
    <div class="social-links">
        <a href="https://github.com/rinto11804" target="_blank">
            <img src={GithubLogo} alt="github/rinto11804" />
        </a>
        <a
            href="https://www.linkedin.com/in/rinto-joseph-t-r-a0921225a/"
            target="_blank"
            rel="linkedin/rintojosephtr"
        >
            <img src={LinkedinLogo} alt="" />
        </a>

        <a
            href="https://www.instagram.com/rinto_josephtr/"
            target="_blank"
            rel="instagram/rinto_josephtr"
        >
            <img src={InstagramLogo} alt="" />
        </a>
    </div>
    <img src={Profile} alt="profile" />
    <h2>Hello👋,I'm rinto</h2>
    <code>I'm a self taught programmer</code>
</div>

<style>
    .profile {
        position: absolute;
        top: 10rem;
        height: 20rem;
        display: flex;
        flex-direction: column;
        gap: 0.7rem;
        align-items: center;
        justify-content: space-evenly;
        padding: 1rem;
        border: 2px solid #ffffff14;
        border-radius: 0.65rem;
        z-index: 2;
        box-shadow: 2px 2px 10px #242424c2;
    }
    .profile h2 {
        letter-spacing: 0.1rem;
        font-size: 1.7rem;
    }
    .social-links {
        display: flex;
        width: 100%;
        justify-content: flex-end;
        gap: 1.5rem;
    }
    .social-links img {
        width: 1rem;
        filter: contrast(0.01);
        cursor: pointer;
    }
    .profile > img {
        width: 8rem;
        border-radius: 50%;
        border: 2px solid whitesmoke;
        filter: grayscale(10);
    }
    /* background-color: #bdafaf; */

    .profile code {
        font-size: 1rem;
        letter-spacing: 0.2rem;
        font-weight: 800;
        padding: 0.75rem;
        background-color: #f3eded14;
        backdrop-filter: blur(10px);
        font-weight: lighter;
        border-radius: 0.55rem;
        border: 2px solid #ece9e914;
    }

    @media (max-width: 745px) {
        .profile {
            top: 10rem;
            width: 25rem;
        }
        .profile h2 {
            font-size: 1.5rem;
        }
        .profile code {
            font-size: 0.9rem;
            font-weight: lighter;
            text-align: center;
        }
    }
</style>
