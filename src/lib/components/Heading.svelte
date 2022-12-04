<script>
	export let size = 1
</script>

<div
	role='heading'
	aria-level='{size}'
>
	<slot />
</div>

<style lang='scss'>
  div[role='heading'] {
    color: var(--ebony-clay);
    font-weight: 900;
		text-align: center;

    &[aria-level='1'] {
      font-size: 2.5rem;
      line-height: 2.75rem;
    }
  }

  @media (min-width: 768px) {
    div[role='heading'] {
      &[aria-level='1'] {
        font-size: 3rem;
      }
    }
  }

  @media (min-width: 1440px) {
    div[role='heading'] {
      &[aria-level='1'] {
        font-size: 3rem;
        line-height: 4rem;
      }
    }
  }
</style>
