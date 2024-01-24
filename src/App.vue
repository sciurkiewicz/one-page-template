<script setup lang="ts">
</script>

<template>
	<nav id="header" class="fixed bg-black text-white w-full z-20 top-0">
	<div id="progress" class="h-1 z-40 top-0"
		style="background:linear-gradient(to right, #FFC100 var(--scroll), transparent 0);"></div>
	<div class="w-full md:max-w-4xl mx-auto flex flex-wrap items-center justify-between mt-0 py-3">
		<div class="block lg:hidden pl-8 p-2">
			<a class="text-yellow-300 font-bold text-base no-underline hover:no-underline" href="#">
				TechFest
			</a>
		</div>
		<div class="block lg:hidden pr-4">
			<button id="nav-toggle" class="flex items-center px-3 py-2 text-yellow-300 border-gray-600 focus:outline-none">
          <svg fill="text-yellow-300" viewBox="0 0 20 20" class="w-6 h-6 fill-current">
            <title>Menu</title>
            <path fill-rule="evenodd"
              d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM9 15a1 1 0 011-1h6a1 1 0 110 2h-6a1 1 0 01-1-1z"
              clip-rule="evenodd"></path>
          </svg>
        </button>
		</div>
		<div class="w-full flex-grow p-4 lg:flex lg:items-center lg:w-auto hidden lg:block mt-2 lg:mt-0 bg-black md:bg-transparent z-20"
			id="nav-content">
			<ul class="list-reset lg:flex justify-center flex-1 items-center">
				<li class="mr-3">
					<a class="border-b-0 md:border-b-4 border-yellow-300 inline-block py-2 px-4 text-yellow-300 font-bold"
						href="#">Home</a>
				</li>
				<li class="mr-3">
					<a class="inline-block hover:text-yellow-300 hover:text-underline py-2 px-4" href="#">Skills</a>
				</li>
				<li class="mr-3">
					<a class="inline-block hover:text-yellow-300 hover:text-underline py-2 px-4" href="#">Project</a>
				</li>
				<li class="mr-3">
					<a class="inline-block hover:text-yellow-300 hover:text-underline py-2 px-4" href="#">Contact</a>
				</li>
			</ul>
		</div>
	</div>
</nav>
<section>
	<div class="bg-black text-white h-screen align-middle">
		<div class="container mx-auto flex flex-col md:flex-row items-center align-middle flex justify-center items-center h-screen">
			<div class="flex flex-col w-full lg:w-1/3 justify-center items-start p-8">
				<h1 class="text-3xl md:text-5xl mb-3 text-yellow-300 tracking-loose">Szymon Ciurkiewicz</h1>
				<h2 class="text-3xl md:text-5xl leading-relaxed md:leading-snug mb-2">Front-End Developer
				</h2>
				<p class="text-sm md:text-base text-gray-50 mb-4">Explore your favourite events and
					register now to showcase your talent and win exciting prizes.</p>
				<a href="#"
					class="bg-transparent hover:bg-yellow-300 text-yellow-300 hover:text-black rounded shadow hover:shadow-lg py-2 px-4 border border-yellow-300 hover:border-transparent">
					Explore Now</a>
			</div>
			<div class="p-8 mt-12 mb-6 md:mb-0 md:mt-0 ml-0 md:ml-12 lg:w-2/3  justify-center">
				<img class="" src="./assets/logo.png">
			</div>
					</div>
				</div>
	</section>
<section>
	<div class="bg-black text-white py-20 h-screen align-middle">
		<div class="container mx-auto flex flex-col md:flex-row items-center align-middle">
			<div class="py-4 bg-black text-white">

<div class="mx-auto flex flex-col md:flex-row">
	<div class="flex flex-col w-full lg:w-3/5 p-8">
		<h1 class="text-3xl md:text-5xl text-yellow-300 my-4 leading-relaxed md:leading-snug">Skills
		</h1>
		<div class="font-sans text-sm md:text-lg my-2 md:my-4">Our team has put a lot of effort to build this
			website
			and get a platform for people to register for this overall India tech fest. We really appreciate
			each team member's contribution and dedication towards the website.
			Do leave a feedback if you enjoyed being here. <br>
			<p>Regards,</p>
			<p>Team i-GNEz</p>
		</div>
	</div>
