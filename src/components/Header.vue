<template>
  <header>
    <div class="header-cont">
      <div class="logo">
        <img src="@/assets/img/dc-logo.png" alt="Logo-DC">
      </div>
      <nav>
        <ul>
          <li v-for="(link, index) in menu" :key="index">
            <a :href="link.url" :class="{ active : link.current }">{{link.text}}</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
	name: "Header",
	data() {
		return {
			menu: [
                {
                    text: "CHARACTERS",
                    url: "#",
                    current: false,
                },
                {
                    text: "COMICS",
                    url: "#",
                    current: true,
                },
                {
                    text: "MOVIES",
                    url: "#",
                    current: false,
                },
                {
                    text: "TV",
                    url: "#",
                    current: false,
                },
                {
                    text: "GAMES",
                    url: "#",
                    current: false,
                },
                {
                    text: "COLLECTIBLES",
                    url: "#",
                    current: false,
                },
                {
                    text: "VIDEOS",
                    url: "#",
                    current: false,
                },
                {
                    text: "FANS",
                    url: "#",
                    current: false,
                },
                {
                    text: "NEWS",
                    url: "#",
                    current: false,
                },
                {
                    text: "SHOP",
                    url: "#",
                    current: false,
                },
            ],
		}
	}
}
</script>

<style lang="scss" scoped>

@import "../assets/style/variables";

header{
  background-color: #ffffff;
  
  div.header-cont{
    width: $sizeContainer;
    margin: auto;
    display: flex;
    height: 5rem;
    align-items: center;
    .logo img{
      height: 4.375rem;
    }
    nav{
      width: 100%;
      ul{
        display: flex;
        list-style: none;
        justify-content: flex-end;
      }
      a{
        display: inline-block;
        text-decoration: none;
        padding: .5rem;
        color: #464646;
        font-size: 1.125rem;
        font-weight: 500;
        &.active {
          color:$mainColor;
          box-shadow: 0 0 0 .125rem $mainColor;
        }
      }
    }


  }
}
</style>
