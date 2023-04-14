<template>
  <div class="bg-white py-24">
    <div class="mx-auto max-w-7xl border">
      <div class="mx-auto lg:mx-0">
        <h2 class="text-lg leading-8 text-gray-600 border-b p-4">
          We have found 1700 emails for Dunder Mifflin Paper in our database
        </h2>
        <p
          class="mt-6 text-lg leading-8 text-gray-900 px-6 underline font-semibold"
        >
          Relevant Prospects
        </p>
      </div>
      <ul
        role="list"
        class="mx-auto mt-2 grid max-w-2xl grid-cols-1 gap-x-8 gap-y-16 sm:grid-cols-2 lg:mx-0 lg:max-w-none lg:grid-cols-3 px-6"
      >
        <li v-for="person in people" :key="person.name">
          <div class="flex flex-1 flex-col p-8">
            <img
              class="aspect-[3/2] w-full rounded-2xl object-cover"
              :src="person.imageUrl"
              alt=""
            />
            <h3
              class="text-center mt-6 text-lg font-semibold leading-8 tracking-tight text-gray-900"
            >
              {{ person.name }}
            </h3>
            <p class="text-center text-base leading-7 text-gray-600">
              {{ person.role }}
            </p>
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>

<script setup>
const people = [
  {
    name: "Dwight Schrute",
    role: "Sales Development Executive",
    imageUrl:
      "https://images.unsplash.com/photo-1472099645785-5658abf4ff4e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=8&w=1024&h=1024&q=80",
  },
  {
    name: "Jim Halpert",
    role: "Sales Manager",
    imageUrl:
      "https://images.unsplash.com/photo-1531427186611-ecfd6d936c79?ixlib=rb-=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=8&w=1024&h=1024&q=80",
  },
  {
    name: "Andy Bernard",
    role: "Sales Development Executive",
    imageUrl:
      "https://images.unsplash.com/photo-1472099645785-5658abf4ff4e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=8&w=1024&h=1024&q=80",
  },
  // More people...
];
</script>
