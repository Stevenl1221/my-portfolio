<script>
    const projects = [
        {
            name: "Project 1",
            image: "https://images.unsplash.com/photo-1576153192396-180ecef2a715?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1374&q=80"
        },
        {
            name: "Project 2",
            image: "https://images.unsplash.com/photo-1545235617-9465d2a55698?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=880&q=80"
        },
        {
            name: "Project 3",
            image: "https://images.unsplash.com/photo-1586717791821-3f44a563fa4c?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1470&q=80"
        }
    ];
</script>

<div class="py-10 container mt-40 flex justify-between items-center mx-auto px-8 md:px-14 lg:px-24 w-full" id="projects">
    <section class="w-full text-center">
        <h2 id="work" class="secondary-title md:text-left text-4xl font-bold mb-6">Portfolio</h2>
        <p class="section-paragraph md:text-left text-gray-500">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ullamcorper
            nulla nunc quis molestie volutpat elementum at. Ultrices ipsum, enim
            cursus lorem ac. Orci maecenas praesent arcu eget orci est orci
            nullam. Leo purus est pellentesque massa at tortor, est. Aliquet
            pulvinar a mattis sagittis. Suspendisse porta id elementum, massa.
        </p>
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6 mt-6">
            {#each projects as project}
                <div class="img-wrapper relative overflow-hidden">
                    <img class="h-full w-full object-cover rounded" src={project.image}
                        alt=""
                    />
                    <div class="img-overlay w-full h-full absolute top-0 z-10 after:w-full after:rounded after:h-full after:absolute after:top-0 after:left-0 after:opacity-0 after:bg-black">
                        <h2 class="img__title relative mb-8 my-16 text-4xl font-Oswald font-thin text-white text-center transition duration 0.3s ease-in-out tracking-wider">{project.name}</h2>
                        <a class="img__link relative block w-3/5 p-2.5 font-Montserrat font-medium text-white no-underline hover:bg-secondary text-center text-base border-solid border-2 border-white tracking-wider mx-auto transition duration 0.3 ease-in-out hover:text-gray-50" href="#">View Case Study</a>
                    </div>
                </div>
            {/each}
        </div>
    </section>
</div>

<style global lang="postcss">
    .img-overlay {
        width: 100%;
        height: 100%;
    }
    .img-overlay:after {
        content: "";
        z-index: -10;
        transition: all 0.3s ease;
    }
    .img__title {
        top: -200px;
    }
    .img__link {
        top: 200px;
    }
    .img-wrapper:hover .img__title {
        top: 0;
    }
    .img-wrapper:hover .img__link {
        top: 0;
    }
    .img-wrapper:hover .img-overlay:after {
        opacity: 0.75;
    }
</style>