<script>
	import Button from '$lib/components/Button.svelte'
</script>

<footer class='footer'>
	<div style='z-index: 1'>
		<h2 class='footer__heading'>Experience more together</h2>
		<p class='footer__blurb'>
			Stay connected with reliable HD meetings and unlimited one-on-one and group video sessions.
		</p>
		<Button
			kind='primary'
			class='footer__content'
		>
			Download <em class='version'>v1.3</em>
		</Button>
	</div>
</footer>

<style lang='scss'>
  .footer {
    position: relative;
    margin-top: -2rem;
    display: flex;
    flex-direction: column;
    justify-items: center;
    height: 428px;
    background-color: var(--hippie-blue);
    color: var(--alabaster);
    text-align: center;
    padding: 0 1.6rem;

    &:before {
      content: ' ';
      display: block;
      position: absolute;
      left: 0;
      top: 0;
      width: 100%;
      height: 100%;
      opacity: 0.1;
      background-image: url('$lib/assets/mobile/image-footer.jpg');
      background-repeat: no-repeat;
      background-position: 50% 0;
      background-size: cover;
      background-blend-mode: multiply;
    }

    &__content {
      z-index: 1;
    }

    &__heading {
      @extend .footer__content;
      margin-top: 5.8rem;
      font-size: 2rem;
      line-height: 36px;
    }

    &__blurb {
      @extend .footer__content;
      margin-top: 1.4rem;
      font-size: 18px;
    }
  }
</style>
