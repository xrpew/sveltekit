<script>
    import { page } from "$app/stores";
    export let segment;
  </script>
  
  <main>
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
            href="/most/cafeteria"
            aria-current={$page.url.pathname === "/most/cafeteria" ? "page" : undefined}
            class="text-sm font-medium hover:underline underline-offset-4 whitespace-nowrap"
          >
            Cafetería
          </a>
          <a
            aria-current={$page.url.pathname === "/most/filtrado" ? "page" : undefined}
            class="text-sm font-medium hover:underline underline-offset-4 whitespace-nowrap"
            href="/most/filtrado"
          >
            Filtrado
          </a>
          <a
            aria-current={$page.url.pathname === "/most/croissant" ? "page" : undefined}
            class="text-sm font-medium hover:underline underline-offset-4 whitespace-nowrap"
            href="/most/croissant"
          >
            Croissant
          </a>
          <a
            aria-current={$page.url.pathname === "/most/waffles" ? "page" : undefined}
            href="/most/waffles"
            class="text-sm font-medium hover:underline underline-offset-4 whitespace-nowrap"
          >
            Waffles
          </a>
          <a
            aria-current={$page.url.pathname === "/most/tostadas" ? "page" : undefined}
            class="text-sm font-medium hover:underline underline-offset-4 whitespace-nowrap"
            href="/most/tostadas"
          >
            Tostadas
          </a>
          <a
            aria-current={$page.url.pathname === "/most/sandwich" ? "page" : undefined}
            class="text-sm font-medium hover:underline underline-offset-4 whitespace-nowrap"
            href="/most/sandwich"
          >
            sandwich
          </a><a
            aria-current={$page.url.pathname === "/most/pailasomelete" ? "page" : undefined}
            class="text-sm font-medium hover:underline underline-offset-4 whitespace-nowrap"
            href="/most/pailasomelete"
          >
              pailas y omelete
          </a>
          <a
            aria-current={$page.url.pathname === "/most/pasteleria" ? "page" : undefined}
            class="text-sm font-medium hover:underline underline-offset-4 whitespace-nowrap"
            href="/most/pasteleria"
          >
            Pasteleria y Bowls
          </a>
          <a
            aria-current={$page.url.pathname === "/most/jugos" ? "page" : undefined}
            class="text-sm font-medium hover:underline underline-offset-4 whitespace-nowrap"
            href="/most/jugos"
          >
            jugos y bebidas
          </a>
          <a
            aria-current={$page.url.pathname === "/most/desayunos" ? "page" : undefined}
            class="text-sm font-medium hover:underline underline-offset-4 whitespace-nowrap"
            href="/most/desayunos"
          >
            Desayunos
          </a>
          <a
            aria-current={$page.url.pathname === "/most/brunch" ? "page" : undefined}
            class="text-sm font-medium hover:underline underline-offset-4 whitespace-nowrap"
            href="/most/brunch"
          >
            brunch
          </a><a
            aria-current={$page.url.pathname === "/most/almuerzos" ? "page" : undefined}
          class="text-sm font-medium hover:underline underline-offset-4 whitespace-nowrap"
          href="/most/almuerzos"
        >
          almuerzos
        </a><a
          aria-current={$page.url.pathname === "/most/tiendita" ? "page" : undefined}
        class="text-sm font-medium hover:underline underline-offset-4 whitespace-nowrap"
        href="/most/tiendita"
      >
        tiendita
      </a>
        </div>
      </nav>
      <slot></slot>
    </main>
    
    
    <style>
      a[aria-current="page"] {
        text-decoration: underline;
      }
    </style>
        