<template>
  <div class="landing-page">
    <section class="landing-hero pt-5">
      <div class="header__bg"></div>
      <div class="container mx-auto relative">
        <Header/>
        <div class="flex items-center pt-10 px-5 md:px-0">
          <div class="w-1/2">
            <h1 class="text-4xl text-white mb-5">
              We helps <u class="hero-underline">startup</u> to <br />
              getting started & <u class="hero-underline">funding</u> <br />
              their truly needs
            </h1>
            <p class="text-white text-xl font-light mb-8">
            </p>
            <button
              @click="$router.push({ path: '/' })"
              class="block bg-orange-button hover:bg-green-button text-white font-semibold px-12 py-3 text-xl rounded-full"
            >
              Find a Project
            </button>
          </div>
          <div class="w-1/2 flex justify-center">
            <img
              src="/assets/images/ringwithcircles-removebg-preview.png"
              alt="crowdfunding project"
            />
          </div>
        </div>
      </div>
    </section>

    <section class="container mx-auto pt-24">
      <div class="flex justify-between items-center">
        <div class="w-auto">
          <h2 class="text-3xl text-gray-900 mb-8">
           <br></br> Most
            popular
          </h2>
        </div>
        <div class="w-auto mt-5">
          <a class="text-gray-900 hover:underline text-md font-medium" href=""
            >View All</a
          >
        </div>
      </div>
      <div class="flex mt-3 -mx-6">
        <div
          class="card-project w-1/3 mx-6 my-4 p-5 border border-gray-500 rounded-20"
        >
          <div class="item">
            <figure class="item-image">
              <img
                src="/assets/images/adobe.png"
                alt=""
                class="rounded-20 w-full"
              />
            </figure>
            <div class="item-meta">
              <h4 class="text-3xl font-medium text-gray-900 mt-5">
                Adobe XD
              </h4>
              <p class="text-md font-light text-gray-900">
                Adobe XD merupakan salah satu alat bantu gratis paling banyak digunakan untuk web design atau mobile design UI / UX dan prototyping untuk berbagai platform termasuk web, ponsel, tablet, dan lainnya.
              </p>
              <div class="relative pt-4 progress-bar">
                <div
                  class="overflow-hidden h-2 mb-4 text-xs flex bg-gray-200 rounded-lg"
                >
                  <div
                    style="width: 20%"
                    class="shadow-none flex flex-col text-center whitespace-nowrap text-white justify-center bg-purple-progress progress-striped"
                  ></div>
                </div>
              </div>
              <div class="flex progress-info">
                <div>20%</div>
                <div class="ml-auto font-semibold">Nice</div>
              </div>
            </div>
            <NuxtLink
              to="/projects/1"
              class="text-center mt-5 button-cta block w-full bg-orange-button hover:bg-green-button text-white font-semibold px-6 py-2 text-lg rounded-full"
            >
              Start Now
            </NuxtLink>
          </div>
        </div>
        <div
          class="card-project w-1/3 mx-6 my-4 p-5 border border-gray-500 rounded-20"
        >
          <div class="item">
            <figure class="item-image">
              <img
                src="/assets/images/invision.png"
                alt=""
                class="rounded-20 w-full"
              />
            </figure>
            <div class="item-meta">
              <h4 class="text-3xl font-medium text-gray-900 mt-5">
                InVision
              </h4>
              <p class="text-md font-light text-gray-900">
                Desain produk adalah keseluruhan pengalaman produk. Ini adalah ungkapan yang tidak berbentuk, dan rasa serta proses untuk desain produk sangat bervariasi. Ini bisa berarti merancang aplikasi seluler, aplikasi web, situs web, dasbor, branding, atau semua hal di atas.
              </p>
              <div class="relative pt-4 progress-bar">
                <div
                  class="overflow-hidden h-2 mb-4 text-xs flex bg-gray-200 rounded-lg"
                >
                  <div
                    style="width: 45%"
                    class="shadow-none flex flex-col text-center whitespace-nowrap text-white justify-center bg-purple-progress progress-striped"
                  ></div>
                </div>
              </div>
              <div class="flex progress-info">
                <div>45%</div>
                <div class="ml-auto font-semibold">Nice</div>
              </div>
              <NuxtLink
                to="/projects/2"
                class="text-center mt-5 button-cta block w-full bg-orange-button hover:bg-green-button text-white font-semibold px-6 py-2 text-lg rounded-full"
              >
                Start Now
              </NuxtLink>
            </div>
          </div>
        </div>
        <div
          class="card-project w-1/3 mx-6 my-4 p-5 border border-gray-500 rounded-20"
        >
          <div class="item">
            <figure class="item-image">
              <img
                src="/assets/images/figma.png"
                alt=""
                class="rounded-20 w-full"
              />
            </figure>
            <div class="item-meta">
              <h4 class="text-3xl font-medium text-gray-900 mt-5">Figma</h4>
              <p class="text-md font-light text-gray-900">
                Dunia sistem desain sangatlah luas dan panduannya terus berubah seiring dengan munculnya teknologi dan aliran pemikiran baru. Sulit mengetahui harus mulai dari mana, bahkan bagi desainer berpengalaman.
              </p>
              <div class="relative pt-4 progress-bar">
                <div
                  class="overflow-hidden h-2 mb-4 text-xs flex bg-gray-200 rounded-lg"
                >
                  <div
                    style="width: 80%"
                    class="shadow-none flex flex-col text-center whitespace-nowrap text-white justify-center bg-purple-progress progress-striped"
                  ></div>
                </div>
              </div>
              <div class="flex progress-info">
                <div>80%</div>
                <div class="ml-auto font-semibold">Rp 40.000.000</div>
              </div>
              <NuxtLink
                to="/projects/3"
                class="text-center mt-5 button-cta block w-full bg-orange-button hover:bg-green-button text-white font-semibold px-6 py-2 text-lg rounded-full"
              >
                Start Now
              </NuxtLink>
            </div>
          </div>
        </div>
      </div>

    </section>
 
    <section class="container mx-auto pt-24">
  <div class="flex justify-between items-center">
    <div class="w-auto">
      <h2 class="text-3xl text-gray-900 mb-8">
        Trusted Brands
      </h2>
    </div>
    <div class="w-auto mt-5">
      <a class="text-gray-900 hover:underline text-md font-medium" href="">View All</a>
    </div>
  </div>
  <div class="flex mt-3 -mx-6">
    <div class="card-project w-1/3 mx-6 my-4 p-5 border border-gray-500 rounded-20">
      <div class="item">
        <figure class="item-image">
          <img src="/assets/images/google.png" alt="Google Logo" class="rounded-20 w-full">
        </figure>
        <div class="item-meta">
          <h4 class="text-3xl font-medium text-gray-900 mt-5">Google</h4>
          <p class="text-md font-light text-gray-900">
            Est tation latine aliquip id, mea ad tale illud definitiones. Periculis omittantur necessitatibus eum ad, 
          </p>
          <!-- Progress Bar and Start Now Button -->
        </div>
      </div>
    </div>
    <div class="card-project w-1/3 mx-6 my-4 p-5 border border-gray-500 rounded-20">
      <div class="item">
        <figure class="item-image">
          <img src="/assets/images/netflix.png" alt="Netflix Logo" class="rounded-20 w-full">
        </figure>
        <div class="item-meta">
          <h4 class="text-3xl font-medium text-gray-900 mt-5">Netflix</h4>
          <p class="text-md font-light text-gray-900">
            Est tation latine aliquip id, mea ad tale illud definitiones. Periculis omittantur necessitatibus eum ad, 
          </p>
          <!-- Progress Bar and Start Now Button -->
        </div>
      </div>
    </div>
    <div class="card-project w-1/3 mx-6 my-4 p-5 border border-gray-500 rounded-20">
      <div class="item">
        <figure class="item-image">
          <img src="/assets/images/airbnb.png" alt="Airbnb Logo" class="rounded-20 w-full">
        </figure>
        <div class="item-meta">
          <h4 class="text-3xl font-medium text-gray-900 mt-5">Airbnb</h4>
          <p class="text-md font-light text-gray-900">
            Est tation latine aliquip id, mea ad tale illud definitiones. Periculis omittantur necessitatibus eum ad,
          </p>
          <!-- Progress Bar and Start Now Button -->
        </div>
      </div>
    </div>
  </div>
