<script lang="ts">
  import Layout from "../../ui/layouts/CenterLayout.svelte";
</script>

<Layout>
  <div class="l-fs">
    <h1 class="c-sidecar">Sidecars</h1>
    <p>
      A <strong><u>work-in-progress</u></strong> project to improve GitHub notifications
      and workflow.
    </p>
  </div>
</Layout>

<style>
  .l-fs {
    display: grid;
    max-width: 300px;
    margin: 0 auto;
    grid-template-columns: 1fr;
    grid-template-rows: 1fr auto;
    grid-column-gap: 0px;
    grid-row-gap: calc(var(--padding) * 2);
    place-items: center;
    text-align: center;
  }

  .l-fs p {
    margin: 0;
  }

  .c-sidecar {
    width: min(48vw, 80%);
    aspect-ratio: 1/1;
    text-indent: -9999px;
    background-image: url("/images/logos/mascot-only.svg");
    background-size: contain;
    background-position: center;
    background-repeat: no-repeat;
    margin: 0;
  }
</style>
