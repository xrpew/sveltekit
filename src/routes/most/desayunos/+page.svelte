<script>
    import ButonSpecial from "../../ButonSpecial.svelte";
   

  const items = [
    {
      imgSrc:
        "https://th.bing.com/th/id/OIP.pRWDM3mDtd8o8-fYWZ4pxQHaE8?rs=1&pid=ImgDetMain",
      title: "Grilled Salmon",
      description:
        "Succulent salmon fillet grilled to perfection, served with a side of roasted vegetables.",
      price: "$24.99",
      likes: 8,
    },
    {
      imgSrc:
        "https://th.bing.com/th/id/OIP.pRWDM3mDtd8o8-fYWZ4pxQHaE8?rs=1&pid=ImgDetMain",
      title: "Lemon Meringue Pie",
      description:
        "A classic lemon meringue pie with a tangy filling and a light, fluffy meringue topping.",
      price: "$12.99",
      likes: 8,
    },
    {
      imgSrc:
        "https://th.bing.com/th/id/OIP.pRWDM3mDtd8o8-fYWZ4pxQHaE8?rs=1&pid=ImgDetMain",
      title: "Lemon Meringue Pie",
      description:
        "A classic lemon meringue pie with a tangy filling and a light, fluffy meringue topping.",
      price: "$12.99",
      likes: 8,
    },
  ];
  const nophoto = [
    { name: "Clásico", description: "Café simple o té orgánico, jugo del día y tostadas clásicas", price: "$8.000" },
                { name: "Avocado", description: "Café simple o té orgánico, jugo del día y tostón avocado", price: "$12.000" },
                { name: "Argento", description: "Café simple o té orgánico, jugo del día y dos medialunas", price: "$8.400" },
                { name: "Croissant", description: "Café simple o té orgánico, jugo del día y un croissant de jamón y queso", price: "$10.500" },
                { name: "Bowl", description: "Café simple o té orgánico, jugo del día y bowl dulce a elección", price: "$12.000" },
                { name: "Prensado", description: "Café simple o té orgánico, jugo del día y prensado jamón y queso", price: "$11.500" },
                { name: "Paila", description: "Café simple o té orgánico, jugo del día y paila de huevos a elección", price: "$10.400" },
                { name: "Dulce", description: "Café simple o té orgánico, jugo y torta del día", price: "$11.000" },
                { name: "Tentación", description: "Café simple o té orgánico, jugo del día, croissant dulce o waffle dulce a elección", price: "$11.500" },
                { name: "*Opción pan sin gluten", description: "", price: "$2.000" }

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
      <!-- {#each items as item}
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
              <ButonSpecial />
            </div>
          </div>
        </div>
      {/each} -->
      {#each nophoto as item}
        <div
          class="rounded-lg border bg-card text-card-foreground shadow-sm"
          data-v0-t="card"
        >
          <div class="p-4">
            <h3 class="text-lg font-medium">{item.name}</h3>
            <p class="text-muted-foreground text-sm">
              {item.description}
            </p>
            <div class="mt-4 flex items-center justify-between">
              <span class="font-medium">{item.price}</span>
              <ButonSpecial />
            </div>
          </div>
        </div>
      {/each}
    </div>
  </section>
</div>
