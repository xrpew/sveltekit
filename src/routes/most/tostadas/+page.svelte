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
    { name: "Tostadas clásica", description: "Tostadas masa madre, con mermelada o dulce de leche y mantequilla o queso crema", price: "$4.200" },
                { name: "Tostadas con palta", description: "Tostadas masa madre, con semillas y palta", price: "$6.200" },
                { name: "Tostadas francesas", description: "Pan brioche remojado en batido de la casa, sellado en mantequilla y terminado con crema batida, frutos rojos y espejo de miel de palma.", price: "$6.900" },
                { name: "Tostadas francesas nutella", description: "Pan molde brioche, Nutella, frutos rojos, plátano o ambos", price: "$7.400" },
                { name: "Tostadas francesas frutales", description: "Pan molde brioche, frutas de estación, azúcar flor, dip de miel", price: "$7.100" },
                { name: "Tostón avocado", description: "Pan hogaza de masa madre, palta y huevos revueltos (opcional con salsa holandesa)", price: "$7.200" },
                { name: "Tostón hummus", description: "Pan hogaza de masa madre, hummus, palta, tomates frescos y pesto", price: "$6.700" },
                { name: "Tostón salmón", description: "Pan hogaza de masa madre, palta, huevos revueltos y salmón ahumado", price: "$9.900" },
                { name: "Tostada proteica", description: "Tostada de masa madre, mantequilla de maní o mantequilla de almendras, frutos rojos, plátano o ambos y mix de semillas", price: "$6.500" },
                { name: "Tostadas babaganoush", description: "Pure de berenjenas asadas acompañado de tomates cherry y tostadas masamadre", price: "$6.000" },
                { name: "", description: "** Opción pan sin gluten $2.000", price: "" }
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
