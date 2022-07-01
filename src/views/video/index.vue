<template>
    <div class="video-container">
        <!-- <button @click="kai">组件</button>
        <button @click="kai1">函数</button>
        <van-image-preview v-model="show" :images="images" @change="onChange">

        </van-image-preview> -->
        <van-cell is-link @click="showPopup">展示弹出层</van-cell>
        <van-popup v-model="show" position="bottom" closeable close-icon-position="top-right" close-icon="close"
            :style="{ width: '100%', height: '70%' }" round>内容</van-popup>

    </div>
</template>

		<script>

// import { ImagePreview } from "vant";
// export default {
//     data() {
//         return {
//             show: false,

//             images: [
//                 'https://img01.yzcdn.cn/vant/apple-1.jpg',
//                 'https://img01.yzcdn.cn/vant/apple-2.jpg',
//             ],
//         };

//     },
//     methods: {

//         kai() {
//             this.show = true;
//         },
//         kai1() {
//             ImagePreview([
//                 'https://img01.yzcdn.cn/vant/apple-1.jpg',
//                 'https://img01.yzcdn.cn/vant/apple-2.jpg',

//             ]);
//         }
//     },
// };

export default {
    data() {
        return {
            show: false,
        };
    },

    methods: {
        showPopup() {
            this.show = true;
        },
    },
};
</script>

<style scoped>
</style>