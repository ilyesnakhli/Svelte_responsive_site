<script>
	function burger()
	{
		if(menu.classList.contains('hidden'))
		{
			menu.classList.remove('hidden');
		}
		else{
			menu.classList.add('hidden');
		}
	}
	import Nav from "../src/components/nav.svelte";
	import n from "../src/test.svelte"
</script>



<style>
	
</style>

<body class="text-gray-600 font-sans">
	<div class="grid md:grid-cols-3">
		<div class="md:col-span-1 md:flex md:justify-end">
			<nav class="text-right">
				<div class="flex items-center">
					<h1 class="font-bold uppercase p-4 border-b border-gray-200 animate-bounce">
						<a href="#" class="hover:text-gray-800 cursor-pointer ">
							Hot Pizzas 
						</a>
					</h1>
					<div class="px-4 cursor-pointer md:hidden" id="burger" on:click={burger}>
						<svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
							<path stroke-linecap="round" stroke-linejoin="round" d="M4 6h16M4 12h16M4 18h16" />
						  </svg>
					</div>
				</div>
				<ul class="text-sm mt-6 pl-40 hidden md:block flex justify-right" id="menu">
					<li class="text-gray-700 font-bold py-1">
						<a href="#" class="px-4 flex justify-end border-r-4 border-red-600">
							<span>Home</span>
							<svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-5 ml-2" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
								<path stroke-linecap="round" stroke-linejoin="round" d="M3 12l2-2m0 0l7-7 7 7M5 10v10a1 1 0 001 1h3m10-11l2 2m-2-2v10a1 1 0 01-1 1h-3m-6 0a1 1 0 001-1v-4a1 1 0 011-1h2a1 1 0 011 1v4a1 1 0 001 1m-6 0h6" />
							  </svg>
						</a>
					</li>
					<li class="py-1">
						<a href="#" class="px-4 flex justify-end border-r-4 border-white">
							<span>About</span>
							<svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-5 ml-2" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
								<path stroke-linecap="round" stroke-linejoin="round" d="M8.228 9c.549-1.165 2.03-2 3.772-2 2.21 0 4 1.343 4 3 0 1.4-1.278 2.575-3.006 2.907-.542.104-.994.54-.994 1.093m0 3h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z" />
							  </svg>
						</a>
					</li>
					<li class="py-1">
						<a href="#" class="px-4 flex justify-end border-r-4 border-white">
							<span>Contact</span>
							<svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 ml-2" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
								<path stroke-linecap="round" stroke-linejoin="round" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
							  </svg>
						</a>
					</li>
				</ul>
			</nav>
		</div>
		<main class="px-16 py-6 bg-gray-100 col-span-2"> 
			<div class="flex justify-center md:justify-end">
				<a href="#" class="btn text-red-500  border-primary md:border-2 border-red-600 hover:bg-red-400 hover:text-white transition ease-out duration-500">Log in</a>
				<a href="#" class="btn text-red-500 bg-b ml-2 border-primary md:border-2 border-red-600 hover:bg-red-400 hover:text-white transition ease-out duration-500">sign up</a>
			</div>

			
			<header>
				<h2 class="text-gray-700 text-5xl font-medium mt-5 mb-5">Recipies</h2>
				<h3 class="text-2xl font-medium">For ninjas</h3>
			</header>
			<div>
				<h4 class="font-bold mt-12 pb-2 border-b border-gray-200">Latest Recipies</h4>
				<div class="mt-8 grid lg:grid-cols-3 gap-10">
					<div class="card hover:shadow-xl">
						<img src="img/1.jpg" alt="app" class="w-full h-32 sm:h-48 object-cover" href="/img1.svelte">
						<div class="m-4">
							<span class="font-bold">5 Bean Chili Stew</span>
							<span class="block text-gray-500 text-sm">Recipie By Mario</span>
							
							<Nav/>
						</div>
						<div class="badge">
							<svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-5 inline-block animate-spin" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
								<path stroke-linecap="round" stroke-linejoin="round" d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z" />
							  </svg> 
							<span class="">25 mins</span>
						</div>
					</div>

					<div class="card hover:shadow-xl">
						<img src="img/2.jpg" alt="noodles" class="w-full h-32 sm:h-48 object-cover ">
						<div class="m-4">
							<span class="font-bold">Veg noodles</span>
							<span class="block text-gray-500 text-sm">Recipie By Mario</span>
						</div>
						<div class="badge">
							<svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-5 inline-block animate-spin" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
								<path stroke-linecap="round" stroke-linejoin="round" d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z" />
							  </svg> 

							<span class="">25 mins</span>
						</div>
					</div>

					<div class="card hover:shadow-xl">
						<img src="img/3.jpg" alt="Curry" class="w-full h-32 sm:h-48 object-cover">
						<div class="m-4">
							<span class="font-bold">Tofu Curry</span>
							<span class="block text-gray-500 text-sm">Recipie By Mario</span>
						</div>
						<div class="badge">
							<svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-5 inline-block animate-spin" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
								<path stroke-linecap="round" stroke-linejoin="round" d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z" />
							  </svg>
							<span class="">25 mins</span>
						</div>
					</div>
				</div>
				<h4 class="font-bold mt-12 pb-2 border-b border-gray-200">Most Popular</h4>
				<div class="mt-8">

				</div>
			<div class="flex justify-center">
				<div class="btn bg-gray-400 text-gray-700 hover:shadow-inner transform hover:scale-125 hover:bg-opacity-50 transition ease-out duration-300">
					Load More
				</div>
			 </div>
			</div>
		</main>
	</div>
</body>