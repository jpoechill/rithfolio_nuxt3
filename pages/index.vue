<template>
  <div class="mt-0 top-0 text-dark" style="background-color: #fbfbfb;">
    <div class="border-top custom-bg w-100 z-0" style="background-color: #fbfbfb;">
      <div class="container py-6 pb-7 mx-auto">
        <div class="grid grid-cols-12 gap-5 mt-0 mx-[80px] pb-5">
          <div v-for="(project, index) in projects" :key="index" class="h-full  col-span-6">
            <div class="px-4 mt-5 mb-2">
              <div class="bg-white pb-1 box-shadow"
                style="border-radius: 10px; overflow: hidden; border: 1px solid #ddd;">
                <div class="w-full overflow-hidden">
                  <a :href="project.url" target="_blank">
                    <img :src="project.img" class="w-full transform zoom" alt="">
                  </a>
                </div>
                <div class="pt-4 pb-2 px-5 mb-5">
                  <span class="font-medium text-xl px-5 mt-5 text-gray-600 mb-3 block">
                    <h4>{{ project.title }}</h4>
                  </span>
                  <p class="mb-4 mb-5 px-5 text-gray-600">
                    <span v-html="project.description" />
                  </p>
                  <p class="mt-3 pb-0 pt-4 text-right">
                    <span v-for="(link, index) in project.links" :key="index">
                      <a :href="link.url">{{ link.title }}</a>
                      <span v-if="index !== project.links.length - 1"> | </span>
                    </span>
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">

const count = 100099
const projects = [
  {
    title: 'Frontend Quiz',
    description: 'A multi-page, frontend, quiz application utilizing features in Next.js and Tailwind. ',
    img: '/browser-01.jpg',
    url: 'https://ppc-restore.com/',
    links: [
      {
        title: 'Github',
        url: 'https://github.com/jpoechill/fequiz'
      },
      {
        title: 'Live Site',
        url: 'https://fequiz.vercel.app/'
      }
    ]
  },
  {
    title: 'Product Feedback',
    description: 'A frontend, product feedback application made for managing feature requests for products and teams.',
    img: '/browser-12.png',
    url: 'https://compassionate-hugle-3311b0.netlify.app/',
    links: [
      {
        title: 'Github',
        url: 'https://github.com/jpoechill/product-feedback-fem'
      },
      {
        title: 'Demo',
        url: 'https://compassionate-hugle-3311b0.netlify.app/'
      }
    ]
  },
  {
    title: 'Invoices',
    description: 'A frontend, invoice application for managing and tracking invoices for entreprenuers and freelancers.',
    img: '/browser-13.jpg',
    url: 'https://sweet-muffin-869709.netlify.app/',
    links: [
      {
        title: 'Github',
        url: 'https://github.com/jpoechill/invoice-app'
      },
      {
        title: 'Demo',
        url: 'https://sweet-muffin-869709.netlify.app/'
      }
    ]
  },
  {
    title: 'Simple To Dos',
    description: 'A frontend, to-do application featuring light and dark modes, along persistent data with GraphQL.',
    img: '/todo_cover_rithfolio.png',
    url: 'https://todo-gql.vercel.app/',
    links: [
      {
        title: 'Github',
        url: 'https://github.com/jpoechill/fem-todo-fullstack'
      },
      {
        title: 'Demo',
        url: 'https://todo-gql.vercel.app/'
      }
    ]
  }
]
</script>

<style scoped>
.text-light {
  color: #333 !important;
}

.zoom {
  transition: transform .5s ease;
}

.zoom:hover {
  cursor: pointer;
  transform: scale(1.04);
  /* (150% zoom - Note: if the zoom is too large, it will go outside of the viewport) */
}

.fixed-ratio {
  width: 100%;
  padding-bottom: 63.78%;
}

.box-shadow {
  -webkit-box-shadow: 5px 6px 14px 2px rgba(0, 0, 0, 0.25);
  box-shadow: 5px 6px 14px 2px rgba(0, 0, 0, 0.1);
}

.custom-bg {
  background-color: #b7b7b70f;
  background-image: linear-gradient(135deg, #ffffff 25%, transparent 25%), linear-gradient(225deg, #ffffff 25%, transparent 25%), linear-gradient(45deg, #ffffff 25%, transparent 25%), linear-gradient(315deg, #ffffff 25%, rgb(183 183 183 / 0%) 25%);
  background-position: 40px 0, 40px 0, 0 0, 0 0;
  background-size: 80px 80px;
  background-repeat: repeat;
}
</style>