</section>

<section class="container mx-auto pt-24">
  <div class="flex justify-between items-center">
    <div class="w-auto">
      <h2 class="text-3xl text-gray-900 mb-8">
        New Comer Tools
      </h2>
    </div>
    <div class="w-auto mt-5">
      <a class="text-gray-900 hover:underline text-md font-medium" href="">View All</a>
    </div>
  </div>
  <div class="flex mt-3 -mx-6">
    <div class="card-project w-1/3 mx-6 my-4 p-5 border border-gray-500 rounded-20">
      <div class="item">
        <figure class="item-image">
          <img src="/assets/images/framer.png" alt="Framer Logo" class="rounded-20 w-full">
        </figure>
        <div class="item-meta">
          <h4 class="text-3xl font-medium text-gray-900 mt-5">Framer</h4>
          <p class="text-md font-light text-gray-900">
            Adobe XD merupakan salah satu alat bantu gratis paling banyak digunakan untuk web design atau mobile design UI / UX dan prototyping untuk berbagai platform termasuk web, ponsel, tablet, dan lainnya.
          </p>
          <!-- Progress Bar and Start Now Button -->
        </div>
      </div>
    </div>
    <div class="card-project w-1/3 mx-6 my-4 p-5 border border-gray-500 rounded-20">
      <div class="item">
        <figure class="item-image">
          <img src="/assets/images/Whimsical.png" alt="Whimsical Logo" class="rounded-20 w-full">
        </figure>
        <div class="item-meta">
          <h4 class="text-3xl font-medium text-gray-900 mt-5">Whimsical</h4>
          <p class="text-md font-light text-gray-900">
            Adobe XD merupakan salah satu alat bantu gratis paling banyak digunakan untuk web design atau mobile design UI / UX dan prototyping untuk berbagai platform termasuk web, ponsel, tablet, dan lainnya.
          </p>
          <!-- Progress Bar and Start Now Button -->
        </div>
      </div>
    </div>
    <div class="card-project w-1/3 mx-6 my-4 p-5 border border-gray-500 rounded-20">
      <div class="item">
        <figure class="item-image">
          <img src="/assets/images/mindmaster.png" alt="MindMaster Logo" class="rounded-20 w-full">
        </figure>
        <div class="item-meta">
          <h4 class="text-3xl font-medium text-gray-900 mt-5">MindMaster</h4>
          <p class="text-md font-light text-gray-900">
            Adobe XD merupakan salah satu alat bantu gratis paling banyak digunakan untuk web design atau mobile design UI / UX dan prototyping untuk berbagai platform termasuk web, ponsel, tablet, dan lainnya.
          </p>
          <!-- Progress Bar and Start Now Button -->
        </div>
      </div>
    </div>
    <div class="card-project w-1/3 mx-6 my-4 p-5 border border-gray-500 rounded-20">
      <div class="item">
        <figure class="item-image">
          <img src="/assets/images/zapier.png" alt="Zapier Logo" class="rounded-20 w-full">
        </figure>
        <div class="item-meta">
          <h4 class="text-3xl font-medium text-gray-900 mt-5">Zapier</h4>
          <p class="text-md font-light text-gray-900">
            Adobe XD merupakan salah satu alat bantu gratis paling banyak digunakan untuk web design atau mobile design UI / UX dan prototyping untuk berbagai platform termasuk web, ponsel, tablet, dan lainnya.
          </p>
          <!-- Progress Bar and Start Now Button -->
        </div>
      </div>
    </div>
  </div>
