<template>
    <div>
        <v-card class="ma-0 pa-0" elevation="0" height="400px">
    <v-row>
        <v-col>
        <!-- <div class="gallery"> -->
           
            <div class="block-33 display--inline-top">
                <div class="gutter relative">
                    <div class="gallery-h gallery-h--tb">
                        <div class="gallery-image relative">
                            <div class="gallery-image__img relative">
                                <div class="fill-dimensions cover-img"
                                    style="background-image:url('http://images.all-free-download.com/images/graphiclarge/beautiful_scenery_04_hd_images_166331.jpg')">
                                </div>
                            </div>
                        </div>
                        <div class="gallery-image">
                            <div class="gallery-image__img relative">
                                <div class="fill-dimensions cover-img"
                                    style="background-image:url('http://images.all-free-download.com/images/graphiclarge/beautiful_scenery_04_hd_images_166331.jpg')">
                                </div>
                            </div>
                        </div>
                        <div class="gallery-image">
                            <div class="gallery-image__img relative">
                                <div class="fill-dimensions cover-img"
                                    style="background-image:url('http://images.all-free-download.com/images/graphiclarge/beautiful_scenery_04_hd_images_166331.jpg')">
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            </v-col>
            <v-col>
            <div class="block-33 display--inline-top">
                <div class="gutter relative">
                    <div class="gallery-h">
                        <div class="gallery-image relative">
                            <div class="gallery-image__img relative">
                                <div class="fill-dimensions cover-img"
                                    style="background-image:url('http://images.all-free-download.com/images/graphiclarge/beautiful_scenery_04_hd_images_166331.jpg')">
                                </div>
                            </div>
                        </div>
                        <div class="gallery-image">
                            <div class="gallery-image__img relative">
                                <div class="fill-dimensions cover-img"
                                    style="background-image:url('http://images.all-free-download.com/images/graphiclarge/beautiful_scenery_04_hd_images_166331.jpg')">
                                </div>
                            </div>
                        </div>
                        <div class="gallery-image">
                            <div class="gallery-image__img relative">
                                <div class="fill-dimensions cover-img"
                                    style="background-image:url('http://images.all-free-download.com/images/graphiclarge/beautiful_scenery_04_hd_images_166331.jpg')">
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </v-col>
        </v-row>
        </v-card>
        <!-- </div> -->
    </div>
</template>
<style scoped>
.gallery {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    /* height: 100%; */
}
.block-33 {
    width: 250px;
}
.display--inline-top {
    display: inline-block;
    vertical-align: top;
}

.fill-dimensions {
    width: 100%;
    height: 100%;
    position: absolute;
    top: 0;
    left: 0;
}

.cover-img {
    background-size: cover;
    background-position: center center;
    background-repeat: no-repeat;
}
.gallery-image {
    padding-bottom: 2.35em;
    animation: marqueeTop 8s linear infinite;
}
.gallery-h--tb {
    .gallery-image {
        animation: marqueeBottom 8s linear infinite;
    }
}
.gallery-image__img {
    padding-top: 50vh;
    width: 100px;
    margin: 10px auto;

}
.gallery-h {
    overflow: hidden;
}

@keyframes marqueeTop {
    0% {
        -webkit-transform: translate3d(0, 0, 0);
        transform: translate3d(0, 0, 0)
    }

    100% {
        -webkit-transform: translate3d(0, -100%, 0);
        transform: translate3d(0, -100%, 0)
    }
}

@keyframes marqueeBottom {
    0% {
        -webkit-transform: translate3d(0, -100%, 0);
        transform: translate3d(0, -100%, 0)
    }

    100% {
        -webkit-transform: translate3d(0, 0, 0);
        transform: translate3d(0, 0, 0)
    }
}
</style>