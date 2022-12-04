<script>
	/* @type {string} */
	export let sectionNumber

</script>

<svg
	width='58'
	height='142'
	xmlns='http://www.w3.org/2000/svg'
	class='indicator'
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

<style>
  .indicator {
  }

  .indicator__line {
    stroke: var(--manatee);
    stroke-width: .02rem;
  }

  .indicator__circle {
    fill: var(--alabaster);
    stroke-width: .02rem;
    stroke: var(--manatee);
    shape-rendering: crispEdges;
  }

  .indicator__number {
    font-size: 1rem;
    text-anchor: middle;
    fill: var(--manatee);
    font-weight: 900;
  }
</style>
