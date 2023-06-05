<template>
    <div>
        <section>
            <div class="container">
                <div class="items" v-for="(item, i) in items" :key="i">
                    <div class="img">
                        <img :src="item.img" alt="">
                    </div>
                    <div class="text">
                        <h3>{{ item.name }}</h3>
                        <div class="price" v-html="item.price">
                        </div>
                    </div>
                </div>
            </div>
            <button>SHOP NOW</button>
        </section>
    </div>
</template>

<script>
export default {
    setup() {
        const items = [
            {
                img: 'https://www.pxg.com/dw/image/v2/BFXB_PRD/on/demandware.static/-/Library-Sites-PXGSharedLibrary/default/dw728d6d15/images/site/clubs/drivers/ECOM-1438-Drivers-Category-Page-730x680-Marquee-Drivers.png',
                name: '0311 GEN6 DRIVERS',
                price: '$499<sup>99</sup>'
            },
            {
                img: 'https://www.pxg.com/dw/image/v2/BFXB_PRD/on/demandware.static/-/Library-Sites-PXGSharedLibrary/default/dw436b3f2b/images/site/clubs/drivers/GEN5/GEN5-Drivers-Opt.png',
                name: '0311 GEN5 DRIVERS',
                price: '$289<sup>99</sup>'
            },
            {
                img: 'https://www.pxg.com/dw/image/v2/BFXB_PRD/on/demandware.static/-/Library-Sites-PXGSharedLibrary/default/dwa979a379/images/site/clubs/drivers/ECOM-279-0211-Woods-720%C3%97682-Driver-single.png',
                name: '0211 DRIVERS',
                price: '$199<sup>99</sup>'
            },
            {
                img: 'https://www.pxg.com/dw/image/v2/BFXB_PRD/on/demandware.static/-/Library-Sites-PXGSharedLibrary/default/dw27fd4929/images/site/clubs/fairway-woods/GEN6/GEN6-Fairway-Grouping.png',
                name: '0311 GEN6 FARAWAYS',
                price: '$299<sup>99</sup>'
            },
            {
                img: 'https://www.pxg.com/dw/image/v2/BFXB_PRD/on/demandware.static/-/Library-Sites-PXGSharedLibrary/default/dw08395287/images/site/clubs/fairway-woods/GEN5-Fairways-670x630.png',
                name: '0311 GEN5 FARAWAYS',
                price: '$199<sup>99</sup>'
            },
            {
                img: 'https://www.pxg.com/dw/image/v2/BFXB_PRD/on/demandware.static/-/Library-Sites-PXGSharedLibrary/default/dw6817047c/images/site/clubs/fairway-woods/ECOM-574-0211-Fairways-720%C3%97682-Fairway-single.png',
                name: '0211 FARAWAYS',
                price: '$149<sup>99</sup>'
            }
        ]

        return {
            items
        }
    }
}
</script>

<style scoped>
section {
    background-color: #171717;
    padding: 3rem 1rem;
}

.img {
    width: 50%;
    height: auto;
    margin: auto;
}
.container {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 5rem 1rem;
    max-width: 1000px;
    margin: 3rem auto;
}

.items {
    position: relative;
}

button {
    color: #fff;
    border: 2px solid #fff;
    background-color: transparent;
    font-weight: 700;
    padding: 0.5rem 2rem;
    margin-top: 3rem;
}

h3 {
    color: #fff;
}

.text {
    display: flex;
    flex-direction: column;
    align-items: center;
}

.price {
    color: #fff;
    border: 1px solid #ff003b;
    padding: 0.5rem 1rem;
}

@media only screen and (max-width: 800px) {
    .container {
        grid-template-columns: repeat(2, 1fr);
    }
}
</style>