</div>


<div class="flex flex-wrap text-center md:text-left px-8 md:px-4 lg:px-8">

	<div class="my-4 px-1 w-1/2 md:w-1/3 lg:w-1/6 overflow-hiddden">
		<div>
			<img class="border-4 border-yellow-300 rounded-full transition duration-500 hover:border-white mx-auto md:mx-0 w-24 md:w-auto"
				src="https://user-images.githubusercontent.com/54521023/152726300-b03e134b-ff5c-40bf-a982-e01d825b4b68.png"
				alt="user-avatar">
			<p class="text-lg mt-4 md:mt-8"><b>User Name</b></p>
			<p class="text-yellow-300">Designation</p>
		</div>
	</div>

	<div class="my-4 px-1 w-1/2 md:w-1/3 lg:w-1/6">
		<div>
			<img class="border-4 border-yellow-300 rounded-full transition duration-500 hover:border-white mx-auto md:mx-0 w-24 md:w-auto"
				src="https://user-images.githubusercontent.com/54521023/152726300-b03e134b-ff5c-40bf-a982-e01d825b4b68.png"
				alt="user-avatar">
			<p class="text-lg mt-4 md:mt-8"><b>User Name</b></p>
			<p class="text-yellow-300">Designation</p>
		</div>
	</div>

	<div class="my-4 px-1 w-1/2 md:w-1/3 lg:w-1/6">
		<div>
			<img class="border-4 border-yellow-300 rounded-full transition duration-500 hover:border-white mx-auto md:mx-0 w-24 md:w-auto"
				src="https://user-images.githubusercontent.com/54521023/152726300-b03e134b-ff5c-40bf-a982-e01d825b4b68.png"
				alt="user-avatar">
			<p class="text-lg mt-4 md:mt-8"><b>User Name</b></p>
			<p class="text-yellow-300">Designation</p>
		</div>
	</div>

	<div class="my-4 px-1 w-1/2 md:w-1/3 lg:w-1/6">
		<div>
			<img class="border-4 border-yellow-300 rounded-full transition duration-500 hover:border-white mx-auto md:mx-0 w-24 md:w-auto"
				src="https://user-images.githubusercontent.com/54521023/152726300-b03e134b-ff5c-40bf-a982-e01d825b4b68.png"
				alt="user-avatar">
			<p class="text-lg mt-4 md:mt-8"><b>User Name</b></p>
			<p class="text-yellow-300">Designation</p>
		</div>
	</div>

	<div class="my-4 px-1 w-1/2 md:w-1/3 lg:w-1/6">
		<div>
			<img class="border-4 border-yellow-300 rounded-full transition duration-500 hover:border-white mx-auto md:mx-0 w-24 md:w-auto"
				src="https://user-images.githubusercontent.com/54521023/152726300-b03e134b-ff5c-40bf-a982-e01d825b4b68.png"
				alt="user-avatar">
			<p class="text-lg mt-4 md:mt-8"><b>User Name</b></p>
			<p class="text-yellow-300">Designation</p>
		</div>
	</div>

	<div class="my-4 px-1 w-1/2 md:w-1/3 lg:w-1/6">
		<div>
			<img class="border-4 border-yellow-300 rounded-full transition duration-500 hover:border-white mx-auto md:mx-0 w-24 md:w-auto"
				src="https://user-images.githubusercontent.com/54521023/152726300-b03e134b-ff5c-40bf-a982-e01d825b4b68.png"
				alt="user-avatar">
			<p class="text-lg mt-4 md:mt-8"><b>User Name</b></p>
			<p class="text-yellow-300">Designation</p>
		</div>
	</div>

</div>
</div>

</div>
</div>
</section>

