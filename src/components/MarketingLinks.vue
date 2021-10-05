<template>
<div class="MarketingLinks">
    <div class="MarketingLinks-cont">
        <ul>
          <li v-for="(link, index) in icone" :key="index">
            <a :href="link.url">
                <img :src="link.img" alt=""> <div>{{link.text}}</div>
            </a>
          </li>
        </ul>
    </div>
</div>
</template>

<script>
export default {
    name: "MarketingLinks",
    data() {
		return {
			icone: [
                {
                    "img": require("../assets/img/buy-comics-digital-comics.png"),
                    "url": "#",
                    "text": "DIGITAL COMICS",
                },
                {
                    "img": require("../assets/img/buy-comics-digital-comics.png"),
                    "url": "#",
                    "text": "DC MERCHANDISE",
                },
                {
                    "img": require("../assets/img/buy-comics-digital-comics.png"),
                    "url": "#",
                    "text": "SUBSCRIPTION",
                },
                {
                    "img": require("../assets/img/buy-comics-digital-comics.png"),
                    "url": "#",
                    "text": "COMIC SHOP LOCATOR",
                },
                {
                    "img": require("../assets/img/buy-comics-digital-comics.png"),
                    "url": "#",
                    "text": "DC POWER VISA",
                }
            ],
		}
	}

}
</script>

<style lang="scss" scoped>

@import "../assets/style/variables";

.MarketingLinks{
    height: 8rem;
    background-color: $mainColor;
    .MarketingLinks-cont{
        height: 100%;
        font-size: 1.375rem;
        color: #fff;
        width: $sizeContainer;
        margin: auto;
        display: flex;
        align-items: center;
        justify-content: center;
        ul{
            list-style: none;
            display: flex;

        }
        a{
            display: flex;
            text-decoration: none;
            padding: .5rem;
            color: #fff;
            font-size: 1.125rem;
            font-weight: 500;
            align-items: center;
        }
        img{
            width: 3.75rem;
            padding-right: .625rem;
        }
        div{
            display: inline-block;
        }
    }
    
}
</style>