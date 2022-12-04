<script>
	import SectionIndicator from '$lib/components/SectionIndicator.svelte'
	import womanInVideoCallUrl from '$lib/assets/desktop/image-woman-in-videocall.jpg'
	import womanVideoChattingUrl from '$lib/assets/desktop/image-women-videochatting.jpg'
	import manTextingUrl from '$lib/assets/desktop/image-man-texting.jpg'
	import manInMeetingUrl from '$lib/assets/desktop/image-men-in-meeting.jpg'

</script>

<div class='meeting-landing-page'>
	<header class='header'>
		<img
			alt=''
			class='header__logo'
		>
		<div class='hero'>
			<img
				alt=''
				class='hero__image hero__image__left'
			>
			<img
				alt=''
				class='hero__image hero__image__right'
			>
			<div class='hero__cta'>
				<h1
					class='heading-1'
				>
					Group Chat for Everyone
				</h1>
				<p class='normal-text'>
					Meet makes it easy to connect with others face-to-face virtually and collaborate across any device.
				</p>
				<div class='hero__cta__buttons'>
					<button class='button button__primary'>Download <em>v1.3</em></button>
					<button class='button button__secondary'>What is it?</button>
				</div>
			</div>
		</div>
	</header>
	<main class='main'>
		<SectionIndicator sectionNumber='01' />

		<div class='main__images'>
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

		<div class='main__message'>
			Built for modern use
		</div>

		<div class='main__about'>
			<h2>Smarter meetings, all in one place</h2>
			<p>Send messages, share files, show your screen, and record your meetings — all in one workspace. Control who can
				join with invite&#8209;only team access, data encryption, and data export.</p>
		</div>

		<div class='main__section__02'>
			<SectionIndicator sectionNumber='02' />
		</div>
	</main>
	<footer class='footer'>
		<h2 class='footer__heading'>Experience more together</h2>
		<p class='footer__blurb'>
			Stay connected with reliable HD meetings and unlimited one-on-one and group video sessions.
		</p>
		<button class='button footer__button'>
			Download <em>v1.3</em>
		</button>
	</footer>
</div>

<style>
  .meeting-landing-page {
    min-height: 2215px;
  }

  .header {
    display: grid;
    grid-template-rows: repeat(2, auto);
    grid-template-columns: auto;
    margin-top: 3rem;
  }

  .header__logo {
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
  }

  .hero__image {
    grid-row: 1;
    overflow: hidden;
    width: 199px;
    height: 153px;
    object-fit: cover;
  }

  .hero__image__left {
    content: url('$lib/assets/desktop/image-hero-left.png');
    object-position: right;
    justify-self: end;
    grid-column: 1;
  }

  .hero__image__right {
    content: url('$lib/assets/desktop/image-hero-right.png');
    object-position: left;
    grid-column: 3;
    justify-self: start;
  }

  .hero__cta {
    grid-row: 2;
    grid-column: 1 / span 3;
  }

  .hero__cta .heading-1 {
    text-align: center;
    margin-top: 3rem;
    padding: 0 3rem;
  }

  .hero__cta .normal-text {
    text-align: center;
    margin-top: 1.6rem;
    padding: 0 1rem;
  }

  .hero__cta__buttons {
    display: grid;
    grid-template-columns: auto;
    grid-template-rows: repeat(2, auto);
    grid-row-gap: 1.1rem;
    margin-top: 1.8rem;
  }

  .button {
    place-self: center;
    height: 58px;
    padding: 1.2rem 2.5rem;
    border-radius: 2rem;
    color: var(--alabaster);
    font-weight: 900;
    border: none;
  }

  .button em {
    font-style: normal;
    color: var(--malibu);
  }

  .button__primary {
    background-color: var(--hippie-blue);
  }

  .button__secondary {
    background-color: var(--deluge);
    padding: 1rem 1.8rem;
  }

  .main {
    display: grid;
    place-items: center;
    margin-top: 4rem;
  }

  .main__images {
    margin-top: 3.9rem;
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-column-gap: 1.5rem;
    grid-row-gap: 1.5rem;
  }

  .main__images img {
    width: 151px;
    height: 143px;
    border-radius: .5rem;
  }

  .main__message {
    margin-top: 4rem;
    font-size: 1rem;
    letter-spacing: .25rem;
    line-height: 26px;
    font-weight: 900;
    color: var(--hippie-blue);
    text-transform: uppercase;
  }

  .main__about {
    display: grid;
    place-items: center;
    margin: 0 1.6rem;
    text-align: center;
  }

  .main__about h2 {
    margin-top: 1.4rem;
    font-size: 2rem;
    line-height: 36px;
  }

  .main__about p {
    margin-top: 2.2rem;
    line-height: 26px;
    letter-spacing: 0;
    color: var(--manatee);
  }

  .main__section__02 {
    margin-top: 3.9rem;
		z-index: 1;
  }

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
  }

  .footer:before {
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

  .footer__heading {
    margin-top: 5.8rem;
    font-size: 2rem;
    line-height: 36px;
		z-index: 1;
  }

  .footer__blurb {
    margin-top: 1.4rem;
    font-size: 18px;
		z-index: 1;
  }

  .footer__button.button {
    margin-top: 2rem;
    background-color: var(--deluge);
    padding: 1rem 2.6rem;
		z-index: 1;
  }
</style>