<section>
	<div class="bg-black text-white py-20 h-screen align-middle">
		<div class="container mx-auto flex flex-col md:flex-row items-center align-middle">
		    <div class="bg-black text-white py-8">
    <div class="container mx-auto flex flex-col items-start md:flex-row my-12 md:my-24">
      <div class="flex flex-col w-full sticky md:top-36 lg:w-1/3 mt-2 md:mt-12 px-8">
			<h1 class="text-3xl md:text-5xl text-yellow-300 my-4 leading-relaxed md:leading-snug">Projects
			</h1>
			<div class="font-sans text-sm md:text-lg my-2 md:my-4">Our team has put a lot of effort to build this
				website
				and get a platform for people to register for this overall India tech fest. We really appreciate
				each team member's contribution and dedication towards the website.
				Do leave a feedback if you enjoyed being here. <br>
				<p>Regards,</p>
				<p>Team i-GNEz</p>
			</div>
			<div class="font-sans text-sm md:text-lg my-2 md:my-4">
				
				<p>Regards,</p>
				<p>Team i-GNEz</p>
			</div>
      </div>
      <div class="ml-0 md:ml-12 lg:w-2/3 sticky">
        <div class="container mx-auto w-full h-full">
          <div class="relative wrap overflow-hidden p-10 h-full">
            <div class="border-2-2 border-yellow-555 absolute h-full border"
              style="right: 50%; border: 2px solid #FFC100; border-radius: 1%;"></div>
            <div class="border-2-2 border-yellow-555 absolute h-full border"
              style="left: 50%; border: 2px solid #FFC100; border-radius: 1%;"></div>
            <div class="mb-8 flex justify-between flex-row-reverse items-center w-full left-timeline">
              <div class="order-1 w-5/12"></div>
              <div class="order-1 w-5/12 px-1 py-4 text-right">
                <p class="mb-3 text-base text-yellow-300">JavaScript/Electron</p>
                <h4 class="mb-3 font-bold text-lg md:text-2xl">Registration</h4>
                <p class="text-sm md:text-base leading-snug text-gray-50 text-opacity-100">
                  Pick your favourite event(s) and register in that event by filling the form corresponding to that
                  event. Its that easy :)
                </p>
              </div>
            </div>
            <div class="mb-8 flex justify-between items-center w-full right-timeline">
              <div class="order-1 w-5/12"></div>
              <div class="order-1  w-5/12 px-1 py-4 text-left">
                <p class="mb-3 text-base text-yellow-300">JavaScript/Electron</p>
                <h4 class="mb-3 font-bold text-lg md:text-2xl">Participation</h4>
                <p class="text-sm md:text-base leading-snug text-gray-50 text-opacity-100">
                  Participate online. The links for your registered events will be sent to you via email and whatsapp
                  groups. Use those links and show your talent.
                </p>
              </div>
            </div>
            <div class="mb-8 flex justify-between flex-row-reverse items-center w-full left-timeline">
              <div class="order-1 w-5/12"></div>
              <div class="order-1 w-5/12 px-1 py-4 text-right">
                <p class="mb-3 text-base text-yellow-300">JavaScript/Electron</p>
                <h4 class="mb-3 font-bold text-lg md:text-2xl">Result Declaration</h4>
                <p class="text-sm md:text-base leading-snug text-gray-50 text-opacity-100">
                  The ultimate genius will be revealed by our judging panel on 10th May, 2021 and the resukts will be
                  announced on the whatsapp groups and will be mailed to you.
                </p>
              </div>
            </div>

            <div class="mb-8 flex justify-between items-center w-full right-timeline">
              <div class="order-1 w-5/12"></div>

              <div class="order-1  w-5/12 px-1 py-4">
                <p class="mb-3 text-base text-yellow-300">JavaScript/Electron</p>
                <h4 class="mb-3 font-bold  text-lg md:text-2xl text-left">Prize Distribution</h4>
                <p class="text-sm md:text-base leading-snug text-gray-50 text-opacity-100">
                  The winners will be contacted by our team for their addresses and the winning goodies will be sent at
                  their addresses.
                </p>
              </div>
            </div>
          </div>
          <img class="mx-auto -mt-36 md:-mt-36" src="https://user-images.githubusercontent.com/54521023/116968861-ef21a000-acd2-11eb-95ac-a34b5b490265.png" />
        </div>
      </div>
    </div>
  </div>	
</div>
</div>
</section>



</template>

<style>
html {
	background-color: black;
}
</style>