<template>
    <div>
        <template v-for="theme in themes">
            {{ theme.name }} 
            <img :src="theme.featured.url" class="w-20"/>
            
        </template>
    </div>
</template>

<script>
import { mapState } from 'vuex'
export default {
    name: 'MokaThemes',
    computed:{
        ...mapState ( ['themes'] )
    }
}
</script>