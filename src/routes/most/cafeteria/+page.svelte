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
    { name: "Americano", description: "espresso, agua", price: "$2.500" },
                { name: "Espresso", description: "25-30 ml de extracción de café", price: "$2.300" },
                { name: "Macchiatto", description: "espresso, espuma de leche", price: "$2.700" },
                { name: "After eight", description: "espresso, leche texturizada, menta y chocolate", price: "$4.900" },
                { name: "Capuccino", description: "espresso, leche", price: "$2.900" },
                { name: "Mocaccino", description: "doble espresso, leche, chocolate", price: "$4.100" },
                { name: "Flat white", description: "doble espresso, leche", price: "$3.500" },
                { name: "Latte", description: "espresso, doble carga de leche", price: "$3.400" },
                { name: "Latte saborizado", description: "espresso, leche, vainilla o chocolate o caramelo", price: "$4.000" },
                { name: "Matcha latte", description: "té verde pulverizado alto en antioxidantes, L-teanina y leche", price: "$4.400" },
                { name: "Matcha chai latte", description: "té matcha especiado con jengibre, canela, cardamomo, pimienta, aromatizado con vainilla y leche", price: "$4.900" },
                { name: "Chai latte", description: "té especiado con canela, cardamomo, pimienta y leche texturizada", price: "$4.400" },
                { name: "Chai latte flamingo", description: "té especiado con canela, cardamomo, pimienta, aromatizado con vainilla, sin azúcar, descafeinado y leche", price: "$4.400" },
                { name: "Chocolate caliente espeso", description: "60ml de chocolate liberté, 200ml de leche y marshmallow", price: "$4.900" },
                { name: "Chocolate caliente", description: "30ml de chocolate liberté y 200ml de leche", price: "$4.400" },
                { name: "Chocolate cream", description: "30ml de chocolate liberté, 200ml de leche, terminado con crema chantilly.", price: "$5.200" },
                { name: "Café bombóm", description: "60ml espresso, leche condensada, espuma de leche, terminado con canela.", price: "$4.700" },
                { name: "Capuccino nutella", description: "60ml espresso, leche, espuma de leche, terminado con borde de Nutella y almendras trozadas", price: "$4.900" },
                { name: "Té orgánico variedades", description: "(english breakfast, earl grey, chai masala, rooibos, rooibos naranja, verde jazmín, berries, manzanilla)", price: "$3.000" },                
                { name: "Espresso tonic", description: "doble extracción de café, tónica, hielo", price: "$4.000" },
                { name: "Espresso naranja", description: "25-30 ml de extracción de café, naranja, hielo", price: "$4.300" },
                { name: "Café helado", description: "25-30 ml de extracción de café, helado de vainilla, leche, crema batida y syrup de chocholate", price: "$5.200" },
                { name: "Affogato", description: "doble espresso y helado de vainilla", price: "$4.200" },
                { name: "Cold brew", description: "extracción en frio de café que se realiza durante un periodo de tiempo entre 12 y 24 horas", price: "$3.600" },
                { name: "Vaso de cookie", description: "solo se puede agregar adicional a: affogato, chocolate caliente, espresso y macchiatto", price: "$2.000" },
                { name: "Vaso de cookie dulce de leche", description: "con dulce de leche en su interior -solo se puede agregar adicional a: affogato, chocolate caliente, espresso y macchiatto", price: "$2.300" },
                { name: "Agregado extracción de café", description: "", price: "$600" },
                { name: "Extras", description: "-Leche de almendras -leche de avena -leche de soya -syrup vainilla -syrup caramelo -syrup -menta -crema", price: "$700", tipe:"" },
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
      class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-6"
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
              <span class="font-bold">{item.tipe ? item.tipe : ''}</span>
              <!-- <ButonSpecial /> -->
            </div>
          </div>
        </div>
      {/each}
    </div>
  </section>
</div>
