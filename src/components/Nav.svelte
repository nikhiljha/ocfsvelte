<script>
	export let segment;
  let expanded = false;
  let signedin = false;

	function toggleHamburger() {
		expanded = !expanded;
	}

	// a11y, designates current page in nav
	function ariaCurrent(name) {
		return segment === name ? "page" : undefined;
	}
</script>

<nav class="navbar" role="navigation" aria-label="main navigation">
  <div class="navbar-brand">
    <a aria-current='{ariaCurrent(undefined)}' class="navbar-item" href="/">
      <img alt="penguin wearing a blue and yellow scarf" src="logo-text.png" height="28">
    </a>

    <div role="button" class="navbar-burger burger {expanded ? "is-active" : ""}" aria-label="menu" aria-expanded={expanded} on:click={toggleHamburger} data-target="mainNav">
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
    </div>
  </div>

  <div id="mainNav" class="navbar-menu {expanded ? "is-active" : ""}">
    <div class="navbar-start">
      <a aria-current='{ariaCurrent("about")}' class="navbar-item" href="/about">
        About
      </a>

	  <a aria-current='{ariaCurrent("services")}' class="navbar-item" href="/services">
        Services
      </a>

	  <a aria-current='{ariaCurrent("help")}' class="navbar-item" href="/help">
        Help
      </a>
    </div>

    <div class="navbar-end">
      <div class="navbar-item">
        <div class="buttons">
          {#if signedin}
          <a class="button is-primary" href="/account/dashboard">
            <strong>Dashboard</strong>
          </a>
          {:else}
          <a class="button is-primary" href="/account/register">
            <strong>Create Account</strong>
          </a>
          <a class="button is-light" href="/account/login">
            Sign In
          </a>
          {/if}
        </div>
      </div>
    </div>
  </div>
</nav>
