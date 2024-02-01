<script setup lang="ts">
  import { ref } from 'vue'

const progress = ref(null)

window.addEventListener('DOMContentLoaded', function() {
  progress.value = document.getElementById('progress')
  if (progress.value) {
	window.addEventListener('scroll', function() {
	  const windowHeight = window.innerHeight
	  const fullHeight = document.documentElement.scrollHeight
	  const scrollTop = window.pageYOffset || document.documentElement.scrollTop
	  const scrollPercent = (scrollTop / (fullHeight - windowHeight)) * 100

	  progress.value.style.setProperty('--scroll', scrollPercent + '%')
	})
  }
})

function openMailApplication() {
  window.location.href = 'mailto:email@example.com'
}
</script>

<template>
	<nav id="header" class="fixed bg-black text-white w-full z-20 top-0">
	<div id="progress" class="h-1 z-40 top-0" style="background:linear-gradient(to right, #FFC100 var(--scroll), transparent 0);"></div>
	<div class="w-full md:max-w-4xl mx-auto flex flex-wrap items-center justify-between mt-0 py-3">
		<div class="block lg:hidden pl-8 p-2">
			<a class="text-yellow-300 font-bold text-base no-underline hover:no-underline" href="#">
				Szymon Ciurkiewicz
			</a>
		</div>
		<div class="block lg:hidden pr-4">
			<button id="nav-toggle" class="flex items-center px-3 py-2 text-yellow-300 border-gray-600 focus:outline-none">
          <!-- <svg fill="text-yellow-300" viewBox="0 0 20 20" class="w-6 h-6 fill-current">
            <title>Menu</title>
            <path fill-rule="evenodd"
              d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM9 15a1 1 0 011-1h6a1 1 0 110 2h-6a1 1 0 01-1-1z"
              clip-rule="evenodd"></path>
          </svg> -->
        </button>
		</div>
		<div class="w-full flex-grow p-4 lg:flex lg:items-center lg:w-auto hidden lg:block mt-2 lg:mt-0 bg-black md:bg-transparent z-20"
			id="nav-content">
			<ul class="list-reset lg:flex justify-center flex-1 items-center">
				<!-- <li class="mr-3">
					<a class="inline-block hover:text-yellow-300 hover:text-underline py-2 px-4 active:" href="#">Home</a>
				</li> -->
				<li class="mr-3">
					<a class="inline-block hover:text-yellow-300 hover:text-underline py-2 px-4 active:" href="#skills">Skills</a>
				</li>
				<li class="mr-3">
					<a class="inline-block hover:text-yellow-300 hover:text-underline py-2 px-4 active:" href="#projects">Projects</a>
				</li>
				<li class="mr-3">
					<a class="inline-block hover:text-yellow-300 hover:text-underline py-2 px-4 active:" href="#contact">Contact</a>
				</li>
			</ul>
		</div>
	</div>
</nav>
<section>
	<div class="bg-black text-white h-screen align-middle">
		<div class="container mx-auto flex flex-col md:flex-row items-center align-middle flex justify-center items-center h-screen">
			<div class="flex flex-col w-full lg:w-1/3 justify-center items-start p-8">
				<h1 class="text-3xl md:text-8xl mb-3 text-yellow-300 tracking-loose " style="font-weight: 700">Szymon Ciurkiewicz</h1>
				<h2 class="text-3xl md:text-3xl leading-relaxed md:leading-snug mb-2" >Front-End Developer
				</h2>
				<p class="text-sm md:text-base text-gray-50 mb-4">I'm passionate about cutting-edge, pixel-perfect, beautiful interfaces and intuitively implemented UX. </p>
				<a href="#contact" class="mt-5 relative h-[50px] w-40 rounded overflow-hidden border border-yellow-300 bg-black text-yellow-300 shadow-2xl transition-all before:absolute before:left-0 before:top-0 before:h-full before:w-0 before:duration-500 after:absolute after:right-0 after:top-0 after:h-full after:w-0 after:duration-500 hover:text-white hover:shadow-yellow-300 hover:before:w-2/4 hover:before:bg-yellow-300 hover:after:w-2/4 hover:after:bg-yellow-300 text-center"><span class="relative z-10">Contact me <p class="animate-bounce">👇</p></span></a>
			</div>
			<div class="p-8 mt-12 mb-6 md:mb-0 md:mt-0 ml-0 md:ml-12 lg:w-2/3 justify-center">
				<img class="" src="./assets/logo.png">
			</div>
					</div>
				</div>
	</section>
