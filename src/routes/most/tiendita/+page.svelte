<script>
   

  const items = [
    {
      imgSrc:
      "src/routes/tiendita/file.jpg",
      title: "Grilled Salmon",
      description:
        "Succulent salmon fillet grilled to perfection, served with a side of roasted vegetables.",
      price: "$24.99",
      likes: 8,
    },
    {
      imgSrc:
        "https://instagram.fscl11-2.fna.fbcdn.net/v/t39.30808-6/397310981_17884035323957532_2494761078698259730_n.jpg?stp=dst-jpg_e35_p640x640_sh0.08&efg=eyJ2ZW5jb2RlX3RhZyI6ImltYWdlX3VybGdlbi4xMTUyeDIwNDguc2RyLmYzMDgwOCJ9&_nc_ht=instagram.fscl11-2.fna.fbcdn.net&_nc_cat=100&_nc_ohc=MJmdFfaeBEUQ7kNvgFyPczM&edm=AGFyKLkAAAAA&ccb=7-5&ig_cache_key=MzIyNjcyNDgyMTg0OTA2MjM4OQ%3D%3D.2-ccb7-5&oh=00_AYCL5HtkwdtzmySVetkli1jniEoL_yCYenrLAnR_nnhcZQ&oe=66AB7DE8&_nc_sid=5a0a6d",
      title: "Lemon Meringue Pie",
      description:
        "A classic lemon meringue pie with a tangy filling and a light, fluffy meringue topping.",
      price: "$12.99",
      likes: 8,
    },
    {
      imgSrc:
      "https://instagram.fscl11-2.fna.fbcdn.net/v/t39.30808-6/397310981_17884035323957532_2494761078698259730_n.jpg?stp=dst-jpg_e35_p640x640_sh0.08&efg=eyJ2ZW5jb2RlX3RhZyI6ImltYWdlX3VybGdlbi4xMTUyeDIwNDguc2RyLmYzMDgwOCJ9&_nc_ht=instagram.fscl11-2.fna.fbcdn.net&_nc_cat=100&_nc_ohc=MJmdFfaeBEUQ7kNvgFyPczM&edm=AGFyKLkAAAAA&ccb=7-5&ig_cache_key=MzIyNjcyNDgyMTg0OTA2MjM4OQ%3D%3D.2-ccb7-5&oh=00_AYCL5HtkwdtzmySVetkli1jniEoL_yCYenrLAnR_nnhcZQ&oe=66AB7DE8&_nc_sid=5a0a6d",
      title: "Lemon Meringue Pie",
      description:
        "A classic lemon meringue pie with a tangy filling and a light, fluffy meringue topping.",
      price: "$12.99",
      likes: 8,
    },
  ];
  const nophoto = [
    {name:"Poleras",description:"",price:"$15.000"},
                {name:"Totes",description:"",price:"$12.000"},
                {name:"Café en grano / molido",description:"250 gr",price:"$9.000"},
  ];
</script>

<svelte:head>
  <title>El pasaje</title>
  <meta name="description" content="About this app" />
  <script src="https://cdn.tailwindcss.com"></script>
</svelte:head>

<div class="flex flex-col min-h-screen">
  

  <section
    class="container px-0 py-8 md:px-6 flex flex-col items-start gap-8 max-w-[80%] md:max-w-[70%] mx-auto"
  >
    <div
      id="sectionItemsContent"
      class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6"
    >
      {#each items as item}
        <div
          class="rounded-lg border bg-card text-card-foreground shadow-sm"
          data-v0-t="card"
        >
          <img
            src={item.imgSrc}
            width="150"
            height="100"
            alt="Dish"
            class="rounded-t-md object-cover w-[100%]"
          />
          <div class="p-4">
            <h3 class="text-lg font-medium">{item.title}</h3>
            <p class="text-muted-foreground text-sm">{item.description}</p>
            <div class="mt-4 flex items-center justify-between">
              <span class="font-medium">{item.price}</span>
              <button
                class="inline-flex items-center justify-center hover:backdrop-brightness-50 whitespace-nowrap rounded-md text-sm font-medium ring-offset-background transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50 border border-input bg-background hover:bg-accent hover:text-accent-foreground h-10 px-4 py-2"
              >
                Me gusta ({item.likes})
              </button>
            </div>
          </div>
        </div>
      {/each}
      {#each nophoto as item}
        <div class="rounded-lg border bg-card text-card-foreground shadow-sm" data-v0-t="card" >
          <div class="p-4">
            <h3 class="text-lg font-medium">{item.name}</h3>
            <p class="text-muted-foreground text-sm">
              {item.description}
            </p>
            <div class="mt-4 flex items-center justify-between">
              <span class="font-medium">{item.price}</span>
              <button
                class="inline-flex items-center justify-center hover:backdrop-brightness-50 whitespace-nowrap rounded-md text-sm font-medium ring-offset-background transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50 border border-input bg-background hover:bg-accent hover:text-accent-foreground h-10 px-4 py-2"
              >
                Me gusta (8)
              </button>
            </div>
          </div>
        </div>
      {/each}
    </div>
  </section>
</div>
