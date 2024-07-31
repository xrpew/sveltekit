<script>
  import { page } from "$app/stores";
</script>

<nav
  class="bg-slate-400 py-2 px-4 md:px-6 sticky top-[4rem] z-10 overflow-x-auto scrollbar-thin scrollbar-thumb-muted-foreground scrollbar-track-transparent"
>
  <div class="container mx-auto flex gap-4">
    <a
    aria-current={$page.url.pathname === "/most" ? "page" : undefined}
      class="text-sm font-medium active:underline hover:underline underline-offset-4 whitespace-nowrap"
      href="/most"
    >
      Lo más pedido
    </a>

    <a
      href="/cafeteria"
      aria-current={$page.url.pathname === "/cafeteria" ? "page" : undefined}
      class="text-sm font-medium hover:underline underline-offset-4 whitespace-nowrap"
    >
      Cafetería
    </a>
    <a
      aria-current={$page.url.pathname === "/filtrado" ? "page" : undefined}
      class="text-sm font-medium hover:underline underline-offset-4 whitespace-nowrap"
      href="/filtrado"
    >
      Filtrado
    </a>
    <a
      aria-current={$page.url.pathname === "/croissant" ? "page" : undefined}
      class="text-sm font-medium hover:underline underline-offset-4 whitespace-nowrap"
      href="/croissant"
    >
      Croissant
    </a>
    <a
      aria-current={$page.url.pathname === "/waffles" ? "page" : undefined}
      href="/waffles"
      class="text-sm font-medium hover:underline underline-offset-4 whitespace-nowrap"
    >
      Waffles
    </a>
    <a
      aria-current={$page.url.pathname === "/tostadas" ? "page" : undefined}
      class="text-sm font-medium hover:underline underline-offset-4 whitespace-nowrap"
      href="/tostadas"
    >
      Tostadas
    </a>
    <a
      aria-current={$page.url.pathname === "/sandwich" ? "page" : undefined}
      class="text-sm font-medium hover:underline underline-offset-4 whitespace-nowrap"
      href="/sandwich"
    >
      sandwich
    </a><a
      aria-current={$page.url.pathname === "/pailasomelete" ? "page" : undefined}
      class="text-sm font-medium hover:underline underline-offset-4 whitespace-nowrap"
      href="pailasomelete"
    >
        pailas y omelete
    </a>
    <a
      aria-current={$page.url.pathname === "/pasteleria" ? "page" : undefined}
      class="text-sm font-medium hover:underline underline-offset-4 whitespace-nowrap"
      href="/pasteleria"
    >
      Pasteleria y Bowls
    </a>
    <a
      aria-current={$page.url.pathname === "/jugos" ? "page" : undefined}
      class="text-sm font-medium hover:underline underline-offset-4 whitespace-nowrap"
      href="/jugos"
    >
      jugos y bebidas
    </a>
    <a
      aria-current={$page.url.pathname === "/desayunos" ? "page" : undefined}
      class="text-sm font-medium hover:underline underline-offset-4 whitespace-nowrap"
      href="/desayunos"
    >
      Desayunos
    </a>
    <a
      aria-current={$page.url.pathname === "/brunch" ? "page" : undefined}
      class="text-sm font-medium hover:underline underline-offset-4 whitespace-nowrap"
      href="/brunch"
    >
      brunch
    </a><a
      aria-current={$page.url.pathname === "/almuerzos" ? "page" : undefined}
    class="text-sm font-medium hover:underline underline-offset-4 whitespace-nowrap"
    href="/almuerzos"
  >
    almuerzos
  </a><a
    aria-current={$page.url.pathname === "/tiendita" ? "page" : undefined}
  class="text-sm font-medium hover:underline underline-offset-4 whitespace-nowrap"
  href="/tiendita"
>
  tiendita
</a>
  </div>
</nav>

<style>
  a[aria-current="page"] {
    text-decoration: underline;
  }
</style>
