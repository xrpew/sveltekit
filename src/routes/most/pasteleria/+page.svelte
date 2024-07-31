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
    { name: "Medialuna argentina", description: "", price: "$2.000" },
                { name: "Medialuna rellena", description: "Con pastelera o dulce de leche", price: "$2.400" },
                { name: "Porción queque", description: "(consultar disponibilidad)", price: "$2.900" },
                { name: "Cookie", description: "(consultar disponibilidad)", price: "$2.800" },
                { name: "Cookie sin azucar", description: "(consultar disponibilidad)", price: "$2.300" },
                { name: "Porción de trufas", description: "", price: "$2.500" },
                { name: "Rollo de canela", description: "", price: "$3.200" },
                { name: "Alfajor brownie", description: "bases de brownie rellenas con dulce de leche", price: "$3.900" },
                { name: "Alfajor de maicena", description: "", price: "$2.600" },
                { name: "Alfajor de coco", description: "", price: "$2.600" },
                { name: "Brownie", description: "", price: "$3.200" },
                { name: "Brownie con helado", description: "", price: "$4.900" },
                { name: "Banoffee", description: "", price: "$4.900" },
                { name: "Chocotorta", description: "", price: "$4.700" },
                { name: "Cheesecake", description: "", price: "$4.900" },
                { name: "Carrot cake", description: "", price: "$4.900" },
                { name: "Lemon pie", description: "", price: "$4.900" },
                { name: "Torta húmeda de chocolate", description: "bizcocho de cacao húmedo relleno con dulce de leche, bañanado en ganache bitter", price: "$5.700" },
                { name: "Torta brownie", description: "bizcocho a base de brownie, dulce de leche y merengue", price: "$5.700" },
                { name: "Porción de frutas de estación", description: " con dip de miel", price: "$4.300" },
                { name: "Vegancito", description: "lingote de bizcocho de vainilla cubierto de chocolate bitter, relleno de gel de frambuesa decorado con chantilly (todos los componentes de origen vegetal)", price: "$3.600" },
                { name: "Bowl ipanema", description: "Acai, arándanos, fruta de la estación, plátano, granola, coco y mantequilla de mani", price: "$7.900" },
                { name: "Bowl natural", description: "Yogurt natural, granola, frutas de estación y miel", price: "$6.600" },
                { name: "Bowl porridge invernal", description: "Avena integral cocida en leche vegetal con manzana, canela y nueces, con topping de frutas, coco y miel", price: "$6.600" },
                { name: "Rawnie clásico o naranja", description: "Caramelo de naranja crunchy a base de mantequilla de maní sobre bizcocho de dátiles y cacao cubierto de chocolate bitter", price: "$2.900" },
                { name: "Caluga", description: "Suave nougat de nuez y dátiles con toques de vainilla, café y coco, cubierto con chocolate bitter y topping de nuez crocante", price: "$2.900" }
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
