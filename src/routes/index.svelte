<style lang="scss">
  /* All CSS is scoped by default, so don't worry about interfering with
     other components. */
  .intro-title {
    font-weight: 400;
  }

  .intro-title strong {
    font-weight: 700;
  }

  li {
    margin-bottom: 0.3em;
  }
  li a {
    border-bottom: 1px dotted;
  }

  h2 {
    margin-left: 1em;
  }

  h1 {
    max-width: 20em;
  }

  .penguin-swing {
    position: absolute;
    height: 30rem;
    left: 67%;
    right: 0;
    top: -8rem;
  }
  .button.is-gold {
    background-color: #FDB515;
    color: rgba(0, 0, 0, 0.7);
    border-color: transparent;
  }
</style>

<svelte:head>
  <title>Open Computing Facility at UC Berkeley</title>
  <meta
    name="description"
    content="The Open Computing Facility is an all-volunteer student
    organization dedicated to free and open-source computing for all UC Berkeley
    students." />
</svelte:head>

<section class="hero is-primary">
  <div class="hero-body">
    <div class="container">
      <h1 class="title intro-title">
        <strong>Free Computing</strong>
        for the
        <strong title="go bears">University of California, Berkeley</strong>
        Community
      </h1>
      <h2 class="subtitle">
        <ul>
          <li>
            <a href="/services/lab">a modern computer lab</a>
          </li>
          <li>
            <a href="/services/printing">free printing</a>
          </li>
          <li>
            <a href="/services/web">website hosting</a>
          </li>
          <li>
            <a href="/services/hpc">high performance computing</a>
          </li>
          <li>
            <a href="/services">see all services</a>
          </li>
        </ul>
      </h2>
      <div class="is-hidden-touch">
        <img
          src="https://static.ocf.berkeley.edu/img/penguin-swing.svg"
          alt="penguin wearing blue and gold scarf"
          class="penguin-swing" />
      </div>
      <nav class="intro-buttons">
        <a
          class="button is-warning is-large"
          href="https://github.com/jgthms/bulma/releases/download/0.8.2/bulma-0.8.2.zip">
          <span>
            <span>Create an Account</span>
          </span>
        </a>
        <a
          class="button is-light is-large"
          href="https://bulma.io/documentation">
          <span>
            <span>About the OCF</span>
          </span>
        </a>
      </nav>
    </div>
  </div>
</section>

<section class="section">
  <div class="container">
    <h1 class="title">Lab Status</h1>
    <p>The lab is currently closed, and will not be open today because of Summer Break.</p>
    <nav class="intro-buttons">
      <a
        class="button is-warning is-medium"
        href="https://github.com/jgthms/bulma/releases/download/0.8.2/bulma-0.8.2.zip">
        <span>
          <span>Lab Information</span>
        </span>
      </a>
      <a class="button is-light is-medium" href="https://bulma.io/documentation">
        <span>
          <span>Check Staff Hours</span>
        </span>
      </a>
    </nav>
  </div>
</section>

<section class="section">
  <div class="container">
    <h1 class="title">Join Staff</h1>
    <p>Help us out!</p>
    <nav class="intro-buttons">
      <a
        class="button is-gold is-medium"
        href="https://github.com/jgthms/bulma/releases/download/0.8.2/bulma-0.8.2.zip">
        <span>
          <span>Lab Information</span>
        </span>
      </a>
      <a class="button is-light is-medium" href="https://bulma.io/documentation">
        <span>
          <span>Check Staff Hours</span>
        </span>
      </a>
    </nav>
  </div>
</section>