<section id="skills">
	<div class="bg-black text-white py-20 h-screen align-middle">
		<div class="container mx-auto flex flex-col md:flex-row items-center align-middle">
			<div class="py-4 bg-black text-white">

<div class="mx-auto flex flex-col md:flex-row">
	<div class="flex flex-col w-full lg:w-3/5 p-8">
		<h1 class="text-3xl md:text-6xl mb-3 text-yellow-300 tracking-loose" style="font-weight: 700">Skills</h1>
		<div class="font-sans text-sm md:text-lg my-2 md:my-4">
			
I am passionate about crafting solid and scalable products that prioritize exceptional user experiences. My approach to development focuses on creating intuitive interfaces that seamlessly guide users through applications while ensuring stability and scalability.
		</div>
	</div>
</div>


<div class="flex flex-wrap text-center md:text-left px-8 md:px-4 lg:px-8">

	<div class="my-4 px-4 w-1/2 md:w-1/3 lg:w-1/6 overflow-hiddden">
		<div class="border-4 border-yellow-300 rounded-full transition duration-500 mx-auto md:mx-0 w-24 md:w-auto bg-yellow-300 hover:shadow-2xl hover:shadow-yellow-300 hover:transform hover:scale-90">
			<img class="p-8"
				src="./assets/html.svg"
				alt="user-avatar">
		</div>
		<p class="text-lg mt-4 md:mt-8 text-center"><b>HTML 5</b></p>
			<p class="text-yellow-300 text-center"></p>
	</div>

	<div class="my-4 px-4 w-1/2 md:w-1/3 lg:w-1/6 overflow-hiddden">
		<div class="border-4 border-yellow-300 rounded-full transition duration-500 mx-auto md:mx-0 w-24 md:w-auto bg-yellow-300 hover:shadow-2xl hover:shadow-yellow-300 hover:transform hover:scale-90">
			<img class="p-8"
				src="./assets/css.svg"
				alt="user-avatar">
		</div>
		<p class="text-lg mt-4 md:mt-8 text-center"><b>CSS 3</b></p>
			<p class="text-yellow-300 text-center"></p>
	</div>

	<div class="my-4 px-4 w-1/2 md:w-1/3 lg:w-1/6 overflow-hiddden">
		<div class="border-4 border-yellow-300 rounded-full transition duration-500 mx-auto md:mx-0 w-24 md:w-auto bg-yellow-300 hover:shadow-2xl hover:shadow-yellow-300 hover:transform hover:scale-90">
			<img class="p-8"
				src="./assets/js.svg"
				alt="user-avatar">
		</div>
		<p class="text-lg mt-4 md:mt-8 text-center"><b>JavaScript</b></p>
			<p class="text-yellow-300 text-center"></p>
	</div>

	<div class="my-4 px-4 w-1/2 md:w-1/3 lg:w-1/6 overflow-hiddden">
		<div class="border-4 border-yellow-300 rounded-full transition duration-500 mx-auto md:mx-0 w-24 md:w-auto bg-yellow-300 hover:shadow-2xl hover:shadow-yellow-300 hover:transform hover:scale-90">
			<img class="p-8"
				src="./assets/rwd.svg"
				alt="user-avatar">
		</div>
		<p class="text-lg mt-4 md:mt-8 text-center"><b>RWD</b></p>
			<p class="text-yellow-300 text-center"></p>
	</div>

	<div class="my-4 px-4 w-1/2 md:w-1/3 lg:w-1/6 overflow-hiddden">
		<div class="border-4 border-yellow-300 rounded-full transition duration-500 mx-auto md:mx-0 w-24 md:w-auto bg-yellow-300 hover:shadow-2xl hover:shadow-yellow-300 hover:transform hover:scale-90">
			<img class="p-8"
				src="./assets/git.svg"
				alt="user-avatar">
		</div>
		<p class="text-lg mt-4 md:mt-8 text-center"><b>GIT</b></p>
			<p class="text-yellow-300 text-center"></p>
	</div>

	<div class="my-4 px-4 w-1/2 md:w-1/3 lg:w-1/6 overflow-hiddden">
		<div class="border-4 border-yellow-300 rounded-full transition duration-500 mx-auto md:mx-0 w-24 md:w-auto bg-yellow-300 hover:shadow-2xl hover:shadow-yellow-300 hover:transform hover:scale-90">
			<img class="p-8"
				src="./assets/vue.svg"
				alt="user-avatar">
		</div>
		<p class="text-lg mt-4 md:mt-8 text-center"><b>Vue</b></p>
			<p class="text-yellow-300 text-center"></p>
	</div>

