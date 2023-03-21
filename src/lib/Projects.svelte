<script>
    import WorkoutImg from "../assets/workout.png";
    import ASSoftwareImg from "../assets/assoftware.png";
    import WeatherAppImg from "../assets/weatherapp.png";
    const projects = [
        {
            name: "Project 1",
            image: WorkoutImg
        },
        {
            name: "Project 2",
            image: ASSoftwareImg
        },
        {
            name: "Project 3",
            image: WeatherAppImg
        }
    ];
</script>

<div class="py-10 container mt-40 flex justify-between items-center mx-auto px-8 md:px-14 lg:px-24 w-full" id="projects">
    <section class="w-full h-full text-center">
        <h2 id="work" class="md:text-left text-xl font-black mb-6 uppercase text-emerald-300">Portfolio</h2>
        <h3 class="md:text-left text-4xl mb-10 font-bold">some projects i have worked on !</h3>
        <!-- <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6 mt-6">
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
        </div> -->
        <div class="grid grid-cols-1 md:grid-cols-1 lg:grid-cols-1 gap-24 mt-6">
            <div class="rounded bg-slate-800 flex h-160 w-full shadow-[0px_22px_70px_4px_rgba(0,0,0,0.56)] gap-28 p-10 ">
                <div class="img-wrapper">
                    <img class="h-auto w-212 object-cover rounded" src={projects[0].image} alt="" />
                </div>
                <div class="flex-col justify-center">
                    <h5 class="text-xl font-extrabold mb-4 uppercase">Workout Web App</h5>
                    <h6 class="font-semibold">A social workout web app that allows users to create, share, like, and comment on each others’ workout templates and profiles. Users can search or sort by popularity and muscle group.</h6>
                    <div class="mt-2">
                        <span class="badge">MongoDB</span>
                        <span class="badge">Express.js</span>
                        <span class="badge">Node.js</span>
                        <span class="badge">Axios</span>
                        <span class="badge">Git</span>
                    </div>
                    <div class="flex justify-center gap-4 mt-6 text-xl">
                        <a class="text-white font-extrabold" target="_blank" href="https://github.com/Stevenl1221/WorkoutApplication" rel="noreferrer">Code <i class="fa-brands fa-github"></i></a>
                    </div>
                </div>
            </div>
            <div class="rounded bg-slate-800 flex flex-row-reverse h-160 w-full shadow-[0px_22px_70px_4px_rgba(0,0,0,0.56)] gap-32 p-10">
                <div class="img-wrapper">
                    <img class="h-auto w-212 object-cover rounded" src={projects[1].image} alt="" />
                </div>
                <div class="flex-col justify-center">
                    <h5 class="text-xl font-extrabold mb-4 uppercase">AS Software</h5>
                    <h6 class="font-semibold">A website to display products and testimonials of a leading provider of ultrasound reporting and image management. Customers can contact and find a partner at AS Software</h6>
                    <div class="mt-2">
                        <span class="badge">HTML</span>
                        <span class="badge">CSS</span>
                        <span class="badge">JavaScript</span>
                        <span class="badge">Bootstrap</span>
                    </div>
                    <div class="flex justify-center gap-4 mt-6 text-xl">
                        <a class="text-white font-extrabold" target="_blank" href="https://github.com/Stevenl1221/assoftwarre" rel="noreferrer">Code <i class="fa-brands fa-github"></i></a>
                        <a class="text-white font-extrabold" target="_blank" href="https://stevenl1221.github.io/assoftwarre/index.html" rel="noreferrer">Live Demo <i class="fa-solid fa-arrow-up-right-from-square link-icon"></i></a>
                    </div>
                </div>
            </div>
            <div class="rounded bg-slate-800 flex h-auto w-full shadow-[0px_22px_70px_4px_rgba(0,0,0,0.56)] gap-32 p-10">
                <div class="relative justify-center">
                    <img class="h-auto w-212 ml-16 object-cover rounded" src={projects[2].image} alt="" />
                </div>
                <div class="flex-col justify-center ml-16">
                    <h5 class="text-xl font-extrabold mb-4 uppercase">Weather App</h5>
                    <h6 class="font-semibold">A mobile app for me to learn both IOS and Android development that display weather data including forecasts and nowcasts. The weather app displays current weather, hourly weather, and daily weather data with minimalistic UI. It also displays precipitation, wind speed, and humidity. Unique icons for each type of weather, day, and night. </h6>
                    <div class="mt-2">
                        <span class="badge">Flutter</span>
                        <span class="badge">GetX</span>
                        <span class="badge">OpenWeatherAPI</span>
                    </div>
                    <div class="flex justify-center gap-4 mt-6 text-xl">
                        <a class="text-white font-extrabold" target="_blank" href="https://github.com/Stevenl1221/WeatherApp" rel="noreferrer">Code <i class="fa-brands fa-github"></i></a>
                    </div>
                </div>
            </div>
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

