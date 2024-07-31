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
    { name: "Papayo", description: "Origen: Colombia Huila Palestina. <br> Notas: chocolate, berries, anís, canela. <br> Puntaje SCA: 87,5 <br> proceso: honey", price: "" },
                { name: "240ml", description: "", price: "$5.700" },
                { name: "400ml", description: "", price: "$9.800" },
                { name: "La Colombia", description: "Origen: Antioquia, Colombia. <br> Notas: Maracuyá, durazno, chocolate, licoroso. <br> Puntaje SCA: 87 <br> proceso: natural", price: "" },
                { name: "240ml", description: "", price: "$5.700" },
                { name: "400ml", description: "", price: "$9.800" },
                { name: "Pink Bourbon", description: "Origen: Colombia Huila Palestina. <br> Notas: frutas amarillas, caramelo. cítrico, floral. <br> Puntaje SCA: 86,5 <br> proceso: fully washed", price: "" },
                { name: "240ml", description: "", price: "$5.200" },
                { name: "400ml", description: "", price: "$9.300" },
                { name: "Chiroso Honey", description: "Origen: Colombia Antioquia. <br> Notas: cereza, mandarina, caramelo. <br> Puntaje SCA: 87,5 <br> proceso: honey", price: "" },
                { name: "240ml", description: "", price: "$5.700" },
                { name: "400ml", description: "", price: "$9.800" },
                { name: "BRASIL AMA", description: "Origen: Brasil. <br> Notas: Piña madura, licoroso, panela. <br> Puntaje SCA: 87 <br> proceso: Natural", price: "" },
                { name: "240ml", description: "", price: "$5.700" },
                { name: "400ml", description: "", price: "$9.800" },
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
