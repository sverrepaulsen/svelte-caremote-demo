<script>
    let cards = [
        {
            src: "https://www.birmingham.ac.uk/images/news/diabetes-720.jpg",
            title: "Diabetes Type 1",
            description: "Diabetes Type 1 Information Blob"
        },
        {
            src: "https://www.drholdright.co.uk/wp-content/uploads/2019/12/blood_pressure.png",
            title: "Hypertension",
            description: "Hypertension Information Blob"
        },
        {
            src: "https://img.huffingtonpost.com/asset/582c96f81500001800b0d5a5.jpg?ops=scalefit_720_noupscale",
            title: "Diabetes Type 2",
            description: "Diabetes Type 2 Information Blob"
        },
        {
            src: "https://cdn.sanity.io/images/0vv8moc6/infenctioncontrol/ffec4b4e00b687598729b7678a0a3e0108c7275b-720x480.jpg",
            title: "Disease 4",
            description: "Disease 4 Information Blob"
        },
        {
            src: "https://cdn.sanity.io/images/0vv8moc6/infenctioncontrol/ffec4b4e00b687598729b7678a0a3e0108c7275b-720x480.jpg",
            title: "Disease 5",
            description: "Disease 5 Information Blob"
        },
        {
            src: "https://cdn.sanity.io/images/0vv8moc6/infenctioncontrol/ffec4b4e00b687598729b7678a0a3e0108c7275b-720x480.jpg",
            title: "Disease 6",
            description: "Disease 6 Information Blob"
        },
    ]
</script>

<div>
    <div 
        class="w-full relative  bg-center"
        style="background-image: url('https://www.riverbrook.ie/river/wp-content/uploads/2019/10/tender-caregiver-saying-goodbye-1060x707.jpg')"
    >
        <div class="flex flex-col w-full bg-white items-center p-2">
            <button class="bg-white text-blue-800 hover:bg-purple-700 hover:text-white font-bold py-2 px-4 rounded w-72">
                Search Codes
            </button>
        </div>
        <div class="bg-black text-purple-500 pt-56 px-12 pb-10 w-[400px] h-full">
            <h1 class="font-bold text-4xl pb-5">
                Banner Header
            </h1>
            <h5 class="mt-2 font-medium text-2xl pb-10">
                Banner Main Text
            </h5>
            <button class="bg-purple-700 text-white mt-5 font-semibold hover:bg-white hover:text-blue-800 rounded py-2 px-4 w-72">
                Create Disease Configuration
            </button>
        </div>
    </div>
    <div class="flex flex-wrap p-8 items-center justify-center">
        {#each cards as card}
            <div class="mb-10 mx-10 rounded-xl overflow-hidden shadow-xl transition-transform ease-in cursor-pointer hover:scale-110 w-96">
                <img class="object-fill min-w-[300px] min-h-[200px] w-full" src={card.src} alt="">
                <div class="-mt-2 rounded-xl p-2 pt-5">
                    <h2 class="text-lg font-semibold">{card.title}</h2>
                    <h4 class="text-sm font-light my-2">{card.description}</h4>
                </div>
            </div>
        {/each}
    </div>
</div>