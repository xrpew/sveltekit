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
  const nophoto= [
      { name: "Bowl de mar", description: "Mix de hojas verdes, láminas de salmón ahumado, pepino fresco, cubos de palta, semillas de zapallo tostadas, dressing ácida de eneldo", price: "$9.500" },
      { name: "Bowl serrano", description: "Rúcula y mix de hojas verdes, jámon serrano, gajos de naranja a vivo, nueces garrapiñadas, dressing de aceto balsámico y miel", price: "$8.500" },
      { name: "Bowl vegan", description: "Mix verde, champiñones salteados, hummus, cherrys, babaganoush, pepino, palta", price: "$7.900" },
      { name: "Panzottis espinaca o zapallo", description: "Pasta rellena acompañada de salsa pomodoro, rose, pesto o bechamel", price: "$8.900" },
      { name: "Ñoquis", description: "Acompañados de salsa pomodoro, rose, pesto o bechamel", price: "$8.900" },
      { name: "Wok de pollo", description: "Pollo salteado con verduras, soya y arroz", price: "$8.500" },
      { name: "Wrap de pollo", description: "Pollo braseado con queso, verduras asadas, mix de hojas verdes y salsa BBQ", price: "$8.500" },
      { name: "Hojas de parra", description: "Rellenas con carne animal o de soya, arroz jazmín, especias libanesas sobre colchón de hummus y babaganoush, tomates cherris marinados en menta", price: "$12.900" },
      { name: "Sopa crema  (de lunes a viernes)", description: "350 ml de sopa del día", price: "$4.900" },
      { name: "Consulta nuestro menú del día", description: "de lunes a viernes hasta agotar stock", price: "$8.500" },
      ]
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
              <ButonSpecial/>
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
              <ButonSpecial/>

            </div>
          </div>
        </div>
      {/each}
    </div>
  </section>
</div>
