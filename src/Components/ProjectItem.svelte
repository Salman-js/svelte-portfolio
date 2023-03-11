<script>
  import { Button, Icon } from 'svelte-materialify';
  import { mdiGithub, mdiOpenInNew } from '@mdi/js';
  import Design1 from '../assets/design1.svg';
  const stacks = [
    { title: 'Title', image: 'https://reactjs.org/favicon.ico' },
    {
      title: 'Title',
      image: 'https://nextjs.org/static/favicon/favicon-32x32.png',
    },
    {
      title: 'Title',
      image:
        'https://pbs.twimg.com/profile_images/1452637606559326217/GFz_P-5e_400x400.png',
    },
    {
      title: 'Title',
      image: 'https://labs.mysql.com/common/themes/sakila/favicon.ico',
    },
  ];
</script>

<div class="project-item">
  <div class="image-container">
    <img
      src="https://img.freepik.com/free-photo/low-angle-shot-tall-city-building-with-blue-sky-background-new-york_181624-20345.jpg?w=2000"
      alt=""
      class="w-full"
    />
  </div>
  <div class="detail-container">
    <div class="w-full">
      <p class="project-title">Project Title</p>
      <div class="stacks-container">
        {#each stacks as stack, index (index)}
          <img src={stack.image} alt="" class="mx-1 w-6" />
        {/each}
      </div>
      <div class="description-container">
        <p class="project-description">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequuntur
          a, veritatis quis voluptas tenetur, similique rem non, nisi
          necessitatibus esse libero delectus ex blanditiis. Laborum.
        </p>
      </div>
    </div>
    <div class="flex flex-row w-full justify-between items-start">
      <div class="my-auto flex flex-row">
        <div class="my-auto ml-3">
          <Button icon>
            <Icon
              path={mdiGithub}
              class="text-white opacity-40 hover:opacity-100"
              st
            />
          </Button>
        </div>
        <div class="my-auto">
          <Button icon>
            <Icon
              path={mdiOpenInNew}
              class="text-white opacity-40 hover:opacity-100"
            />
          </Button>
        </div>
      </div>
      <img src={Design1} alt="" class="lg:w-20 w-10" />
    </div>
  </div>
</div>
