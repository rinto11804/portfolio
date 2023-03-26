<script>
  import Logo from "/logo.svg";
  import GithubLogo from "../assets/github.svg";
</script>

<nav>
  <img src={Logo} alt="logo" />
  <div class="links">
    <a href="#home">Home</a>
    <a href="#works">Works</a>
    <span>
      <img src={GithubLogo} alt="github logo" />
      <a href="#source"> Source </a>
    </span>
  </div>
</nav>

<style>
  nav {
    position: fixed;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 1rem;
    background-color: #2e2e2eab;
    gap: 5rem;
    width: 100%;
    z-index: 5;
    backdrop-filter: blur(20px);
  }
  img {
    width: 2rem;
    background-color: aliceblue;
    border-radius: 0.3rem;
    padding: 0.2rem;
  }
  span img {
    width: 1.4rem;
    border-radius: 50%;
  }
  .links span {
    display: flex;
    align-items: center;
    gap: 0.5rem;
  }

  .links {
    display: flex;
    align-items: flex-end;
    justify-content: space-evenly;
    gap: clamp(0.1rem, 5rem, 10rem);
    list-style: none;
  }

  @media (max-width: 745px) {
    span img {
      width: 1.2rem;
    }
    .links {
      font-size: 0.8rem;
      gap: 3rem;
    }
  }
</style>
