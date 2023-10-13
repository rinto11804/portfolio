<script>
    import GithubLogo from "../assets/github.svg";
    import KanbanBoardImg from "../assets/kanban-board.png";
    import LomusicImg from "../assets/lomusic.png";
</script>

<section>
    <h1>Projects</h1>
    <div class="projects">
        <div class="project-description">
            <img src={KanbanBoardImg} alt="" class="project-img" />
            <h3>kanban-board-svelte</h3>
            <p>
                A kanban board in which you could drag and drop task using
                sveltejs
            </p>
            <a href="https://github.com/rinto11804/kanban-board-svelte" target="_blank">
                <img src={GithubLogo} alt="github/rinto11804" />
                <span>View Source↗</span>
            </a>
        </div>

        <div class="project-description">
            <img src={LomusicImg} alt="" class="project-img" />
            <h3>lomusic</h3>
            <p>
                A wesite shows recent trending music and discover songs by using
                Spotify Web API
            </p>
            <div>
              <a href="https://github.com/rinto11804/lomusic" target="_blank">
                <img src={GithubLogo} alt="github/rinto11804" />
                <span>View Source↗</span>
            </a>

            <a href="https://lomusic.vercel.app " target="_blank">
                <span>View Demo↗</span>
            </a>   
            </div>
           
            
        </div>

        <div class="project-description">
            <img src="https://aloia-systems.gumlet.io/images/articles/cli-tool-in-go.png?w=640&h=426&s=356207c0e3f77945526ae3eb0c5c225f" alt="" class="project-img" />
            <h3>Libgen CLI</h3>
            <p>
                A command line tool using Go that allow one to download a books from libgen website
            </p>
            <a href="https://github.com/rinto11804" target="_blank">
                <img src={GithubLogo} alt="github/rinto11804" />
                <span>View Source↗</span>
            </a>
        </div>

        <div class="project-description">
            <img src="https://raw.githubusercontent.com/vlang/v-logo/master/dist/v-logo.svg?sanitize=true" alt="" class="project-img" />
            <h3>Gifdl</h3>
            <p>
                A CLI tool using Vlang that allow one to download a gif from internet
            </p>
            <a href="https://github.com/rinto11804/gifdl" target="_blank">
                <img src={GithubLogo} alt="github/rinto11804" />
                <span>View Source↗</span>
            </a>
        </div>
    </div>  
</section>

<style>
    .projects {
        display: flex;
        flex-direction: row;
        align-items: start;
        gap: 4rem;
        justify-content: space-between;
        margin-block: 2rem;
        flex-wrap: wrap;
    }
    .project-description {
        width: fit-content;
        padding: 1rem;
        display: flex;
        flex-direction: column;
        align-items: start;
        justify-content: space-between;
        gap: 1.2rem;
        border: 2px solid #414141;
        border-radius: 0.25rem;
    }
    h1 {
        color: whitesmoke;
        font-size: 2.5rem;
    }
    h3 {
        font-size: 1.8rem;
    }

    .project-img {
        width: 40rem;
        height: 20rem;
        object-fit: contain;
    }
    a{
        margin-right: 0.3rem;
    }

    a img {
        width: 1rem;
        filter: contrast(0.01);
        cursor: pointer;
    }
</style>