</div>
</div>

</div>
</div>
</section>

<section id="projects">
	<div class="bg-black text-white py-20 h-screen align-middle">
		<div class="container mx-auto flex flex-col md:flex-row items-center align-middle">
		    <div class="bg-black text-white py-8">
    <div class="container mx-auto flex flex-col items-start md:flex-row my-12 md:my-24">
      <div class="flex flex-col w-full sticky md:top-36 lg:w-1/3 px-8">
		<h1 class="text-3xl md:text-6xl mb-3 text-yellow-300 tracking-loose text-center" style="font-weight: 700" id="contact">Contact me 👇</h1>
			<p class="font-sans text-sm md:text-lg my-2 md:my-4 text-center"><svg class="inline-block fill-current mr-2"
            xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24">
            <path
              d="M12 12.713l-11.985-9.713h23.971l-11.986 9.713zm-5.425-1.822l-6.575-5.329v12.501l6.575-7.172zm10.85 0l6.575 7.172v-12.501l-6.575 5.329zm-1.557 1.261l-3.868 3.135-3.868-3.135-8.11 8.848h23.956l-8.11-8.848z" />
          </svg> sciurkiewicz@gmail.com</p>
			<div class="font-sans text-sm md:text-lg my-2 md:my-4 text-center">

				<button @click="openMailApplication" class="relative h-[50px] w-40 rounded overflow-hidden border border-yellow-300 bg-black text-yellow-300 shadow-2xl transition-all before:absolute before:left-0 before:top-0 before:h-full before:w-0 before:duration-500 after:absolute after:right-0 after:top-0 after:h-full after:w-0 after:duration-500 hover:text-white hover:shadow-yellow-300 hover:before:w-2/4 hover:before:bg-yellow-300 hover:after:w-2/4 hover:after:bg-yellow-300"><span class="relative z-10">Mail me ✉️</span></button>


			<!-- <form @submit.prevent="submitForm">
  			  <div>
  			    <label for="name">Imię:</label>
  			    <input type="text" id="name" v-model="name" required>
  			  </div>
  			  <div>
  			    <label for="email">Email:</label>
  			    <input type="email" id="email" v-model="email" required>
  			  </div>
  			  <div>
  			    <label for="message">Wiadomość:</label>
  			    <textarea id="message" v-model="message" required></textarea>
  			  </div>
  			  <button type="submit">Wyślij</button>
  			</form> -->
			</div>
      </div>
      <div class="ml-0 md:ml-12 lg:w-2/3 sticky">
        <div class="container mx-auto w-full h-full">
			<h1 class="text-3xl md:text-6xl mb-3 text-yellow-300 tracking-loose text-center" style="font-weight: 700">Projects 👇</h1>
          <div class="relative wrap overflow-hidden p-10 h-full">
            <div class="border-2-2 border-yellow-300 absolute h-full border"
              style="right: 50%; border: 2px solid rgb(253 224 71);; border-radius: 1%;"></div>
            <div class="border-2-2 border-yellow-300 absolute h-full border"
              style="left: 50%; border: 2px solid rgb(253 224 71);; border-radius: 1%;"></div>


            <div class="mb-8 flex justify-between flex-row-reverse items-center w-full left-timeline ">
              <div class="order-1 w-5/12"></div>
              <div class="order-1 w-5/12 px-1 py-4 text-right">
                <p class="mb-3 text-base text-yellow-300">Wordpress + Custom JS and CSS</p>
                <h4 class="mb-3 font-bold text-lg md:text-2xl">Sygnalista Landing (Front-End Developer)</h4>
                <p class="text-sm md:text-base leading-snug text-gray-50 text-opacity-100 mb-4 mb-4">
					Sygnalista.net is an application enabling safe and anonymous reporting of irregularities within any organization.
                </p>
				<a class="text-yellow-300" href="https://sygnalista.net/">sygnalista.net</a>
              </div>
            </div>
            <div class="mb-8 flex justify-between items-center w-full right-timeline">
              <div class="order-1 w-5/12"></div>
              <div class="order-1  w-5/12 px-1 py-4 text-left">
                <p class="mb-3 text-base text-yellow-300">Wordpress</p>
                <h4 class="mb-3 font-bold text-lg md:text-2xl">Marceto (Front-End Developer)</h4>
                <p class="text-sm md:text-base leading-snug text-gray-50 text-opacity-100 mb-4">
					Marceto is a multi E-commerce platform. It enables both B2C and B2B sellers to explore new growth opportunities in the world of e-commerce.
                </p>
				<a class="text-yellow-300" href="https://marceto.pl/">marceto.pl</a>
              </div>
            </div>
            <div class="mb-8 flex justify-between flex-row-reverse items-center w-full left-timeline">
              <div class="order-1 w-5/12"></div>
              <div class="order-1 w-5/12 px-1 py-4 text-right">
                <p class="mb-3 text-base text-yellow-300">Nuxt</p>
                <h4 class="mb-3 font-bold text-lg md:text-2xl">Zetomarket (Front-End Developer)</h4>
                <p class="text-sm md:text-base leading-snug text-gray-50 text-opacity-100 mb-4">
					The online store created in Nuxt
                </p>
				<a class="text-yellow-300" href="https://zetomarket.pl/">zetomarket.pl</a>
              </div>
            </div>

            <div class="mb-8 flex justify-between items-center w-full right-timeline">
              <div class="order-1 w-5/12"></div>

              <div class="order-1  w-5/12 px-1 py-4">
                <p class="mb-3 text-base text-yellow-300">React</p>
                <h4 class="mb-3 font-bold  text-lg md:text-2xl text-left">Scribe</h4>
                <p class="text-sm md:text-base leading-snug text-gray-50 text-opacity-100 mb-4">
					"Scribe" is an application for creating lightning-fast notes.
                </p>
				<a class="text-yellow-300" href="https://github.com/sciurkiewicz/scribe">github.com/sciurkiewicz/scribe</a>
              </div>
            </div>
			<div class="mb-8 flex justify-between flex-row-reverse items-center w-full left-timeline">
              <div class="order-1 w-5/12"></div>
              <div class="order-1 w-5/12 px-1 py-4 text-right">
                <p class="mb-3 text-base text-yellow-300">Vue3 + VueFire</p>
                <h4 class="mb-3 font-bold text-lg md:text-2xl">Crystal Ship</h4>
                <p class="text-sm md:text-base leading-snug text-gray-50 text-opacity-100 mb-4">
					"Crystal Ship" is a social networking app created using Firebase and Vue.
                </p>
				<a class="text-yellow-300" href="https://github.com/sciurkiewicz/crystal-ship">github.com/sciurkiewicz/crystal-ship</a>
              </div>
            </div>

            <div class="mb-8 flex justify-between items-center w-full right-timeline">
              <div class="order-1 w-5/12"></div>

              <div class="order-1  w-5/12 px-1 py-4">
                <p class="mb-3 text-base text-yellow-300">Javascript</p>
                <h4 class="mb-3 font-bold  text-lg md:text-2xl text-left">Bushcraft App</h4>
                <p class="text-sm md:text-base leading-snug text-gray-50 text-opacity-100 mb-4">
					An application built in pure JavaScript containing essential bushcraft tools such as a map, compass, and survival guides.
                </p>
				<a class="text-yellow-300" href="https://github.com/sciurkiewicz/bushcraft-app">github.com/sciurkiewicz/bushcraft-app</a>
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