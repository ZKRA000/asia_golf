<template>
    <div>
        <div class="container">
            <h2>A FITTING EXPERIENCE LIKE NO OTHER.</h2>
            <swiper-container navigation="true" space-between="20" slides-per-view="1" :breakpoints="{
                600: {
                slidesPerView: 2,
                },
                900: {
                slidesPerView: 4,
                },
            }">
                <swiper-slide v-for="(item, index) in items" :key="index">
                    <div class="item">
                        <div class="img">
                            <img :src="item.img" alt="">
                        </div>
                        <div class="text">
                            <h3>{{ item.name }}</h3>
                            <p>{{ item.location }}</p>
                        </div>
                        <button>
                            Learn More
                        </button>
                    </div>
                </swiper-slide>
            </swiper-container>
        </div>
    </div>
</template>

<script>
import { register } from 'swiper/element/bundle'
register()

export default {
    setup() {
        const items = [
            {
                img: 'https://www.pxg.com/dw/image/v2/BFXB_PRD/on/demandware.static/-/Library-Sites-PXGSharedLibrary/default/dw9cf0089d/images/site/locations/PXGM-6397-PXG-Denver-Store-Location-Tile-Image-768-384.jpeg',
                name: 'DENVER',
                location: 'Colorado'
            },
            {
                img: 'https://www.pxg.com/dw/image/v2/BFXB_PRD/on/demandware.static/-/Library-Sites-PXGSharedLibrary/default/dwc4658c67/images/site/locations/Locations-Thumbnail-Scottsdale-768x384.jpeg',
                name: 'BOSTON',
                location: 'Massachussets'
            },
            {
                img: 'https://www.pxg.com/dw/image/v2/BFXB_PRD/on/demandware.static/-/Library-Sites-PXGSharedLibrary/default/dwf682da1e/images/site/locations/PXG-Store-Location-home-detroit.jpeg',
                name: 'DETROIR',
                location: 'Michigan'
            },
            {
                img: 'https://www.pxg.com/dw/image/v2/BFXB_PRD/on/demandware.static/-/Library-Sites-PXGSharedLibrary/default/dwc4658c67/images/site/locations/Locations-Thumbnail-Scottsdale-768x384.jpeg',
                name: 'SCOTTSDALE',
                location: 'Arizona'
            },
            {
                img: 'https://www.pxg.com/dw/image/v2/BFXB_PRD/on/demandware.static/-/Library-Sites-PXGSharedLibrary/default/dw9cf0089d/images/site/locations/PXGM-6397-PXG-Denver-Store-Location-Tile-Image-768-384.jpeg',
                name: 'DENVER',
                location: 'Colorado'
            }
        ]

        return {
            items
        }
    }
}
</script>

<style scoped>

.item {
    padding: 1rem 1rem;
}
.container {
    background-color: #000;
    color: #fff;
    text-align: center;
    padding: 1rem;
}

button {
    border: 2px solid #fff;
    font-weight: 700;
    padding: 0.5rem 1rem;
    background-color: transparent;
    color: #fff;
}
</style>