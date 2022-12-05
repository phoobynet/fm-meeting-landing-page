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
		<Hero />
	</header>
	<main>
		<SectionIndicator sectionNumber='01' />
		<WhatWeDo />
	</main>
	<footer>
		<SectionIndicator sectionNumber='02' />
		<Footer />
	</footer>
</div>

<style lang='scss'>
  .landing {
    min-height: 2215px;

    header {
      margin-top: 3rem;
    }

    main {
      display: flex;
      justify-content: center;
      margin-top: 4rem;
    }
  }
</style>
