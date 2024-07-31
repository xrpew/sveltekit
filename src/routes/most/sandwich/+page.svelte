<script>
  import ButonSpecial from "../../ButonSpecial.svelte";
  import Mininav from "../../Mininav.svelte";

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
    { name: "Prensado", description: "Pan ciabatta de masa madre con mantequilla especiada, jamon y queso.", price: "$6.400" },
                { name: "Especial jamón y queso", description: "pan brioche tostado caliente, queso fundido y jamón.", price: "$6.900" },
                { name: "Especial veggie", description: "pan brioche tostado caliente, queso fundido, cebolla caramelizada y champiñones salteados.", price: "$6.700" },
                { name: "Ave palta", description: "Pan ciabatta de masa madre, pechuga de pollo, mayonesa, palta", price: "$8.300" },
                { name: "Ave pimentón", description: "Pan ciabatta de masa madre, pechuga de pollo y pimenton asado", price: "$8.000" },
                { name: "Pastrami", description: "Tostada masa madre, pastrami, dressing de mostaza miel, encurtidos y rúcula", price: "$9.700" },
                { name: "Sandwich bacon", description: "huevo revuelto, tocino ahúmado y queso fundido, en pan brioche", price:"$9.500"},
                { name: "Croque madame", description: "pan molde masa madre tostado, jamón, queso, bechamel, muzzarella gratinada, terminado con huevo frito.", price: "$9.900" },
                { name: "Veggie sandwich", description: "Pan ciabatta de masa madre, queso fundido, tomate asado y pesto", price: "$7.300" },
                { name: "Vegan sandwich", description: "Pan ciabatta de masa madre, hummus, tomate asado, champiñones y mix verde", price: "$7.500" },
                { name: "*Opción pan ciabatta masa madre", description: "", price: "$1.000" },
                { name: "**Opción pan sin gluten", description: "", price: "$2.000" }
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
