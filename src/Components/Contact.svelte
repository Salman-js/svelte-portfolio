<script>
  import { Button, Icon } from 'svelte-materialify';
  import { mdiGithub, mdiLinkedin, mdiTwitter } from '@mdi/js';
</script>

<div class="specialities-container">
  <div class="w-full p-20 pb-16">
    <div class="w-4/5 flex lg:flex-row flex-col">
      <div class="my-auto">
        <h2 class="projects-title" id="contact">
          <span class="menu-number">03.</span> Get in touch
        </h2>
      </div>
      <a href="mailto:salmanmoh.eth@gmail.com" class="ml-6 lg:mt-0 mt-4">
        <div
          class="rounded-md p-4 border border-[#e7ab54] flex flex-row justify-center"
        >
          <span class="my-auto">
            <img
              src="https://em-content.zobj.net/source/microsoft-teams/337/waving-hand_1f44b.png"
              alt=""
              class="w-8"
            />
          </span>
          <span class="text-2xl text-[#e7ab54] font-bold ml-3 my-auto">
            Say Hello
          </span>
        </div>
      </a>
    </div>
  </div>
  <div class="w-full flex flex-col items-center justify-center px-10 pt-4 pb-6">
    <p class="credit">Designed & built by Salman Mohammed</p>
    <div class="w-full flex flex-row justify-center mb-5 mt-3">
      <div class="my-auto">
        <Button icon>
          <Icon
            path={mdiGithub}
            class="text-white opacity-40 hover:opacity-100"
          />
        </Button>
      </div>
      <div class="my-auto">
        <Button icon>
          <Icon
            path={mdiLinkedin}
            class="text-white opacity-40 hover:opacity-100"
          />
        </Button>
      </div>
      <div class="my-auto">
        <Button icon>
          <Icon
            path={mdiTwitter}
            class="text-white opacity-40 hover:opacity-100"
          />
        </Button>
      </div>
    </div>
  </div>
</div>