</section>

    <section class="container mx-auto pt-24">
  <div class="flex justify-between items-center">
    <div class="w-auto">
      <h2 class="text-3xl text-gray-900 mb-8">
        Testimoninal
      </h2>
    </div>
  </div>
  <div class="flex mb-10">
    <div class="w-1/3">
      <div class="testimonial-box">
        <div class="testimonial-content">
          <p class="testimonial-text">
            Gear Menyediakan informasi tools yang powerful untuk Designer, Developer, dan juga Business Owner agar bisa lebih produktif
          </p>
          <div class="testimonial-author">
            <img src="/assets/images/adobe.png" alt="" class="testimonial-avatar">
            <span class="author-name">Wahid Ari Designer</span>
          </div>
        </div>
        <div class="testimonial-rating">
          <span class="rating-stars">&#9733;&#9733;&#9733;&#9733;&#9733;</span>
        </div>
      </div>
    </div>
    <div class="w-1/3">
      <div class="testimonial-box">
        <div class="testimonial-content">
          <p class="testimonial-text">
            Gear Menyediakan informasi tools yang powerful untuk Designer, Developer, dan juga Business Owner agar bisa lebih produktif
          </p>
          <div class="testimonial-author">
            <img src="/assets/images/gear.png" alt="" class="testimonial-avatar">
            <span class="author-name">Wahid Sharma Developer</span>
          </div>
        </div>
        <div class="testimonial-rating">
          <span class="rating-stars">&#9733;&#9733;&#9733;&#9733;&#9733;</span>
        </div>
      </div>
    </div>
    <div class="w-1/3">
      <div class="testimonial-box">
        <div class="testimonial-content">
          <p class="testimonial-text">
            Gear Menyediakan informasi tools yang powerful untuk Designer, Developer, dan juga Business Owner agar bisa lebih produktif
          </p>
          <div class="testimonial-author">
            <img src="/assets/images/gear.png" alt="" class="testimonial-avatar">
            <span class="author-name">Ari UX Designer</span>
          </div>
        </div>
        <div class="testimonial-rating">
          <span class="rating-stars">&#9733;&#9733;&#9733;&#9733;&#9733;</span>
        </div>
      </div>
    </div>
  </div>
</section>



    <div class="cta-clip -mt-20"></div>
    <CallToAction />
    <Footer />
  </div>
</template>

<style>
@media (max-width: 768px) {
  /* Flex direction column for mobile */
  .landing-page .landing-hero .flex,
  .container,
  .card-project,
  .justify-between,
  .item {
    flex-direction: column !important;
    width: 100% !important;
  }

  /* Remove negative margin */
  .flex.mb-10 {
    margin-bottom: 0 !important;
  }

  /* Remove horizontal margin */
  .mx-6 {
    margin-left: 0 !important;
    margin-right: 0 !important;
  }

  /* Increase bottom margin for vertical spacing */
  .my-4 {
    margin-bottom: 20px !important;
  }

  /* Additional styles for specific sections */
  /* Stack AdobeXD, Invision, Figma items vertically */
  .landing-page .container:nth-child(3) .card-project,
  .landing-page .container:nth-child(4) .card-project,
  .landing-page .container:nth-child(5) .card-project {
    flex-direction: column !important;
  }
}
</style>