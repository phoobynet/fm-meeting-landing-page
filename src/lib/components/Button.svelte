<script>
	/*
	 * @typedef {"primary" | "secondary} ButtonKind
	*/

	/* @type {ButtonKind} */
	export let kind = 'primary'
</script>

<button class='{`btn__${kind}`}'>
	<slot></slot>
</button>

<style lang="scss">
  .btn {
    place-self: center;
    height: 3.62rem;
    padding: 1.1rem 2.5rem;
    border-radius: 2rem;
    color: var(--alabaster);
    font-weight: 900;
    border: none;

    &__primary {
      @extend .btn;
      background-color: var(--hippie-blue);
    }

    &__secondary {
      @extend .btn;
      background-color: var(--deluge);
      padding: 1rem 1.8rem;
    }
  }
</style>
