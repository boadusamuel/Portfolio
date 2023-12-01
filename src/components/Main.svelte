<script>
  import Step from "./Step.svelte";

  let steps = [
    {
      name: "Dinpa",
      icon: "fa-solid fa-cart-shopping",
      href: "https://www.dinpa.co/",
      description:
        "Dinpa is an eccomerce store created with Next.js, Commerce.js & Stripe! Commerce.js is a CMS for managing project and Stripe is used for all transaction handling.",
    },
    {
      name: "Zuberi Core",
      icon: "fa-solid fa-list-check",
      href: "https://core.zuberipay.com/",
      description:
        "Test for model robustness with customized test profiles and receive exhaustive reporting on the performance and potential vulnerabilities of your model.",
    },
    {
      name: "GML",
      icon: "fa-solid fa-music",
      href: "https://play.google.com/store/apps/details?id=tech.rootsdigital.musiga&hl=en&gl=US",
      description:
        "Augment your datasets with our filters and dataset manipulations to ensure your models are trained on the highest quality datasets (coming soon).",
    },
  ];

  let benefits = [
    {
      name: "versatile developer",
      description:
        "Versatile Developer with a comprehensive skill set in software development. Proficient in JavaScript, HTML, CSS, PHP, and experienced with advanced frameworks, including Laravel. Skilled in crafting innovative online solutions with a passion for creativity and problem-solving. Continuously evolving expertise to meet the dynamic demands of the industry, I bring a self-driven commitment to excellence in every project.",
    },
    {
      name: "transform designs to reality",
      description:
        "I am a visionary creator who transforms designs into tangible realities with precision and innovation. Able to transform figma designs into pixel perfect websites and I love the challenge of helping users have amazing online experiences.",
    },
    {
      name: "an excellent communicator",
      description:
        "Communication is key and it's a paramount value of mine. I believe in transparency and constructive communication above all else. This helps me develop deep relationships and ensures my effectiveness and productivity in any work space with any team.",
    },
  ];
</script>

