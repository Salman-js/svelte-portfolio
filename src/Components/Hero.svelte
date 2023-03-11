<script>
  import FooterSvg from '../assets/footer.svg';
  import { Button, Icon } from 'svelte-materialify';
  import { mdiGithub, mdiLinkedin, mdiTwitter } from '@mdi/js';
</script>

<div class="hero">
  <div class="w-full lg:p-32 p-16 pt-40">
    <span class="hello">Hi, My name is</span>
    <div class="lg:w-2/3 w-full mt-6">
      <span class="name">Salman Mohammed.</span>
    </div>
    <div class="w-full mt-4">
      <span class="work"> I build stuff for the web. </span>
    </div>
    <div class="w-full flex flex-row justify-between lg:mt-12 mt-6 ">
      <a href="#works">
        <div class="view-btn">
          <span class="view-btn-text smooth">VIEW PROJECTS</span>
          <div class="view-btn-border" />
        </div>
      </a>
      <div class="flex flex-row pr-10">
        <div class="my-auto">
          <Button icon>
            <Icon path={mdiGithub} class="text-gray-200" />
          </Button>
        </div>
        <div class="my-auto">
          <Button icon>
            <Icon path={mdiLinkedin} class="text-gray-200" />
          </Button>
        </div>
        <div class="my-auto">
          <Button icon>
            <Icon path={mdiTwitter} class="text-gray-200" />
          </Button>
        </div>
      </div>
    </div>
  </div>
  <div class="w-full absolute bottom-0 flex justify-center">
    <img src={FooterSvg} alt="" />
  </div>
</div>
