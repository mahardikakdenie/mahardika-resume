<template>
  <div class="my-auto">
    <h1 class="mb-0">
      {{ $t("personalInfo.name") }}
      <span class="text-primary">{{ $t("personalInfo.lastName") }}</span>
    </h1>

    <h3 class="mb-4">
      <vue-typer
        :text="$t('personalInfo.subHeadingText')"
        :repeat="Infinity"
        :shuffle="true"
        initial-action="typing"
        :pre-type-delay="100"
        :type-delay="82"
        :pre-erase-delay="2000"
        :erase-delay="30"
        erase-style="backspace"
        :erase-on-complete="false"
        caret-animation="blink"
      ></vue-typer>
    </h3>

    <div class="subheading mb-2">
      {{ $t("personalInfo.city") }} · {{ $t("personalInfo.phoneNumber") }} ·
      <a href="mailto:name@email.com">{{ $t("personalInfo.email") }}</a>
    </div>
    <p class="mb-5">
      I'm Mahardika Kessuma Denie, a young man who really likes programming, I
      think programming is something fun, I'm a person who really likes to
      learn, diligent, persistent, and serious, and confident, I've been doing
      website programming for 2 years by creating APIs or apalication Program
      interface using Laravel as a PHP framework and create responsive website
      programs using Vue js as a javascript library that I master So much from
      me, thanks
    </p>
    <ul class="list-inline list-social-icons mb-0">
      <!-- <li class="list-inline-item">
        <a href="#">
          <span class="fa-stack fa-lg">
            <i class="fas fa-circle fa-stack-2x"></i>
            <i class="fab fa-facebook-f fa-stack-1x fa-inverse"></i>
          </span>
        </a>
      </li> -->

      <li class="list-inline-item">
        <a target="blank" :href="$t('personalInfo.linkedin')">
          <span class="fa-stack fa-lg">
            <i class="fas fa-circle fa-stack-2x"></i>
            <i class="fab fa-linkedin-in fa-stack-1x fa-inverse"></i>
          </span>
        </a>
      </li>
      <li class="list-inline-item">
        <a target="blank" :href="$t('personalInfo.github')">
          <span class="fa-stack fa-lg">
            <i class="fas fa-circle fa-stack-2x"></i>
            <i class="fab fa-github-alt fa-stack-1x fa-inverse"></i>
          </span>
        </a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
};
</script>
