<template>
    <div class="main-box">
        
        <div class="obj-list">
            <h2>Наши объекты:</h2>
           <ul>
            <building 
                v-for="obj of objects" :key="obj.id"
                v-bind:obj="obj"                    
            />
           </ul>
        </div>
        <div class="map"> 
            <div id="map" style="width:800px; height:600px"></div>  
        
        </div>
        
    </div>
    
</template>

<script>
import building from '@/views/building'
export default {
    name: 'app',
    data() {
        return {
            objects: [
                {id: 1, title: 'Selezneva, 47', link:'/object'},
                {id: 2, title: 'Vysotskogo, 45/1'}
            ]
        }
    },
    components: {
        building
    },
    /*
    methods: {
        search: function(event) {
            for (obj in objects) {
                if (obj.title == search.value) {
                    alert("OK")
                }
            }
        }
    }*/
}
</script>