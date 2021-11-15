<template>
  <div class="bg-no-repeat bg-cover flex justify-center p-10" :style="bgImg">
    <div
      class="
        grid
        lg:grid-cols-3 lg:w-10/12 lg:h-3/5
        md:grid-cols-2 md:w-4/5 md:h-3/5
        gap-8
        max-w-screen-lg
      "
    >
      <div
        class="
          rounded-md
          bg-black bg-opacity-50
          border-2
          text-white
          flex flex-col
          items-center
          p-10
          shadow-2xl
          hover:bg-opacity-80
          transition
          duration-500
          ease-in-out
          transform
          hover:-translate-y-1 hover:scale-110
          gap-6
          text-center text-xs
          font-sans
          md:text-sm
          xl:text-lg
        "
        v-for="items of data"
        :key="items.id"
      >
        <img
          class="
            w-20
            h-20
            rounded-full
            object-cover
            md:h-28 md:w-28
            lg:w-36 lg:h-36
          "
          :src="items.image"
        />
        <div class="tracking-tight">
          {{ items.description }}
        </div>
        <div
          class="
            flex flex-row
            w-full
            text-center
            justify-around
            divide-purple-500 divide-x-2 divide-black
          "
        >
          <div class="w-1/2">{{ items.name }}</div>
          <div class="w-1/2">{{ items.ocupation }}</div>
        </div>
        <button
          class="
            text-white
            font-bold
            py-1
            px-2
            rounded
            bg-gradient-to-r
            from-purple-500
            to-purple-400
          "
        >
          More Information
        </button>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      data: [
        {
          id: 1,
          name: "Alfred",
          description:
            '"Lorem ipsum dolor sit amet consectetur adipisicing elit. Minus tempora sequi fugit dolorem veritatis incidunt consectetur animi tempore suscipit excepturi itaque accusamus nobis vel, hic numquam"',
          ocupation: "Developer",
          image:
            "https://images.unsplash.com/photo-1521252659862-eec69941b071?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=325&q=80",
        },
        {
          id: 2,
          name: "Joel",
          description:
            '"Lorem ipsum dolor sit amet consectetur adipisicing elit. Minus tempora sequi fugit dolorem veritatis incidunt consectetur animi tempore suscipit excepturi itaque accusamus nobis vel, hic numquam"',
          ocupation: "Doctor",
          image:
            "https://images.unsplash.com/photo-1603415526960-f7e0328c63b1?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=870&q=80",
        },
        {
          id: 3,
          name: "Sarah",
          description:
            '"Lorem ipsum dolor sit amet consectetur adipisicing elit. Minus tempora sequi fugit dolorem veritatis incidunt consectetur animi tempore suscipit excepturi itaque accusamus nobis vel, hic numquam"',
          ocupation: "Engineer",
          image:
            "https://images.unsplash.com/photo-1628890920690-9e29d0019b9b?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=387&q=80",
        },
        {
          id: 4,
          name: "Blanca",
          description:
            '"Lorem ipsum dolor sit amet consectetur adipisicing elit. Minus tempora sequi fugit dolorem veritatis incidunt consectetur animi tempore suscipit excepturi itaque accusamus nobis vel, hic numquam"',
          ocupation: "Engineer",
          image:
            "https://images.unsplash.com/photo-1508214751196-bcfd4ca60f91?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=870&q=80",
        },
        {
          id: 5,
          name: "Juan",
          description:
            '"Lorem ipsum dolor sit amet consectetur adipisicing elit. Minus tempora sequi fugit dolorem veritatis incidunt consectetur animi tempore suscipit excepturi itaque accusamus nobis vel, hic numquam"',
          ocupation: "Engineer",
          image:
            "https://images.unsplash.com/photo-1544723795-3fb6469f5b39?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=389&q=80",
        },
        {
          id: 6,
          name: "Karla",
          description:
            '"Lorem ipsum dolor sit amet consectetur adipisicing elit. Minus tempora sequi fugit dolorem veritatis incidunt consectetur animi tempore suscipit excepturi itaque accusamus nobis vel, hic numquam"',
          ocupation: "Engineer",
          image:
            "https://images.unsplash.com/photo-1598550880863-4e8aa3d0edb4?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=327&q=80",
        },
      ],
      bgImg: {
        backgroundImage: `url(${require("../assets/images/bg-image.jpg")})`,
      },
    };
  },
};
//BG IMAGE
//https://images.unsplash.com/photo-1634270874854-3c7492905b74?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1100&q=80
</script>