<script>
    import Profile from '$lib/img/linkedin_profile.jpeg';
    import Social from '$lib/social/Social.svelte';
</script>

<section id="about" class="pb-24">
	<div class="max-w-6xl mx-auto px-6">
            <section class="bg-white">
                <div class="container py-8 mx-auto">
                    <div class="items-center lg:grid lg:grid-cols-3">
                        <div class="lg:col-span-2 lg:mr-24">
                            <h2 class="text-3xl font-semibold text-gray-800">Who I am</h2>
    
                            <p class="text-gray-500 my-5 text-justify">
                                I am a Data Scientist and Data Analyst based in Sonoma County, California. I have a master’s degree and over five years experience providing actionable insights. I have a diverse background working in both public and private sectors from research to marketing which gives me a unique eye in which to approach your data-driven questions.
                            </p>

                            <p class="text-gray-500 mt-3">I look forward to hearing about how I can help you solve your data questions!
                            </p>
        
                            <Social />
                        </div>
        
                        <div class="mt-8 lg:col-span-1">
                            <div class="flex items-center justify-center lg:justify-end">
                                <div class="max-w-lg">
                                    <!-- <img class="object-cover object-center w-full h-64 rounded-md shadow" src="https://images.unsplash.com/photo-1484399172022-72a90b12e3c1?ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=1500&q=80" alt=""> -->

                                    <img src="https://rshogan.imgix.net/clients/jessicahogama/IMG-2649_cropped_2.jpg?auto=compress,format" alt="" class="object-contain h-96 w-full rounded-xl" />
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </section>
    </div>
</section>