<!-- <script>
    import WorkoutImg from "../assets/workout.png";
    import ASSoftwareImg from "../assets/assoftware.png";
    import WeatherAppImg from "../assets/weatherapp.png";
    
    const projects = [
        {
            name: "Workout Web App",
            description: "A social workout web app that allows users to create, share, like, and comment on each others’ workout templates and profiles. Users search or sort by popularity and muscle group.",
            technologies: ["MongoDB", "Express.js", "Node.js", "Axios", "Git"],
            image: WorkoutImg,
            githubLink: "https://github.com/Stevenl1221/WorkoutApplication"
        },
        {
            name: "AS Software",
            description: "A website to display products and testimonials of a leading provider of ultrasound reporting and image management. Customers can contact and find a partner at AS Software",
            technologies: ["HTML", "CSS", "JavaScript", "Bootstrap"],
            image: ASSoftwareImg,
            githubLink: "https://github.com/Stevenl1221/assoftwarre",
            liveDemoLink: "https://stevenl1221.github.io/assoftwarre/index.html"
        },
        {
            name: "Weather App",
            description: "A mobile app for me to learn both IOS and Android development that display weather data including forecasts and nowcasts. The weather app displays current weather, hourly weather, and daily weather data with minimalistic UI. It also displays precipitation, wind speed, and humidity. Unique icons for each type of weather, day, and night.",
            technologies: ["Flutter", "GetX", "OpenWeatherAPI"],
            image: WeatherAppImg,
            githubLink: "https://github.com/Stevenl1221/WeatherApp"
        }
    ];
</script>

<div class="py-10 container mx-auto px-4 md:px-8 lg:px-24" id="projects">
    <h2 class="text-center md:text-left text-3xl md:text-4xl font-bold text-emerald-300 uppercase tracking-wider mb-6">Portfolio</h2>
    <h3 class="text-center md:text-left text-xl font-semibold mb-10">some projects i have worked on!</h3>
    <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
        {#each projects as project}
            <div class="bg-slate-800 rounded overflow-hidden shadow-lg">
                <div class="h-56 md:h-64 bg-cover bg-center" style="background-image: url('{project.image}')"></div>
                <div class="p-6 md:p-8">
                    <h4 class="text-xl md:text-2xl font-semibold mb-4">{project.name}</h4>
                    <p class="text-gray-400 text-sm md:text-base mb-4">{project.description}</p>
                    <div class="flex flex-wrap">
                        {#each project.technologies as technology}
                            <span class="text-gray-400 text-sm md:text-base bg-gray-700 rounded-full py-1 px-3 mr-2 mb-2">{technology}</span>
                        {/each}
                    </div>
                    <div class="mt-6 flex justify-between">
                        <a class="text-white text-xl md:text-2xl font-semibold hover:underline" target="_blank" href="{project.githubLink}" rel="noreferrer">Code <i class="fab fa-github ml-2"></i></a>
                        {#if project.liveDemoLink}
                            <a class="text-white text-xl md:text-2xl font-semibold hover:underline" target="_blank" href="{project.liveDemoLink}" rel="noreferrer">Live Demo <i class="fas fa-external-link-alt ml-2"></i></a>
                        {/if}
                    </div>
                </div>
            </div>
        {/each}
    </div>
</div> -->