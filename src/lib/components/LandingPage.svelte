<script>
	import LandingPageFooter from '$lib/components/LandingPageFooter.svelte'
	import LandingPageHeader from '$lib/components/LandingPageHeader.svelte'
	import LandingPageMain from '$lib/components/LandingPageMain.svelte'
	import SectionIndicator from '$lib/components/SectionIndicator.svelte'


</script>

<LandingPageHeader />
<SectionIndicator sectionNumber='01' />
<LandingPageMain />
<LandingPageFooter />

<style lang='scss'>
  .version {
    color: var(--malibu);
    font-style: normal;
  }
</style>
