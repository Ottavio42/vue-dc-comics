<template>
<div class="MarketingLinks">
    <div class="MarketingLinks-cont">
        <ul>
          <li v-for="(link, index) in icone" :key="index">
            <a :href="link.url">
                <img :src="link.img" alt=""> <span>{{link.text}}</span>
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
                    "img": "../assets/img/buy-comics-digital-comics.png",
                    "url": "#",
                    "text": "DIGITAL COMICS",
                },
                {
                    img: "../assets/img/buy-comics-digital-comics.png",
                    url: "#",
                    text: "DC MERCHANDISE",
                },
                {
                    img: "../assets/img/buy-comics-digital-comics.png",
                    url: "#",
                    text: "SUBSCRIPTION",
                },
                {
                    img: "../assets/img/buy-comics-digital-comics.png",
                    url: "#",
                    text: "COMIC SHOP LOCATOR",
                },
                {
                    img: "./assets/img/buy-comics-digital-comics.png",
                    url: "#",
                    text: "DC POWER VISA",
                }
            ],
		}
	}

}
</script>

<style lang="scss" scoped>

@import "../assets/style/variables";

.MarketingLinks{
    height: 5rem;
    background-color: $mainColor;
    .MarketingLinks-cont{
        font-size: 1.375rem;
        color: #fff;
        width: $sizeContainer;
        margin: auto;
        display: flex;
        align-items: center;
        ul{
            list-style: none;
            display: flex;

        }
        a{
            display: inline-block;
            text-decoration: none;
            padding: .5rem;
            color: #fff;
            font-size: 1.125rem;
            font-weight: 500;
        }
        img{
            width: 100%;
            height: 50px;
        }
    }
}
</style>