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
            <div id="map" style="width:1200px; height:800px"></div>  
        
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
                {id: 1, title: 'Selezneva, 47'},
                {id: 2, title: 'Vysotskogo, 45/1'}
            ]
        }
    },
    components: {
        building
    }
}
</script>