<main class="flex flex-col flex-1 p-4">
  <section
    id="introPage"
    class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14"
  >
    <div
      class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10"
    >
      <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
        Hi! I'm <span class="poppins text-violet-400">Samuel</span> Boadu
        <br />Full Stack
        <span class="poppins text-violet-400">Developer</span>
      </h2>
      <p class="text-base sm:text-lg md:text-xl">
        My <span class="text-violet-400"> favorite tech stacks</span> includes PHP, Laravel, Livewire,
        JavaScript (Vue JS, NUXT.JS, SvelteKit and React), TailwindCSS, Bootstrap, Node.js + Express.js &
        Mysql, MongoDB, PostgreSQL and Firebase/Firestore!
      </p>

      <a href="#contact"
        class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950 z-[9]"
      >
        <div
          class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
        />
        <h4 class="relative">Get in touch &rarr;</h4>
    </a>
    </div>
    <div class="relative shadow-2xl grid place-items-center">
      <img
        src={"images/profile.jpg"}
        alt="Samuel Boadu / boadusamuel / software developer"
        class="object-cover z-[2] max-h-[70vh] rounded"
      />
    </div>
  </section>
  <section class="py-20 lg:py-32 flex flex-col gap-24" id="projects">
    <div class="flex flex-col gap-2 text-center">
      <h6 class="text-large sm:text-xl md:text-2xl">
        A few of my creative endeavors.
      </h6>
      <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
        Curious to <span class="poppins text-violet-400">see</span> my work?
      </h3>
    </div>
    <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
      <Step step={steps[0]}>
        <p>
          Dinpa is an ecommerce store with the backend created using <strong
            class="text-violet-400"
            >Laravel, Livewire, MySQL!</strong
          > Dinpa allows merchants to sell their products on the platform.
        </p>
      </Step>
      <Step step={steps[1]}>
        <p>
          Zuberi Core is a Payroll Management System built with <strong class="text-violet-400"
            >Nuxt.js</strong
          > for the frontend
          & <strong class="text-violet-400">Laravel</strong> for the backend. The system
          allows management of employees
        </p>
      </Step>
      <Step step={steps[2]}>
        <p>
          Ghana Music Live (GML) is a <strong class="text-violet-400"
            >Node JS</strong
          >
          backend application, hosted on
          <strong class="text-violet-400">AWS</strong>, allowing the consumption of API by the
          <strong class="text-violet-400">Mobile App</strong>
          to display all music, artist etc.. information.!
        </p>
      </Step>
    </div>
  </section>
  <section
    id="about"
    class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative"
  >
    <div
      class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4"
    >
      <h6 class="text-large sm:text-xl md:text-2xl">Want to know more?</h6>
      <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
        A bit <span class="poppins text-violet-400">about</span> me.
      </h3>
    </div>
    <p class="mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl">
      I am . . .
    </p>
    <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
      {#each benefits as benefit, index}
    
        <div class="flex gap-6 sm:gap-8">
          <p
            class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold"
          >
            0{index + 1}
          </p>
          <div class="flex flex-col gap-6 sm:gap-8">
            <h3 class="text-2xl sm:text-3xl md:text-5xl">
              {benefit.name}
            </h3>
            <p>{benefit.description}
            </p>
           
          </div>
        </div>
      {/each}
    </div>
    <h5 class={" text-2xl sm:text-3xl font-semibold text-center poppins "}>
      The <span class="text-violet-400">Complete</span> Package
    </h5>
    <div
      class="flex flex-col overflow-x-scroll gap-10 max-w-[800px] mx-auto w-full"
    >
      <table class="bg-white text-slate-700 rounded text-center">
        <thead class={"border-b border-solid border-slate-200  "}>
          <tr class="">
            <th />
            <th class="whitespace-nowrap p-2 px-4">Candidate #1</th>
            <th class="whitespace-nowrap p-2 px-4">Candidate #2</th>
            <th class="whitespace-nowrap p-2 px-4">Candidate #3</th>
            <th class="bg-violet-700 text-white whitespace-nowrap p-4 px-8"
              >Me</th
            >
          </tr>
        </thead>
        <tbody>
          <tr class="border-b border-solid border-slate-200">
            <td
              class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
              >Dedication</td
            >
            <td><i class="fa-solid fa-xmark text-slate-500" /></td>
            <td><i class="fa-solid fa-check text-slate-500" /></td>
            <td><i class="fa-solid fa-xmark text-slate-500" /></td>
            <td><i class="fa-solid fa-check text-green-500" /></td>
          </tr>
          <tr class="border-b border-solid border-slate-200">
            <td
              class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
              >Critical Thought</td
            >
            <td><i class="fa-solid fa-xmark text-slate-500" /></td>
            <td><i class="fa-solid fa-check text-slate-500" /></td>
            <td><i class="fa-solid fa-check text-slate-500" /></td>
            <td><i class="fa-solid fa-check text-green-500" /></td>
          </tr>
          <tr>
            <td
              class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
              >Interpersonal Skills</td
            >
            <td><i class="fa-solid fa-check text-slate-500" /></td>
            <td><i class="fa-solid fa-check text-slate-500" /></td>
            <td><i class="fa-solid fa-xmark text-slate-500" /></td>
            <td><i class="fa-solid fa-check text-green-500" /></td>
          </tr>
          <tr class="border-t border-solid border-slate-200">
            <td
              class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
              >Progamming Ability</td
            >
            <td><i class="fa-solid fa-check text-slate-500" /></td>
            <td><i class="fa-solid fa-xmark text-slate-500" /></td>
            <td><i class="fa-solid fa-check text-slate-500" /></td>
            <td><i class="fa-solid fa-check text-green-500" /></td>
          </tr>
        </tbody>
      </table>
    </div>
    <div class="mx-auto mt-12 italic sm:hidden opacity-50">
      <p>Scroll to see more &rarr;</p>
    </div>
    <p class="mx-auto">So why not choose me?</p>
  </section>

  <section class="pb-20 flex flex-col sm:gap-15 md:gap-24 relative gap-4">
    <h3 class="text-center font-semibold ">
      <span class="text-2xl sm:text-3xl font-semibold text-center poppins">Credit</span>
    </h3>
   <div class="mx-auto">
    <div class="flex justify-between gap-4 flex-col">
      <p class="mb-5 sm:mb-3"><a href="https://www.linkedin.com/in/solomon-appier-sign/" target="_blank">Solomon APPIER-SIGN <span class="text-violet-400">(My Mentor)</span></a> </p>
      
      <p><a href="https://www.freecodecamp.org/" target="_blank">FreeCodeCamp  <span class="text-violet-400">(Online Resource)</span></a> </p>
    </div>
   </div>
  </section>
</main>
