<div class='meeting-landing-page'>
	<header class='header'>
		<img
			alt=''
			class='header__logo'
		>
		<div class='hero'>
			<img
				alt=''
				class='hero__image hero__image__left'
			>
			<img
				alt=''
				class='hero__image hero__image__right'
			>
			<div class='hero__cta'>
				<h1
					class='heading-1'
				>
					Group Chat for Everyone
				</h1>
				<p class='normal-text'>
					Meet makes it easy to connect with others face-to-face virtually and collaborate across any device.
				</p>
				<div class='hero__cta__buttons'>
					<button class='button button__primary'>Download <em>v1.3</em></button>
					<button class='button button__secondary'>What is it?</button>
				</div>
			</div>
		</div>
	</header>
	<main>

	</main>
</div>

<style>
  .meeting-landing-page {
  }

  .header {
    display: grid;
    grid-template-rows: repeat(2, auto);
    grid-template-columns: auto;
    margin-top: 3rem;
  }

  .header__logo {
    content: url('$lib/assets/logo.svg');
    width: 119px;
    height: 28px;
    grid-row: 1;
    grid-column: 1;
    justify-self: center;
  }

  .hero {
    display: grid;
    margin-top: 3.4rem;
    grid-template-columns: 1fr 0 1fr;
    grid-template-rows: repeat(2, auto);
    grid-column-gap: 0.5rem;
  }

  .hero__image {
    grid-row: 1;
    overflow: hidden;
    width: 199px;
    height: 153px;
    object-fit: cover;
  }

  .hero__image__left {
    content: url('$lib/assets/desktop/image-hero-left.png');
    object-position: right;
    grid-column: 1;
  }

  .hero__image__right {
    content: url('$lib/assets/desktop/image-hero-right.png');
    object-position: left;
    grid-column: 3;
  }

  .hero__cta {
    grid-row: 2;
    grid-column: 1 / span 3;
  }

  .hero__cta .heading-1 {
    text-align: center;
    margin-top: 3rem;
    padding: 0 3rem;
  }

  .hero__cta .normal-text {
    text-align: center;
    margin-top: 1.6rem;
    padding: 0 1rem;
  }

	.hero__cta__buttons {
		display: flex;
		width: auto;
		flex-direction: column;
		justify-content: center;
		margin-top: 2rem;
	}

  .button {
    padding: 1rem 2rem;
    border-radius: 2rem;
    color: var(--alabaster);
    font-weight: 900;
    border: none;
  }

  .button em {
    font-style: normal;
    color: var(--malibu);
  }

  .button__primary {
    background-color: var(--hippie-blue);
  }

  .button__secondary {
    background-color: var(--deluge);
  }
</style>
