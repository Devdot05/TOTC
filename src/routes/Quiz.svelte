<script lang="ts">
  const stats = [
    { value: "15K+", label: "Students", color: "text-green-800" },
    { value: "75%", label: "Total Success", color: "text-green-800" },
    { value: "35", label: "Main Questions", color: "text-green-800" },
    { value: "26", label: "Chief Experts", color: "text-green-800" },
    { value: "16", label: "Years of Experience", color: "text-green-800" },
  ];
</script>

<!-- Custom CSS for wave -->
<style>
  
</style>

<!-- HEADER -->
<section class="bg-teal-400 text-white">

  <header class="flex items-center justify-between px-6 py-4  text-white">
    <div class="text-xl font-bold text-blue-500">TOTC</div>
    <nav class="hidden md:flex gap-6">
      {#each ['Home', 'Courses', 'Careers', 'Blog', 'About Us'] as item}
        <a href="#" class="text-gray-700 hover:text-blue-500">{item}</a>
      {/each}
    </nav>
    <div class="flex gap-3">
      <button class="px-4 py-2 rounded-full font-semibold bg-red-500 text-white hover:bg-red-600">Login</button>
      <button class="px-4 py-2 rounded-full font-semibold bg-teal-50 text-blue-500 border border-blue-200 hover:bg-blue-50">Sign Up</button>
    </div>
  </header>
  
  
  <div class="relative overflow-hidden">
    <div class="max-w-7xl mx-auto px-8 flex flex-col md:flex-row items-center justify-between">
      <div class="max-w-lg md:mb-20 text-center lg:text-left py-3 px-2">
        <h1 class="text-4xl md:text-5xl font-bold leading-tight mb-4">
          Studying <span class="text-orange-400">Online</span> is now much easier
        </h1>
        <p class="mb-6 opacity-90">
          TOTC is an interesting platform that will teach you in a more interactive way
        </p>
        <div class="flex flex-col sm:flex-row gap-4 justify-center md:justify-start">
          <button class="px-6 py-3 bg-white text-blue-500 font-bold rounded-full hover:bg-gray-100 transition">
            Join for free
          </button>
          <button class="px-6 py-3 bg-white/20 backdrop-blur-sm text-white font-medium rounded-full flex items-center justify-center gap-2 hover:bg-white/30 transition">
            <svg xmlns="http://www.w3.org/  2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor">
              <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zM9.555 7.168A1 1 0 008 8v4a1 1 0 001.555.832l3-2a1 1 0 000-1.664l-3-2z" clip-rule="evenodd" />
            </svg>
            Watch how it works
          </button>
        </div>
      </div>
  
      <div class="flex justify-center">
        <img
          src="images/hero.png"
          alt="Student learning"
          class="w-80 h-auto md:w-90"
        />
      </div>
  
      <!-- Floating cards (keep as-is) -->
      <!-- <div class="absolute hidden md:block">
        <div class="absolute top-[20%] right-[10%] bg-white text-gray-800 p-4 rounded-xl shadow-lg max-w-[180px]">
          <div class="flex items-start gap-2">
            <span class="w-6 h-6 bg-red-500 text-white rounded flex items-center justify-center text-xs">🎓</span>
            <div>
              <strong class="block">250k</strong>
              <span class="text-sm">Assisted Student</span>
            </div>
          </div>
        </div>
  
        <div class="absolute bottom-[15%] right-[15%] bg-white text-gray-800 p-4 rounded-xl shadow-lg max-w-[180px]">
          <div class="flex items-start gap-2">
            <span class="w-6 h-6 bg-blue-500 text-white rounded flex items-center justify-center text-xs">📧</span>
            <div>
              <strong class="block">Congratulations</strong>
              <span class="text-sm">Your admission completed</span>
            </div>
          </div>
        </div>
  
        <div class="absolute top-[40%] right-[5%] bg-white text-gray-800 p-4 rounded-xl shadow-lg max-w-[180px]">
          <div class="flex items-start gap-2">
            <img src="images/hero.png" alt="">
            <div>
              <strong class="block text-sm">User Experience Class</strong>
              <span class="text-xs">Today at 12:00 PM</span>
              <button class="mt-2 w-full py-1 bg-red-500 text-white text-xs rounded-full">Join Now</button>
            </div>
          </div>
        </div>
      </div> -->
      <div class="max-w-2.5xl mx-auto rounded-lg absolute -bottom-1 z-99 right-0 w-full ">
        <img src="/wave5.svg" alt="svg img" class="w-full"/>
        <!-- <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Quae, nam.</p> -->
      </div>
    </div>
  </div>
</section>

<section>
  <div class="max-w-3xl px-4 sm:px-6 md:px-8 text-center mx-auto">
    <h3 class="text-2xl sm:text-3xl md:text-4xl font-bold text-gray-800 mb-4">
      Our Success
    </h3>
    <p class="text-gray-600 text-sm sm:text-base md:text-lg leading-relaxed">
      Ornare id fames interdum porttitor nulla turpis etiam. Diam vitae sollicitudin at nec nam et pharetra gravida. Adipiscing a quis ultrices eu ornare tristique vel nisl orci.
    </p>
  </div>
  <div class="bg-white py-12">
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-5 gap-y-8 gap-x-6 text-center">
      {#each stats as stat}
        <div>
          <h1 class={"text-4xl md:text-5xl font-bold !bg-gradient-to-r !from-blue-500 !to-green-400 !bg-clip-text !text-transparent"}>{stat.value}</h1>
          <p class="mt-2 text-sm font-medium">{stat.label}</p>
        </div>
      {/each}
    </div>
  </div>
</div>
</section>

<section class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
  <div class="max-w-3xl mx-auto text-center mb-10">
    <h2 class="text-3xl font-semibold mb-3">All-In-One <span class="text-green-600">Cloud Software</span></h2>
    <p class="text-gray-600">TOTC is one powerful online software suite that combines all the tools needed to run a successful school or office.</p>
  </div>

  <div class="max-w-6xl mx-auto grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8">
    <!-- CARD 1 -->
    <div class="relative bg-white shadow-lg rounded-2xl px-6 pt-16 pb-8 text-center">
      <div class="absolute -top-8 left-1/2 transform -translate-x-1/2">
        <img src="/images/Group_79.png" alt="" class="w-18 h-18" />
      </div>
      <h3 class="text-lg font-semibold mb-3">Online Billing, Invoicing, & Contracts</h3>
      <p class="text-gray-600">Simple and secure control of your organization’s financial and legal transactions. Send customized invoices and contracts.</p>
    </div>

    <!-- CARD 2 -->
    <div class="relative bg-white shadow-lg rounded-2xl px-6 pt-16 pb-8 text-center">
      <div class="absolute -top-8 left-1/2 transform -translate-x-1/2">
        <img src="/images/Group_80.png" alt="" class="w-18 h-18" />
      </div>
      <h3 class="text-lg font-semibold mb-3">Easy Scheduling & Attendance Tracking</h3>
      <p class="text-gray-600">Schedule and reserve classrooms at one campus or multiple campuses. Keep detailed records of student attendance.</p>
    </div>

    <!-- CARD 3 -->
    <div class="relative bg-white shadow-lg rounded-2xl px-6 pt-16 pb-8 text-center">
      <div class="absolute -top-8 left-1/2 transform -translate-x-1/2">
        <img src="/images/Group_81.png" alt="" class="w-18 h-18" />
      </div>
      <h3 class="text-lg font-semibold mb-3">Customer Tracking</h3>
      <p class="text-gray-600">Automate and track emails to individuals or groups. Skilline’s built-in system helps organize your organization.</p>
    </div>
  </div>
</section>

<section class="max-w-5xl mx-auto px-4 sm:px-6 lg:px-8 py-16">
  <div class="text-center max-w-4xl mx-auto px-5">
    <h2>What is TOTC?</h2>
    <p>TOTC is a platform that allows educators to create online classes whereby they can store the course materials online; manage assignments, quizzes and exams; monitor due dates; grade results and provide students with feedback all in one place.</p>
  </div>
 <div class="grid grid-cols-1 md:grid-cols-2 gap-6 text-white text-center max-w-7xl mx-auto px-4 py-12">
  <!-- LEFT CARD -->
  <div
    class="relative flex flex-col items-center justify-center h-64 md:h-96 rounded-2xl overflow-hidden">
    <div class="absolute inset-0 bg-[url('/images/Group_22.png')] bg-cover bg-center"></div>
    <div class="relative z-10">
      <h3 class="text-2xl font-semibold mb-4">FOR INSTRUCTORS</h3>
      <button class="bg-white text-amber-800 px-6 py-2 rounded-full font-medium hover:bg-amber-100 transition">
        Start a class today
      </button>
    </div>
  </div>

  <!-- RIGHT CARD -->
  <div
    class="relative flex flex-col items-center justify-center h-64 md:h-96 rounded-2xl overflow-hidden">
    <div class="absolute inset-0 bg-[url('/images/Group_23.png')] bg-cover bg-center"></div>
    <!-- <div class="absolute inset-0 bg-blue-900/60"></div> overlay -->
    <div class="relative z-10">
      <h3 class="text-2xl font-semibold mb-4">FOR STUDENTS</h3>
      <button class="bg-white text-blue-900 px-6 py-2 rounded-full font-medium hover:bg-blue-100 transition">
        Enter access code
      </button>
    </div>
  </div>
</div>
</section>

<!-- <section class="max-w-6xl mx-auto px-4 grid grid-cols-1 md:grid-cols-2 gap-8 mb-100">
  <div class="lg:mt-20 md:mt-5">
    <h3 class="mb-3 !text-md !lg:text-xl ">Everything you can do in a physical classroom, <span class="text-green-500">you can do with TOTC</span></h3>
    <p class="text-sm lg:text-1xl">TOTC’s school management software helps traditional and online schools manage scheduling, attendance, payments and virtual classrooms all in one secure cloud-based system.</p>
    <button>Learn more</button>
  </div>
  <div class="relative bg-red-500 h-screen-1/2">
    <div class="w-30 h-27 bg-blue-600 absolute -top-4 -left-3 rounded-2xl"></div>
    <div class="w-30 h-30 bg-green-600 absolute -bottom-4 -right-3 rounded-2xl"></div>
    <div class="z-10 absolute top-0 left-0 bg-amber-600 w-100 h-30 rounded-2xl"> 
      <img src="/images/Group_17.png" alt="" class="z-10 absolute top-0 left-0 bg-amber-600 w-100 h-100 rounded-2xl">
    </div>
  </div>
</section> -->


<section class="max-w-6xl mx-auto px-12 grid grid-cols-1 md:grid-cols-2 gap-16 items-center">
  <div class="space-y-5 text-center md:text-left">
    <h3 class="text-2xl lg:text-3xl font-semibold leading-snug">
      Everything you can do in a physical classroom,
      <span class="text-green-500">you can do with TOTC</span>
    </h3>
    <p class="text-gray-600 text-base lg:text-lg">
      TOTC’s school management software helps traditional and online schools manage scheduling, attendance, payments, and virtual classrooms — all in one secure cloud-based system.
    </p>
    <button class="bg-green-500 text-white px-6 py-3 rounded-full font-medium hover:bg-green-600 transition">
      Learn more
    </button>
  </div>

  <div class="relative flex justify-center items-center bg-amber-500">
    <div class="w-20 h-20 bg-blue-400 absolute -top-2 -left-3 rounded-2xl"></div>
    <div class="w-24 h-24 bg-green-400 absolute -bottom-1 -right-2 rounded-2xl"></div>

    <div class="relative z-10 rounded-2xl overflow-hidden shadow-lg">
      <img
        src="/images/Group_17.png"
        alt="Classroom illustration"
        class="w-full h-auto object-cover rounded-2xl"
      />
    </div>
  </div>
</section>

<section class="max-w-6xl mx-auto px-6 py-16 lg:py-24">
  <div class="max-w-4xl mx-auto text-center">
    <h3 class="!text-blue-900">Our <span class="text-green-400">Features</span></h3>
    <p>This very extraordinary feature, can make learning activities more efficient</p>
  </div>
  <div class="flex flex-col md:flex-row justify-between items-center mt-12">
    <div class="max-w-200 md:w-1/2">
      <img src="/images/Group_71.png" alt="Features illustration" />
    </div>
    <div class="mt-10 md:mt-0 px-5">
      <h3 class="!text-blue-900">A <span class="text-green-400">user interface</span> designed for the classroom</h3>
      <div class="flex items-center gap-4">
        <img src="/images/Group_72.png" alt="Features illustration" class="w-5 h-5"/>
        <p class="text-md sm:text-1xl">Teachers don’t get lost in the grid view and have a dedicated Podium space.</p>
      </div>
      <div class="flex items-center gap-4">
        <img src="/images/Group_73.png" alt="Features illustration" class="w-5 h-5" />
        <p class="text-md sm:text-1xl">TA’s and presenters can be moved to the front of the class.</p>
      </div>
      <div class="flex items-center gap-4">
        <img src="/images/users_2.png" alt="Features illustration" class="w-5 h-5"/>
        <p class="text-md sm:text-1xl">Teachers can easily see all students and class data at one time.</p>
      </div>
    </div>
  </div>

  <div class="flex flex-col items-center md:flex-row gap-10 mt-20 justify-between">
    <div class="text-center ">
      <h3><span class="text-green-400">Tools</span> <span class="text-blue-900">For Teachers And Learners</span></h3>
      <p>Class has a dynamic set of teaching tools built to be deployed and used during class.Teachers can handout assignments in real-time for students to complete and submit.</p>
    </div>
    <div>
      <img src="/images/Group_122.png" alt="Tools illustration" class="w-200"/>
    </div>
  </div>

  <div class="flex flex-col-reverse md:flex-row items-center justify-between gap-12 max-w-6xl mx-auto px-6 py-16">
  
    <div class="flex-1 flex justify-center">
      <div class="relative w-full max-w-md">
        <img
        src="/images/Group_92.png"
        alt="Tools illustration"
        class="w-full h-auto object-contain drop-shadow-lg rounded-2xl"
        />
        <!-- optional floating accent -->
        <div class="absolute -top-6 -left-6 w-16 h-16 bg-green-100 rounded-full -z-10"></div>
      </div>
    </div>
    <div class="flex-1 text-center md:text-left space-y-4">
      <h3 class="text-2xl lg:text-3xl font-semibold leading-snug text-blue-900">6
        Assessments, <span class="text-green-500">Quizzes</span>, Tests
      </h3>
      <p class="text-gray-600 text-base lg:text-lg">
        Easily launch live assignments, quizzes, and tests. Student results are automatically entered in the online gradebook.
      </p>
      <button class="mt-4 bg-green-500 text-white px-6 py-2 rounded-full font-medium hover:bg-green-600 transition">
        Get Started
      </button>
    </div>
  </div>


  <div class="flex flex-col md:flex-row items-center justify-between mt-16">
    <div class="max-w-xl px-12">
      <h3><span class="text-green-400">Class Management</span> Tools for Educators</h3>
      <p>Class provides tools to help run and manage the class such as Class Roster, Attendance, and more. With the Gradebook, teachers can review and grade tests and quizzes in real-time.</p>
    </div>
    <div>
      <img src="/images/Group_124.png" alt="">
    </div>
  </div>

  <div class="flex flex-col md:flex-row items-center justify-between mt-16">
    <div>
      <img src="/images/Group_106.png" alt="">
    </div>
    <div class="max-w-xl px-12">
      <h3>One-on-One <span class="text-green-400">Discussions</span></h3>
      <p>Teachers and teacher assistants can talk with students privately without leaving the Zoom environment.</p>
    </div>
  </div>
</section>


<section class="bg-blue-50 py-16 px-6 lg:px-12">
  <!-- Header -->
  <div class="max-w-6xl mx-auto text-center mb-10">
    <h2 class="text-3xl font-bold text-blue-900">Explore Course</h2>
    <p class="text-gray-500 mt-2">Sed eros finibus, placerat orci id, dapibus.</p>
  </div>

  <!-- Course Sections -->
  <div class="space-y-16 max-w-6xl mx-auto">
    <!-- One section -->
    <div>
      <!-- Title and See All -->
      <div class="flex items-center justify-between mb-4">
        <h3 class="text-xl font-semibold text-blue-800">Lorem Ipsum</h3>
        <a href="#" class="text-green-500 hover:text-green-600 font-medium">See all →</a>
      </div>

      <!-- Tilted Tags -->
      <div class="flex overflow-x-auto gap-3 mb-6 pb-2">
        <div class="flex gap-3">
          <span class="bg-green-100 text-green-700 px-4 py-2 rounded-xl transform -rotate-6 whitespace-nowrap">UI Design</span>
          <span class="bg-orange-100 text-orange-700 px-4 py-2 rounded-xl transform rotate-3 whitespace-nowrap">Coding Concept</span>
          <span class="bg-blue-100 text-blue-700 px-4 py-2 rounded-xl transform -rotate-6 whitespace-nowrap">Web Design</span>
          <span class="bg-yellow-100 text-yellow-700 px-4 py-2 rounded-xl transform rotate-3 whitespace-nowrap">Data Analysis</span>
        </div>
      </div>

      <!-- Course Card -->
      <div class="bg-white rounded-2xl shadow-md p-5 flex items-center gap-6 hover:shadow-xl transition">
        <img src="/images/course1.jpg" alt="Course" class="w-32 h-32 rounded-xl object-cover" />
        <div>
          <h4 class="font-semibold text-lg text-blue-900">Integer id Orc Sed Ante Tincidunt</h4>
          <p class="text-gray-500 text-sm mt-1">
            Cras convallis lacus orci, tristique tincidunt magna fringilla at.
          </p>
          <div class="flex items-center justify-between mt-3">
            <span class="text-yellow-400">★★★★★</span>
            <span class="text-blue-800 font-semibold">$450</span>
          </div>
          <button class="mt-3 bg-green-500 text-white px-4 py-1 rounded-full text-sm hover:bg-green-600">
            Explore
          </button>
        </div>
      </div>
    </div>
  </div>
</section>


<section class="bg-[#E9F3FF] py-16 px-6">
  <!-- Header -->
  <div class="text-center mb-12">
    <h2 class="text-3xl font-bold text-gray-900 relative inline-block">
      Explore Course
      <span class="absolute -bottom-2 left-0 w-full h-1 bg-purple-400"></span>
    </h2>
    <p class="text-gray-500 mt-4">Sed eros finibus, placerat orci id, dapibus.</p>
  </div>

  <!-- One Section -->
  <div class="max-w-6xl mx-auto mb-20">
    <!-- Title and See all -->
    <div class="flex justify-between items-center mb-6">
      <h3 class="font-semibold text-xl text-gray-800">Lorem Ipsum</h3>
      <a href="#" class="text-sky-500 font-medium hover:underline">SEE ALL →</a>
    </div>

    <!-- Tilted Tags -->
    <div class=" max-h-30 bg-amber-800">
      <div class="bg-white px-2 py-1 rounded-4 rotate-80">
        <div class="bg-green-400 px-2 py-2 rounded-4">
          <span class="bg-orange-100 text-orange-600 px-5 py-2 rounded-full">UI Design</span>
        </div>
      </div>
       
      <div class="bg-white px-2 py-1 rounded-4 rotate-80">
        <div class="bg-green-400 px-2 py-2 rounded-4">
          <span class="bg-green-100 text-green-600 px-5 py-2 rounded-4 -rotate-6 shadow-sm">Coding Concept</span>
        </div>
      </div>
       <div class="bg-white px-2 py-1 rounded-4 rotate-80">
        <div class="bg-green-400 px-2 py-2 rounded-4">
          <span class="bg-blue-100 text-blue-600 px-5 py-2 rounded-full rotate-3 shadow-sm">Web Design</span>
        </div>
      </div>
       <div class="bg-white px-2 py-1 rounded-4 rotate-80">
        <div class="bg-green-400 px-2 py-2 rounded-4">
          <span class="bg-yellow-100 text-yellow-600 px-5 py-2 rounded-full -rotate-3 shadow-sm">UX System</span>
        </div>
      </div>
      <div class="bg-white px-2 py-1 rounded-4 rotate-80">
        <div class="bg-green-400 px-2 py-2 rounded-4">
          <span class="bg-pink-100 text-pink-600 px-5 py-2 rounded-full rotate-6 shadow-sm">Frontend</span>
        </div>
      </div>
    </div>

    <!-- Course Card -->
    <div class="flex flex-col sm:flex-row items-center bg-white shadow-md rounded-3xl overflow-hidden hover:shadow-xl transition">
      <img src="/images/course1.jpg" alt="Course" class="w-full sm:w-48 h-48 object-cover">
      <div class="p-6 flex flex-col justify-between">
        <h4 class="text-lg font-semibold text-gray-800">Integer id Orc Sed Ante Tincidunt</h4>
        <p class="text-gray-500 text-sm mt-2">Cras convallis lacus orci, tristique tincidunt magna fringilla at faucibus vel.</p>
        <div class="flex items-center justify-between mt-4">
          <span class="text-yellow-400 text-lg">★★★★★</span>
          <span class="text-gray-800 font-semibold">$450</span>
        </div>
        <button class="mt-4 bg-sky-500 text-white px-6 py-2 rounded-full hover:bg-sky-600 transition">EXPLORE</button>
      </div>
    </div>
  </div>
</section>


 
 