<script>
    import Background from "../assets/vibrant_oil_painting.png";
    import Profile from "../assets/profile-photo.jpg";
</script>

<img class="background" src={Background} alt="" />
<div class="profile">
    <img src={Profile} alt="profile" />
    <h2>@rintojosephtr</h2>
    <code>Hello!,I'm self taught programmer</code>
</div>

<style>
    .background {
        aspect-ratio: clamp(16/9, 3/4, 5/6);
        width: 100%;
        opacity: 30%;
    }
    .profile {
        position: absolute;
        top: 10rem;
        display: flex;
        flex-direction: column;
        gap: 1rem;
        align-items: center;
        justify-content: space-between;
    }
    .profile h2 {
        letter-spacing: 0.1rem;
        font-size: 2rem;
    }
    .profile img {
        width: 8rem;
        border-radius: 50%;
        border: 2px solid whitesmoke;
    }
    .profile code {
        font-size: 1rem;
        letter-spacing: 0.1rem;
        padding: 0.75rem;
        background-color: #ffffff14;
        backdrop-filter: blur(10px);
        border-radius: 0.55rem;
    }

    @media (max-width: 745px) {
        .background {
            height: 30rem;
        }
        .profile img {
            width: 6rem;
        }
        .profile {
            top: 5rem;
        }
        .profile h2 {
            font-size: 1.5rem;
        }
        .profile code {
            font-size: 0.8rem;
        }
    }
</style>
