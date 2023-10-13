<script>
  import Logo from "/logo.svg";
  import GithubLogo from "../assets/github.svg";
  import {  Link } from "svelte-routing";
</script>

<nav>
  <img src={Logo} alt="logo" />
  <div class="links">
    <Link to="/">Home</Link>
    <Link to="/projects">Projects</Link>
  </div>

  <span>
    <img src={GithubLogo} alt="github logo" />
    <a href="https://github.com/rinto11804/portfolio" target="_blank">
      Source
    </a>
  </span>
</nav>

<style>
  nav {
    position: sticky;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 1rem;
    gap: 5rem;
    width: 100%;
    z-index: 5;
    backdrop-filter: blur(20px);
    border-bottom: 2px solid #51515123;
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
  span {
    display: flex;
    align-items: center;
    gap: 0.5rem;
    border-radius: 10rem;
    padding: 0.8rem;
  }

  span:hover{
    background-color: #313131;
  }

  .links {
    display: flex;
    align-items: flex-end;
    justify-content: space-evenly;
    gap: clamp(0.1rem, 2rem, 10rem);
    background-color: #313131;
    border-radius: 10rem;
    padding: 5px;
    list-style: none;
  }
  :global(.links a){
      padding: 0.8rem;
  }

  :global(.links a:hover) {
    text-decoration: underline;
    background-color: #414141;
    font-weight: bolder;
    border-radius: 10rem;
  }
  span a{
    font-size: 1.2rem;
    font-weight: bolder;
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
