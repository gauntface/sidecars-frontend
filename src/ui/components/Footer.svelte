<script lang="ts">
  import SigninButton from "./SigninButton.svelte";
</script>

<footer>
  <div class="l-rows">
    <div>
      <h5>Useful Links</h5>
      <ul>
        <li><a href="/">Home</a></li>
        <li><a href="https://www.buymeacoffee.com/gauntface" target="_blank">Support this Project</a></li>
        <li><a href="https://app.beampipe.io/domain/sidecars.dev" target="_blank">Analytics</a></li>
				<li><SigninButton modifier="highlight" /></li>
      </ul>
    </div>
    <div>
      <h5>Policy</h5>
      <ul>
        <li><a href="/privacy">Privary Policy</a></li>
        <li><a href="/cookies">Cookies</a></li>
      </ul>
    </div>
    <div>
      <h5>Get in Touch</h5>
      <ul>
        <li><a href="https://github.com/gauntface/sidecars-frontend/issues/new">Found a bug?</a></li>
        <li><a href="mailto:sidecars@gaunt.dev">E-mail</a></li>
      </ul>
    </div>
  </div>
  <p>© All rights reserved {new Date().getFullYear()}</p>
</footer>

<style>
	footer {
		width: 100%;
		background: var(--color-secondary);
		container-type: inline-size;
		margin: var(--xl-padding) auto 0 auto;
	}

	footer p {
		margin: var(--l-padding) auto;
		text-align: center;
	}

	footer ul {
		list-style: none;
		margin: 0;
		padding: 0;
	}

	footer li {
		margin: var(--s-padding) 0;
	}

	footer h5 {
		font-size: 1rem;
    margin-top: 0;
    margin-bottom: 1.2lh;
	}

	.l-rows {
		width: var(--width);
		margin: var(--l-padding) auto;
		border-bottom: solid;
    border-color: rgba(255,255,255,.2);
    border-width: 1px;
	}

	.l-rows > div {
		margin-bottom: var(--xl-padding);
	}

	@container (min-width: 520px) {
		.l-rows {
				display: flex;
				flex-direction: row;
				justify-content: space-between;
		}
	}
</style>
