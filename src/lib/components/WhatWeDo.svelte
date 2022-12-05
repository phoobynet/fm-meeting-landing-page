<script>
	import womanInVideoCallUrl from '$lib/assets/desktop/image-woman-in-videocall.jpg'
	import womanVideoChattingUrl from '$lib/assets/desktop/image-women-videochatting.jpg'
	import manTextingUrl from '$lib/assets/desktop/image-man-texting.jpg'
	import manInMeetingUrl from '$lib/assets/desktop/image-men-in-meeting.jpg'
</script>

<div class='what-we-do'>
	<div class='what-we-do__images'>
		<img
			src={womanInVideoCallUrl}
			alt=''
		>
		<img
			src={womanVideoChattingUrl}
			alt=''
		>
		<img
			src={manInMeetingUrl}
			alt=''
		>

		<img
			src={manTextingUrl}
			alt=''
		/>
	</div>

	<div class='what-we-do__message'>
		Built for modern use
	</div>

	<div class='what-we-do__about'>
		<h2>Smarter meetings, all in one place</h2>
		<p>Send messages, share files, show your screen, and record your meetings — all in one workspace. Control who can
			join with invite&#8209;only team access, data encryption, and data export.</p>
	</div>
</div>

<style lang='scss'>
  .what-we-do {
    display: grid;
    place-items: center;

    &__images {
      margin-top: 3.9rem;
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      grid-column-gap: 1.5rem;
      grid-row-gap: 1.5rem;

      img {
        width: 151px;
        height: 143px;
        border-radius: .5rem;
      }
    }

    &__message {
      margin-top: 4rem;
      font-size: 1rem;
      letter-spacing: .25rem;
      line-height: 26px;
      font-weight: 900;
      color: var(--hippie-blue);
      text-transform: uppercase;
    }

    &__about {
      display: grid;
      place-items: center;
      margin: 0 1.6rem;
      text-align: center;

      h2 {
        margin-top: 1.4rem;
        font-size: 2rem;
        line-height: 36px;
      }

      p {
        margin-top: 2.2rem;
        line-height: 26px;
        letter-spacing: 0;
        color: var(--manatee);
      }
    }
  }
</style>
