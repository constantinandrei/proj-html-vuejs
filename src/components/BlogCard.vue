<template>
    <div class="col">
        <div class="my-card position-relative">
            <div class="position-absolute">
                <div class="green">07</div>
                <div class="pink">MAY '19</div>
                <div class="tr-left"></div>
                <div class="tr-right"></div>
            </div>
            <img :src="`img/${imgSrc}`" alt="">
            <div class="post-title py-3">
                {{ articleTitle }}
            </div>
            <div class="post-author">
                By {{articleAuthor}}
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'BlogCard',
        props: {
            imgSrc: String,
            articleTitle: String,
            articleAuthor: {
                type: String,
                default: 'Emily Fields'
            }
        }
    }
</script>

<style lang="scss" scoped>
    img {
        width: 100%
    }

    .position-absolute {
        top: -20px;
        left: 20px;
        height: 300px;
        max-width: 60px;
        overflow: hidden;
        .green {
            background-color: rgb(192, 225, 208);
            width: 55px;
            height: 40px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: bold;
            font-style: italic;
            font-family: 'Comic Sans MS';
            font-size: 1.3rem;
        }

        .pink {
            position: relative;
            background-color: rgb(243, 208, 199);
            width: 55px;
            height: 30px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: .7rem;
            z-index: 3;
            font-weight: bold;
        }

        .tr-left {
            overflow: hidden;
            position: absolute;
            left: 0;
            width: 75%;
            height: 20px;
            background-color: rgb(243, 208, 199);
            transform: rotate(-30deg) translateY(-15px);
        }

        .tr-right {
            overflow: hidden;
            position: absolute;
            right: 0;
            width: 75%;
            height: 20px;
            background-color: rgb(243, 208, 199);
            transform: rotate(30deg) translateY(-15px);
        }
    }

    .post-author {
        font-style: italic;
    }

    .post-title {
        font-size: 1.5rem;
    }
</style>