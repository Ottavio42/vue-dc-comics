<template>
<div class="MarketingLinks">
    <div class="MarketingLinks-cont">
        <ul>
          <li v-for="(link, index) in icone" :key="index">
            <a :href="link.url">
                {{link.img}} <span>{{link.text}}</span>
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
                    img: "<img src='@/assets/img/buy-comics-digital-comics.png' alt='icona-market'>",
                    url: "#",
                    text: "DIGITAL COMICS",
                },
                {
                    img: '<img src="@/assets/img/buy-comics-digital-comics.png" alt="icona-market">',
                    url: "#",
                    text: "DC MERCHANDISE",
                },
                {
                    img: '<img src="@/assets/img/buy-comics-digital-comics.png" alt="icona-market">',
                    url: "#",
                    text: "SUBSCRIPTION",
                },
                {
                    img: '<img src="@/assets/img/buy-comics-digital-comics.png" alt="icona-market">',
                    url: "#",
                    text: "COMIC SHOP LOCATOR",
                },
                {
                    img: '<img src="@/assets/img/buy-comics-digital-comics.png" alt="icona-market">',
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
    }
}
</style>