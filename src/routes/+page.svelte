<script>
	import Footer from '$lib/components/Footer.svelte'
	import Hero from '$lib/components/Hero.svelte'
	import Logo from '$lib/components/Logo.svelte'
	import SectionIndicator from '$lib/components/SectionIndicator.svelte'
	import WhatWeDo from '$lib/components/WhatWeDo.svelte'
</script>

<div class='landing'>
	<header>
		<Logo />
		<div class='landing__hero'>
			<Hero />
		</div>
	</header>
	<main>
		<SectionIndicator sectionNumber='01' />
		<WhatWeDo />
	</main>
	<footer>
		<SectionIndicator sectionNumber='02' />
		<div class='landing__footer'>
			<Footer />
		</div>
	</footer>
</div>

<style lang='scss'>
  .landing {
    min-height: 2215px;

    header {
      margin-top: 3rem;

      .landing__hero {
        margin-top: 3.3rem;
      }
    }

    main {
      margin-top: 4rem;
    }

    footer {
      margin-top: 4rem;

      .landing__footer {
        z-index: -99;
      }
    }
  }
</style>
