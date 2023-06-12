<template>
    <!-- top navigation -->
    <div>
        <Navigation/><!-- using the imported element -->
    </div>
    <!-- center section -->
    <!-- bottom section -->
    
</template>

<script>
//1.import components
//2.build option object
//3.
//import is outside export default
//import components to Home page i.e navigation.vue
import Navigation from '../navigation/Navigation.vue'

export default{
components:{//explicitly say which are your imported elements , otherwise it won't work for options api
Navigation//
}

}
</script>

<style scoped>


</style>