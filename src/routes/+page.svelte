<script>
  import HiddenStar from "$lib/assets/images/hiddenstar-banner.png";
  import HiddenStarLogo from "$lib/assets/images/hiddenstar-logo-no-text.png";
  import HiddenStarLogoText from "$lib/assets/images/hiddenstar-logo.png";
  import LonghornCover from "$lib/assets/images/longhorn-cover.png";
</script>

<main class="container-fluid">
  <header>
    <div class="logo">
      <img src={HiddenStarLogo} alt="The Hidden Star"/>
    </div>
    <h1>THE HIDDEN STAR</h1>
  </header>
    <div class="splash-image">
      <img src={HiddenStar} alt="The Hidden Star"/>
    </div>
    <section class="content-block">
      <div class="title">
        <img src={LonghornCover} alt="Spooky realistic photography. An old shed is set amid pine trees and scrub brush in rural Wyoming. Hilly country. The sun has only just gone down, there is still a bit of light in the air. Everything - the trees, the shed, the scrub - has burned recently in a fire, though no fire remains. Only ashes and charcoal. It looks as if the camera has been set on the ground, looking up the stairs of the shed. A single longhorn cattle skull lies half-charred in the dust." />
        <div>
          <h2>HAUNTING OF LONGHORN RANCH</h2>
          <p class="blockquote">That's just it, man. Fire might burn out, folks might move on. You watch. Give it two weeks and the coverage drops off even the county paper. They'd rather forget about it. It helps them to imagine that once the last of the retardant is poured over the last of the flame, the fire's a thing of the past. No need to worry about it anymore. But ain't a fire ever burned that didn't leave behind embers and ash. Anyone around here can tell you - you don't mind your embers, they're likely to leap into flame again.</p>
        </div>
      </div>
      <a href="https://longhorn.hiddenstar-magazine.com">
        <button class="main-cta">Read the interactive novel that started it all.</button>
      </a>
    </section>
    <section id="matters">
      <hr />
      <article>
        <h3>ABOUT US</h3>
        <p>Hidden Star Magazine is a publisher of interactive fiction with a novel distribution. Our objective is to widen the way in which fiction writing is presented to a wider audience. Our flagship project, Haunting of Longhorn Ranch, is a ten-part interactive horror novel set to release in early September 2024. Hidden Star is primarily a publisher of horror and fantasy tales. We are inspired by the kinds of horror stories that are intricate and complex. We love characters who seem complicated and real, and we believe the best horror stories are ones in which you find empathy between the pages.</p>
        <p>We hope you like our flagship project. We recognize that the rest of this site is relatively empty at the moment. That's just because we haven't done much yet. Someday, we'll have enough projects to fill this page with additional content, but for now there's nothing to read here.</p>
      </article>
      <article>
        <h3>THE LITTLE FREE FRIGHTS PROJECT</h3>
        <p>Hidden Star Magazine has a print distribution system. You can find installations of the print magazine, if you're lucky, in little free libraries throughout Boulder County and, someday, beyond. These printings include novels, periodicals, and assorted other media. Keep an eye out for the Hidden Star logo in these libraries to pick up a limited release copy.</p>
      </article>
      <article>
        <h3>WRITING FOR HIDDEN STAR</h3>
        <p>Hidden Star Magazine is looking for talented writers in the Boulder County area. If you're interested in writing for the Hidden Star, reach out to our email which can be found in the footer. At the moment, Hidden Star is singularly focused on releasing Longhorn Ranch digitally. Our print circulation is taking a backseat to this project, so please excuse any late responses.</p>
      </article>
      <article></article>
    </section>
  <footer>
    <img src={HiddenStarLogoText} alt="A visual representation of an eclipse, including the name of the magazine, Hidden Star.">
  </footer>
</main>

<style>

  main {
    border: 0px;
    margin: 0px;
    padding: 0px;
  }

  .blockquote { 
    font-style: italic;
    border-left: 3px solid #000;
    padding-left: 1rem;
    text-align: justify;
  }

  p {
    text-align: justify;
  }

  .splash-image img {
    width: 100%; /* Ensure the img takes up the full width of the div */
    height: auto; /* Maintain aspect ratio */
  }

  .splash-image {
    position: fixed;
    width: 85%;
    top: 6rem;  /* Or wherever you want the image to be vertically positioned */
    height: 80vh;
    overflow: hidden;
    left: 50%;
    transform: translateX(-50%); /* Centers the image horizontally */
    z-index: -1; /* Ensures it stays behind other content */
  }

  h1, h2 {
    text-transform: uppercase;
    font-family: "Cormorant Garamond", serif;
    z-index: 2;
  }

  p {
    font-family: "Cormorant Garamond", serif;
    z-index: 2;
  }

  .content-block {
    background-color: #f0f0f0;
    padding: 1.5rem;
    padding-left: 6rem;
    z-index: 2;
    max-width: 50vw;
    flex-grow: 1;
    margin-left: 2rem;
    margin-top: 15rem;
    padding-bottom: 15rem;
  }

  main {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: left;
    height: 100vh;
  }

  header {
    display: flex;
    align-items: center;
    width: 100%;
    height: 10vh;
    background-color: #f0f0f0;
  }

  .logo img {
    width: 3rem;
    padding: 1rem;
  }

  .title {
    display: flex;
  }

  .title img {
    padding-right: 1rem;
    height: 15rem;
  }

  .title h2 {
    font-size: 2.5rem;
    margin: 0rem;
  }

  #matters {
    background-color: #f0f0f0;
    margin: 0 auto;
    padding: 1.5rem;
    width: 85%;
  }

  article {
    margin: 0 auto;
    padding: 1rem;
  }

  footer {
    display: flex;
    align-items: center;
    width: 100%;
    background-color: #1f1d18;
  }

  footer img {
    height: 5rem;
  }

  .main-cta {
    background-color: #f0f0f0;
    border: none;
    outline: none;
    font-family: "Cormorant Garamond", serif;
    font-size: 1rem;
    border-right: 3px solid #000;
    padding-right: 1rem;
    text-transform: uppercase;
    float: right;
    cursor: pointer;
  }

    /* viewframes for mobile */
    @media only screen and (max-width: 1060px) { /* Adjust the breakpoint as needed */
      .splash-image {
        top: 4rem; /* Adjust the vertical position as needed */
      }

      p {
        font-size: 0.75rem;
      }

      .splash-image {
        height: 100vh;
        width: 100%;
        overflow: hidden;
      }

      #matters {
        width: 90%;
      }

      .splash-image img {
        height: 300rem;
        width: auto;
      }
     
      .content-block {
        width: 100%; /* Full-screen width on mobile */
        margin: 0 auto;
        margin-top: 3rem;
        padding: 1rem; /* Optional: add some padding for better readability */
        height: auto; /* Let it adjust based on content, or keep full height if preferred */
      }

      .title img {
        /* display: none; */
        height: 10rem;
        padding-left: 0rem;
      }

      .title h2 {
        font-size: 1.5rem;
      }

      main {
        overflow-x: hidden;
      }
    }

    @media only screen and (max-width: 550px) { /* Adjust the breakpoint as needed */
      .title img {
        display: none;
      }
    }
</style>