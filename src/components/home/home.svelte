<script>
  import GitLabel from "../mini/git_label/git_label.svelte";
  import GitParagraph from "../mini/git_paragraph/git_paragraph.svelte";
  const GitLabelProperties = {
    label: "Develop",
    icon: "/icons/GitBranch_ICON.svg",
    circularIcon: "",
    type: "label",
  };
  const GitLabelProperties1 = {
    label: "Develop",
    icon: "/icons/GitBranch_ICON.svg",
    circularIcon: "",
    type: "label",
  };

  const GitCommandProperties1 = {
    label: "git checkout -b feature/about-me",
    icon: "/icons/GitBranch_ICON.svg",
    circularIcon: "/icons/right_arrow_0.svg",
    type: "command",
  };
  const GitParagraphProperties1 = {
    text: "As a full-stack software engineer I enjoy designing highly interactiveuser interfaces that enthuse customers and creating scalable, reliablebackend solutions - but also caring about the other parts that areneeded for a successful software project: Consistency in design, goodplanning of UI and thinking how it affects the UX, Search EngineOptimization and maintaining the software after initial release.",
    icon: "/icons/User_ICON.svg",
  };

  const GitParagraphProperties2 = {
    text: "While I was working for various companies across the globe, I've had the privilege to learn about their unique challenges of creating software that's best suited for their business. Whether it's been in the health care, logistics or finance sector - it's important to know the external influences that may impact the software project, and how the project itself fits into the bigger picture.",
    icon: "/icons/Note_ICON.svg",
  };

  const GitParagraphProperties3 = {
    text: "I have maintained, developed and launched multiple projects from scratch, carrying the development of it's backend and frontend codebases. My current toolset includes TypeScript/JavaScript, React, Vue, Node.js and all the other various frameworks, libraries and technologies related to them.",
    icon: "/icons/Sheets_ICON.svg",
  };
</script>

<!-- hero section  -->
<section class="hero_section">
  <div class="hs__leftdiv">
    <h1>
      Delivering <span>Quality Software</span> <br />
      To Every Place <span>You Want</span>
    </h1>
    <p>
      As a Software Engineer with an eye for design and user experience, I craft
      quality software from front to back - every aspect considered. You can
      call me your Swiss Army Knife in terms of Software.
    </p>

    <div class="hs__btn_container">
      <a href="/" class="btn_primary">
        Contact <img src="/icons/right_arrow.svg" alt="right_arrow" />
      </a>

      <a href="/about" class="btn_outline_white">
        Learn more <img src="/icons/right_arrow.svg" alt="right_arrow" />
      </a>
    </div>
  </div>
</section>

<!-- about section -->
<section class="about_section">
  <div>
    <GitLabel properties={GitLabelProperties} />
    <div class="about_section__first_section">
      <div class="alan_cooper__quate">
        <p>
          “If we want users to like our software, <br /> we should design it to
          behave like <br /> a likeable person.”
          <br />
          <br />
          <span>- Alan Cooper</span>
        </p>
      </div>

      <div>
        <!-- <img src="/home/ShotingStarToLeft.svg" alt="stripes" /> -->
      </div>
    </div>

    <GitLabel properties={GitCommandProperties1} />

    <div class="about_section__second_section">
      <img src="/home/curve.svg" alt="curve" class="curve" />
      <GitLabel properties={GitLabelProperties1} />

      <div class="about_section__second_section__flexbox">
        <div class="as__ss__f__about_me">
          <h2>
            <span>About Me</span> <br />
            Your Partner in <br /> Web Technology
          </h2>
        </div>

        <div>
          <!-- <img src="/home/ShotingStarToRight.svg" alt="stripes" /> -->
        </div>
      </div>

      <div class="about_section__thired_section__flexbox">
        <div>
          <GitParagraph properties={GitParagraphProperties1} />
        </div>
      </div>

      <div class="about_section__fourth_section__flexbox">
        <div>
          <GitParagraph properties={GitParagraphProperties2} />
        </div>
      </div>

      <div class="about_section__fifth_section__flexbox">
        <div>
          <GitParagraph properties={GitParagraphProperties3} />
        </div>
      </div>
    </div>
  </div>
</section>

<!-- works section -->
<section>Works section</section>

<!-- contact section -->
<section>Contact section</section>

<style lang="scss">
  @import "./home.scss";
</style>
