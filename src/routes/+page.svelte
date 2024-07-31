<script>
  import ButonSpecial from "./ButonSpecial.svelte";
  import Mininav from "./Mininav.svelte";
</script>

<svelte:head>
  <title>El pasaje</title>
  <meta name="description" content="About this app" />
  <script src="https://cdn.tailwindcss.com"></script>
</svelte:head>

<section
  class="container px-4 md:px-6 flex flex-col items-center justify-center gap-8 lg:max-w-[70%] sm:max-w-[90%] mx-auto  lg:h-[90vh]"
>
  <br />

  <div
    id="sectionItemsContent"
    class="grid grid-cols-1 sm:grid-cols-1 lg:grid-cols-1 gap-6 "
  >

    <div
      class="rounded-lg border bg-card text-card-foreground shadow-sm"
      data-v0-t="card"
    >
      <img
        src="https://th.bing.com/th/id/OIP.pRWDM3mDtd8o8-fYWZ4pxQHaE8?rs=1&pid=ImgDetMain"
        width="150"
        height="100"
        alt="Dish"
        class="rounded-t-md object-cover w-[100%]"
      />
      <div class="p-4">
        <div class="mt-4 flex items-center justify-between">
          <button
            class="inline-flex items-center justify-center hover:backdrop-brightness-50 whitespace-nowrap rounded-md text-sm font-medium ring-offset-background transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50 border border-input bg-background hover:bg-accent hover:text-accent-foreground w-[100%] px-4 py-2"
          > <a href="/most">
            IR AL MENÚ
          </a>
		</button>
        </div>
      </div>
    </div>
  </div>
  <br />
</section>

  <section class="w-full py-12 md:py-24 lg:py-32 bg-muted">
    <div class="container grid grid-cols-1 md:grid-cols-2 gap-6 px-4 md:px-6">
      <img
        src="https://th.bing.com/th/id/OIP.jHvTOSF7924Ah63W7mozxQHaEo?rs=1&pid=ImgDetMain"
        alt="Image"
        class="mx-auto aspect-video overflow-hidden rounded-xl object-cover"
      />
      <div class="flex flex-col justify-center space-y-4">
        <h2 class="text-3xl font-bold tracking-tighter md:text-4xl/tight">Texto debajo de la imagen</h2>
        <p class="max-w-[600px] text-muted-foreground md:text-xl/relaxed lg:text-base/relaxed xl:text-xl/relaxed">
          Descripción del texto debajo de la imagen.
        </p>
      </div>
    </div>
  </section>
  <section
  class="container px-4 md:px-6 flex flex-col items-center gap-8 lg:max-w-[70%] sm:max-w-[90%] mx-auto"
>
  <div
    id="sectionItemsContent"
    class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-2 gap-6"
  >
    <div
      class="rounded-lg border bg-card text-card-foreground shadow-sm"
      data-v0-t="card"
    >
      <img
        src="https://th.bing.com/th/id/OIP.pRWDM3mDtd8o8-fYWZ4pxQHaE8?rs=1&pid=ImgDetMain"
        width="150"
        height="100"
        alt="Dish"
        class="rounded-t-md object-cover w-[100%]"
      />
      <div class="p-4">
        <h3 class="text-lg font-medium">Grilled Salmon</h3>
        <p class="text-muted-foreground text-sm">
          Succulent salmon fillet grilled to perfection, served with a side of
          roasted vegetables.
        </p>
        <div class="mt-4 flex items-center justify-between">
          <span class="font-medium">$24.99</span>
          <ButonSpecial/>
        </div>
      </div>
    </div>

    <div class="grid gap-6">
      <div
        class="rounded-lg border bg-card text-card-foreground shadow-sm"
        data-v0-t="card"
      >
        <div class="p-4">
          <h3 class="text-lg font-medium">Chocolasste Mousse</h3>
          <p class="text-muted-foreground text-sm">
            Decadent chocolate mousse topped with a light whipped cream and
            shaved chocolate.
          </p>
          <div class="mt-4 flex items-center justify-between">
            <span class="font-medium">$8.99</span>
            <ButonSpecial/>
          </div>
        </div>
      </div>
      <div
        class="rounded-lg border bg-card text-card-foreground shadow-sm"
        data-v0-t="card"
      >
        <div class="p-4">
          <h3 class="text-lg font-medium">Chocolate Mousse</h3>
          <p class="text-muted-foreground text-sm">
            Decadent chocolate mousse topped with a light whipped cream and
            shaved chocolate.
          </p>
          <div class="mt-4 flex items-center justify-between">
            <span class="font-medium">$8.99</span>
            <ButonSpecial/>
          </div>
        </div>
      </div>
    </div>
    <div class="grid gap-6">
      <div
        class="rounded-lg border bg-card text-card-foreground shadow-sm"
        data-v0-t="card"
      >
        <div class="p-4">
          <h3 class="text-lg font-medium">Chocolate Mousse</h3>
          <p class="text-muted-foreground text-sm">
            Decadent chocolate mousse topped with a light whipped cream and
            shaved chocolate.
          </p>
          <div class="mt-4 flex items-center justify-between">
            <span class="font-medium">$8.99</span>
            <ButonSpecial/>
          </div>
        </div>
      </div>
      <div
        class="rounded-lg border bg-card text-card-foreground shadow-sm"
        data-v0-t="card"
      >
        <div class="p-4">
          <h3 class="text-lg font-medium">Chocolate Mousse</h3>
          <p class="text-muted-foreground text-sm">
            Decadent chocolate mousse topped with a light whipped cream and
            shaved chocolate.
          </p>
          <div class="mt-4 flex items-center justify-between">
            <span class="font-medium">$8.99</span>
            <ButonSpecial/>
          </div>
        </div>
      </div>
    </div>
    <div
    class="rounded-lg border bg-card text-card-foreground shadow-sm"
    data-v0-t="card"
  >
    <img
      src="https://th.bing.com/th/id/OIP.pRWDM3mDtd8o8-fYWZ4pxQHaE8?rs=1&pid=ImgDetMain"
      width="300"
  loading="lazy"
      height="200"
      alt="Dish"
      style=""
      class="rounded-t-md object-cover w-[100%]"
    />
    <div class="p-4">
      <h3 class="text-lg font-medium">Lemon Meringue Pie</h3>
      <p class="text-muted-foreground text-sm">
        A classic lemon meringue pie with a tangy filling and a light, fluffy
        meringue topping.
      </p>
      <div class="mt-4 flex items-center justify-between">
        <span class="font-medium">$12.99</span>
        <ButonSpecial/>
      </div>
    </div>
  </div>


  <br />
</section>
