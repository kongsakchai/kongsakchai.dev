<script lang="ts">
  import "./styles.css";
  import "@fontsource/nunito/400.css";
  import "@fontsource/nunito/500.css";
  import "@fontsource/nunito/700.css";
  import "@fontsource/nunito/700-italic.css";
  import Navbar from "@components/layout/navbar.svelte";
  import { navigating, page } from "$app/stores";
</script>

{#if $page.url.pathname !== "/intro"}
  <Navbar path={$page.url.pathname} />
{/if}

<slot />
