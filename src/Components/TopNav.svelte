<script>
  import {
    Button,
    List,
    ListItem,
    Menu,
    MaterialApp,
  } from 'svelte-materialify';
  import { scale, slide } from 'svelte/transition';
</script>

<div class="top-nav">
  <div class="flex flex-row justify-center items-center">
    <span class="logo">S</span>
    <span class="nav-name">Salman M.</span>
  </div>
  <div class="flex flex-row">
    <Menu
      right
      transition={slide}
      inOpts={{ duration: 500 }}
      class="menu"
      closeOnClick
    >
      <div class="my-auto" slot="activator">
        <svg
          width="57"
          height="20"
          viewBox="0 0 26 20"
          class="menu-icon m-auto hover:w-10 hover:h-5"
        >
          <path
            fill="transparent"
            stroke-width="1.5"
            stroke="#c4c4c4"
            d="M 2 2.5 L 57 2.5"
          />
          <path
            fill="transparent"
            stroke-width="1.5"
            stroke="#c4c4c4"
            d="M 2 9.423 L 57 9.423"
            opacity="1"
          />
          <path
            fill="transparent"
            stroke-width="1.5"
            stroke="#c4c4c4"
            d="M 2 16.346 L 27 16.346"
          />
        </svg>
      </div>
      <div class="w-60 backdrop-blur-md bg-[#4c4c62]">
        <span class="menu-title">Menu</span>
        <List class="w-full">
          <a href="#works" class="w-full">
            <ListItem class="menu-item">
              <span class="menu-number">01.</span> Work</ListItem
            >
          </a>
          <a href="#specialities" class="w-full">
            <ListItem class="menu-item">
              <span class="menu-number">02.</span> Specialities</ListItem
            >
          </a>
          <a href="#contact" class="w-full">
            <ListItem class="menu-item">
              <span class="menu-number">03.</span> Contact</ListItem
            >
          </a>
          <a href="#resume" class="w-full">
            <ListItem
              class="hover:bg-[#3f3f5b] flex justify-center items-center"
            >
              <Button outlined>Resume</Button>
            </ListItem>
          </a>
        </List>
      </div>
    </Menu>
  </div>
</div>
