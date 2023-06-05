<template>
    <div>
        <section>
            <div class="container">
                <h2>FEATURED</h2>
                <div :class="['featured-item', index % 2 != 0 ? 'featured-reverse' : '']" v-for="(item, index) in items" :key="index">
                    <div class="featured-img">
                        <img :src="item.img" alt="">
                    </div>
                    <div class="featured-text">
                        <h4 v-if="item.subTitle != null">{{ item.subTitle }}</h4>
                        <h2>{{ item.title }}</h2>
                        <p>{{ item.description }}</p>
                    </div>
                </div>
            </div>
        </section>
    </div>
</template>

<script>
export default {
    setup() {
        const items = [
            {
                img: "https://www.pxg.com/dw/image/v2/BFXB_PRD/on/demandware.static/-/Library-Sites-PXGSharedLibrary/default/dw25bf23c4/images/site/apparel/one-half/PXGM-8910-CREATIVE-ASSETS-Spring-23-Apparel-Launch-Drop-21024x600-Just-Dropped.jpg",
                title: 'Spring \'23',
                subTitle: 'NEW STYLES ADDED',
                description: 'Grab our latest Spring ‘23 pieces, made with high-performance fabrics that deliver style and comfort on and off the course.'
            },
            {
                img: "https://www.pxg.com/dw/image/v2/BFXB_PRD/on/demandware.static/-/Library-Sites-PXGSharedLibrary/default/dwdec68e34/images/site/landing-pages/lucky7/PXGM-8869-Lucky-7-Homepage-v4-Desktop-1024x600.jpg",
                title: 'Pick 7.',
                subTitle: null,
                description: 'Choose seven unique GEN6 Irons, GEN5 Irons, or Sugar Daddy II Wedges for a killer price. This incredible deal puts some kick in your game without kicking you where it hurts - your wallet. '
            }
        ]


        return {
            items
        }
    }
}
</script>

<style scoped>
h2 {
    margin-top: 0;
    color: #fff;
}

section {
    background-color: #171717;
}

.container {
    max-width: 1000px;
    padding: 3rem 1rem;
    margin: auto;
}

.featured-item {
    width: 100%;
    display: block;
    background-color: #121212;
    margin: 2rem 0;
    box-shadow: 1px 1px 3px #171717;
}

.featured-text {
    color: #fff;
    text-align: left;
    padding: 2rem;
    letter-spacing: 0.1rem;
    line-height: 1.5;
}

@media only screen and (min-width: 800px) {
    .featured-item {
        display: grid;
        grid-template-columns: 60% auto;
        align-items: center;
    }

    .featured-reverse {
        grid-template-columns: auto 60%;
    }

    .featured-reverse > .featured-text {
        grid-column: 1/2;
        grid-row: 1;
    }

    .featured-reverse > .featured-img {
        grid-column: 2/3;
        grid-row: 1;
    }
}
</style>