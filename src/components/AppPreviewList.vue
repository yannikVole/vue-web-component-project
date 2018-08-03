<template>
    <div id="preview-container">
        <app-preview-list-item v-for="previewItem in previewItems" :preview-item="previewItem" :key="previewItem.id"/>
    </div>
</template>

<script>
    import AppPreviewListItem from './AppPreviewListItem';

    export default {
        name: "AppPreviewList",
        components:{
            AppPreviewListItem
        },
        data(){//all vue components have to return da data object!
            return{
                //all 3 preview items defined, this might also be data from an API
                previewItems:[
                    {
                        id:'04c09292-d4c2-4c8b-927e-98cf9501a3c1',
                        imgUrl:"https://images.pexels.com/photos/315788/pexels-photo-315788.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260",
                        readMoreLink:'#',
                        textContent:'Bacon ipsum dolor amet strip steak doner ribeye venison t-bone ball tip. Meatloaf tail capicola andouille cow. Tri-tip turducken beef t-bone strip steak doner boudin bresaola frankfurter pork belly ball tip ribeye meatball swine. Pork belly turducken pork chop shankle filet mignon, cow tail t-bone pork loin frankfurter flank. Jerky biltong hamburger pork loin. Ball tip short ribs doner cow prosciutto shankle bresaola t-bone short loin boudin pig. Beef ribs alcatra picanha meatball pork chop brisket.',
                        heading:'Preview Heading 1'
                    },
                    {
                        id:'fae6bb05-c302-4262-8129-98459dbddcb2',
                        imgUrl:"https://images.pexels.com/photos/1248238/pexels-photo-1248238.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260",
                        readMoreLink:'#',
                        textContent:'Alcatra pork loin pastrami meatloaf. Doner t-bone biltong, drumstick ham hock prosciutto ham landjaeger kielbasa jerky pork pig pastrami andouille. Turducken short loin pastrami capicola, pig chicken drumstick flank pork loin biltong leberkas corned beef. Strip steak flank meatloaf bacon, andouille brisket cow doner tenderloin leberkas jowl pork chop t-bone biltong beef. Pork belly short loin alcatra tenderloin jerky pork sausage andouille meatloaf pork chop jowl pancetta pork loin tri-tip picanha.',
                        heading:'Preview Heading 2'
                    },
                    {
                        id:'059ae9c1-f478-4915-ada6-ab7e7f9885da',
                        imgUrl:"https://images.pexels.com/photos/1231023/pexels-photo-1231023.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260",
                        readMoreLink:'#',
                        textContent:'Doner drumstick filet mignon tenderloin. Pig rump landjaeger, shank sirloin turkey short ribs pastrami beef ribs ham hock pork belly. Brisket chicken chuck hamburger doner jerky buffalo pastrami pork belly ribeye strip steak ham hock beef ribs cow. Drumstick cow chicken venison t-bone andouille, filet mignon bresaola tenderloin frankfurter pork belly jowl corned beef.',
                        heading:'Preview Heading 3'
                    }
                ]
            }
        }
    }
</script>

<style scoped>
    #preview-container{
        display:flex;
        flex-direction:row;
        flex-wrap: wrap;
    }
</style>