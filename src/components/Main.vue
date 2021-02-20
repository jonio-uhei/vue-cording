<template>
    <div class="container">
        <section id="about">
            <div class="section">
                <h2 class="section__title">About</h2><!--/.section__title-->
                    <div class="flex-box1">
                    <img class="section__image" src="../assets/about.jpg" alt=""><!--/.section__image-->
                    <div>
                        <p class="section__name">KAKERU MIYAICHI</p><!--/.section__name-->
                        <ul 
                            class="section__lists"
                            v-for="item in items"
                            :key="item.id"
                        >
                            <li class="section__content" v-text="item.content"></li>
                        </ul><!--/.section__lists-->
                    </div>
                </div><!--/.flex-box-->
            </div><!--/.section-->
        </section><!--/#about-->
        <section id="bycycle">
            <div class="section">
                <h2 class="section__title">Bycycle</h2><!--/.section__title-->
                <div class="flex-box2">
                    <ul 
                        class="section__lists"
                        v-for="list in lists"
                        :key="list.id"
                    >
                        <img class="section__image1":src="list.image">
                        <li class="section__midashi">{{list.title}}</li>
                        <li class="section__content">{{list.content}}</li>
                    </ul><!--/.section__lists-->
                </div><!--/.flex-box2-->
            </div><!--/.section-->
        </section><!--/#about-->
    </div><!--/.container-->
</template>

<script> 
    export default{
        data:function(){
            return{
                items:[
                    {
                        content:'テキストテキストテキストテキストテキストテキスト'
                    },
                    {
                        content:'テキストテキストテキストテキストテキストテキスト'
                    },
                    {
                        id:3,
                        content:'テキストテキストテキストテキストテキストテキスト'
                    },
                ],
                lists:[
                    {
                        image:require('@/assets/bicycle1.jpg'),
                        title:'タイトル',
                        content:'テキストテキストテキスト'
                    },
                    {
                        image:require('@/assets/bicycle2.jpg'),
                        title:'タイトル',
                        content:'テキストテキストテキスト'
                    },
                    {
                        image:require('@/assets/bicycle3.jpg'),
                        title:'タイトル',
                        content:'テキストテキストテキスト'
                    },
                ],
            }
        }
    }
</script>

<style>
    
</style>