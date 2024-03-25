<template>
    <div>
        <v-card class="ma-0 pa-0" elevation="0" height="400px">
            <v-row>
                <v-col class="">
                    <div class="block-33 display--inline-top  gallery-h--tb">
                        <div class="my-2 fill-dimensions cover-img gallery-image"
                            style="background-image:url('http://images.all-free-download.com/images/graphiclarge/beautiful_scenery_04_hd_images_166331.jpg')">
                        </div>
                        <div class="my-2 fill-dimensions cover-img gallery-image"
                            style="background-image:url('http://images.all-free-download.com/images/graphiclarge/beautiful_scenery_04_hd_images_166331.jpg')">
                        </div>
                        <div class="my-2 fill-dimensions cover-img gallery-image"
                            style="background-image:url('https://i.pinimg.com/564x/6e/4b/b1/6e4bb10e44393da31905c3ac56663099.jpg')">
                        </div>
                        <div class="my-2 fill-dimensions cover-img gallery-image"
                            style="background-image:url('http://images.all-free-download.com/images/graphiclarge/beautiful_scenery_04_hd_images_166331.jpg')">
                        </div>
                    </div>
                </v-col>
                <v-col class="">
                    <div class="block-33 display--inline-top  ">
                        <div class="my-2 fill-dimensions cover-img gallery-image"
                            style="background-image:url('https://i.pinimg.com/564x/eb/1e/2e/eb1e2eeefac3fd538486707512c77bb6.jpg')">
                        </div>
                        <div class="my-2 fill-dimensions cover-img gallery-image"
                            style="background-image:url('http://images.all-free-download.com/images/graphiclarge/beautiful_scenery_04_hd_images_166331.jpg')">
                        </div>
                        <div class="my-2 fill-dimensions cover-img gallery-image"
                            style="background-image:url('https://i.pinimg.com/474x/16/fa/a6/16faa6df4c82bf536af0817159d83788.jpg')">
                        </div>
                    </div>
                </v-col>
            </v-row>
        </v-card>
        <!-- </div> -->
    </div>
</template>
<style scoped>
.display--inline-top{
    height: 400px;
    overflow: hidden;
}
.fill-dimensions{
    width: 200px;
    height: 200px;
    border-radius: 10px;
}
.cover-img {
    background-size: cover;
    background-position: center center;
    background-repeat: no-repeat;
}

.gallery-image {
    padding-bottom: 2.35em;
    animation: marqueeTop 2s linear infinite;
}

.gallery-h--tb {
    .gallery-image {
        animation: marqueeBottom 2s linear infinite;
    }
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
    0% {
        -webkit-transform: translate3d(0, 0, 0);
        transform: translate3d(0, 0, 0)
    }
}

@keyframes marqueeBottom {
    0% {
        -webkit-transform: translate3d(0, -100%, 0);
        transform: translate3d(0, -100%, 0)
    }

    100% {
        -webkit-transform: translate3d(-100%, 0, -100%);
        transform: translate3d(0, 0, 0)
    }
}
</style>