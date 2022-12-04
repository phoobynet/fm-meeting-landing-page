<script>
	import Button from '$lib/components/Button.svelte'
	import Heading from '$lib/components/Heading.svelte'
</script>

<header class='header'>
	<img
		alt=''
		class='header__logo'
	>
	<div class='hero'>
		<img
			alt=''
			class='hero__image__left'
		>
		<img
			alt=''
			class='hero__image__right'
		>
		<div class='hero__cta'>
			<Heading size='1'>
				Group Chat for Everyone
			</Heading>
			<p class='normal-text'>
				Meet makes it easy to connect with others face-to-face virtually and collaborate across any device.
			</p>
			<div class='hero__cta__buttons'>
				<Button kind='primary'>
					Download <em class='version'>v1.3</em>
				</Button>
				<Button kind='secondary'>
					What is it?
				</Button>
			</div>
		</div>
	</div>
</header>

<style lang='scss'>
  .header {
    display: grid;
    grid-template-rows: repeat(2, auto);
    grid-template-columns: auto;
    margin-top: 3rem;

    .version {
      color: var(--malibu);
      font-style: normal;
    }

    &__logo {
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

      &__image {
        grid-row: 1;
        overflow: hidden;
        width: 199px;
        height: 153px;
        object-fit: cover;

        &__left {
          @extend .hero__image;
          content: url('$lib/assets/desktop/image-hero-left.png');
          object-position: right;
          justify-self: end;
          grid-column: 1;
        }

        &__right {
          @extend .hero__image;
          content: url('$lib/assets/desktop/image-hero-right.png');
          object-position: left;
          grid-column: 3;
          justify-self: start;
        }
      }


      &__cta {
				margin-top: 3rem;
        grid-row: 2;
        grid-column: 1 / span 3;

        &__buttons {
          display: grid;
          grid-template-columns: auto;
          grid-template-rows: repeat(2, auto);
          grid-row-gap: 1.1rem;
          margin-top: 1.8rem;
        }

        .heading-1 {
          text-align: center;
          margin-top: 3rem;
          padding: 0 3rem;
        }

        .normal-text {
          text-align: center;
          margin-top: 1.6rem;
          padding: 0 1rem;
        }
      }
    }
  }
</style>
