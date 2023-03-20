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
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-2 gap-24 mt-6">
            <div class="img-wrapper relative overflow-hidden">
                <img class="h-full w-full object-cover rounded" src={projects[0].image} alt="" />
            </div>
            <div>
                <h5 class="text-xl font-extrabold mb-4 uppercase">Workout Web App</h5>
                <h6 class="font-semibold">A social workout web app that allows users to create, share, like, and comment on each others’ workout templates and profiles. Users can find new workout exercises by searching or sorting by popularity and muscle group.</h6>
                <div class="mt-2">
                    <span class="badge">Express.js</span>
                    <span class="badge">MongoDB</span>
                    <span class="badge">Axios</span>
                    <span class="badge">Git</span>
                </div>
                <div class="flex justify-center gap-4 mt-6 text-xl">
                    <a target="_blank" href="https://github.com/Stevenl1221/WorkoutApplication" rel="noreferrer">Code <i class="fa-brands fa-github"></i></a>
                </div>
            </div>
            <div>
                <h5 class="text-xl font-extrabold mb-4 uppercase">AS Software</h5>
                <h6 class="font-semibold">A website to display products and testimonials of a leading provider of ultrasound reporting and image management. Customers can contact and find a partner at AS Software</h6>
                <div class="mt-2">
                    <span class="badge">HTML</span>
                    <span class="badge">CSS</span>
                    <span class="badge">JavaScript</span>
                    <span class="badge">Bootstrap</span>
                </div>
                <div class="flex justify-center gap-4 mt-6 text-xl">
                    <a target="_blank" href="https://github.com/Stevenl1221/assoftwarre" rel="noreferrer">Code <i class="fa-brands fa-github"></i></a>
                    <a target="_blank" href="https://stevenl1221.github.io/assoftwarre/index.html" rel="noreferrer">Live Demo <i class="fa-solid fa-arrow-up-right-from-square link-icon"></i></a>
                </div>
            </div>
            <div class="img-wrapper relative overflow-hidden">
                <img class="h-full w-full object-cover rounded" src={projects[1].image} alt="" />
            </div>
            <div class="flex w-full relative justify-center h-4/5">
                <img class="h-3/5 rounded" src={projects[2].image} alt="" />
            </div>
            <div>
                <h5 class="text-xl font-extrabold mb-4 uppercase">Weather App</h5>
                <h6 class="font-semibold">A mobile app for both IOS and Android to display weather data including forecasts and nowcasts. The weather app displays current weather, hourly weather, and daily weather data with minimalistic UI. It also displays precipitation, wind speed, and humidity. Unique icons for each type of weather, day, and night. </h6>
                <div class="mt-2">
                    <span class="badge">Flutter</span>
                    <span class="badge">GetX</span>
                    <span class="badge">OpenWeatherAPI</span>
                </div>
                <div class="flex justify-center gap-4 mt-6 text-xl">
                    <a target="_blank" href="https://github.com/Stevenl1221/WeatherApp" rel="noreferrer">Code <i class="fa-brands fa-github"></i></a>
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