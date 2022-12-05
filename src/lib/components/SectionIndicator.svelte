<script>
	/* @type {string} */
	export let sectionNumber
</script>

<div class='indicator'>
	<svg
		width='58'
		height='142'
		xmlns='http://www.w3.org/2000/svg'
	>

		<line
			x1='28'
			y1='0'
			x2='28'
			y2='84'
			class='indicator__line'
		/>

		<circle
			cx='29'
			cy='112'
			r='28'
			class='indicator__circle'
		/>

		<text
			x='29'
			y='118'
			class='indicator__number'
		>{sectionNumber}
		</text>
	</svg>
</div>

<style lang='scss'>
  $stroke-width: 0.05rem;
  $stroke-color: var(--manatee);

  .indicator {
		display: flex;
		justify-content: center;

    &__shape {
      stroke: $stroke-color;
      stroke-width: $stroke-width;
    }

    &__line {
      @extend .indicator__shape;
    }

    &__circle {
      @extend .indicator__shape;
      fill: var(--alabaster);
    }

    &__number {
      font-size: 1rem;
      text-anchor: middle;
      fill: $stroke-color;
      font-weight: 900;
    }
  }

</style>
