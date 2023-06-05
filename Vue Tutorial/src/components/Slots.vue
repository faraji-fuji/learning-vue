<script>
import ChildComp3 from './ChildComp3.vue';

export default {
    components: {
        ChildComp3
    },

    data(){
        return{
            msg: 'From parent'
        }
    }
}
</script>

<template>
    <ChildComp3>
        Message: {{msg}}
    </ChildComp3>
</template>