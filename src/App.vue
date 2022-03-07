<template>
  <div id="app">

    <!-- Passo props per link header -->
    <myHeader :navLinks="navLinks"/>

    <myMain/>

    <!-- Passo props per footer social e links -->
    <myFooter :footerSocial="footerSocial" :footerLinks="footerLinks"/>
  </div>
</template>

<script>
import myHeader from './components/myHeader.vue'
import myMain from './components/myMain.vue'
import myFooter from './components/myFooter.vue'


export default {
  name: 'App',
  components: {
    myHeader,
    myMain,
    myFooter,
  },

  data(){

    return {

      // oggetti header navbar
      navLinks : [

        {

          name: 'Home',

          url: '#',

        },

        {

          name: 'Pages',

          url: '#',

        },

        {

          name: 'Courses',

          url: '#',

        },

        {

          name: 'Features',

          url: '#',

        },

        {

          name: 'Blog',

          url: '#',

        },

        {

          name: 'Shop',

          url: '#',

        },

      ],

      // oggetti liste footer 
      footerSocial: [

        {

          class: 'fa-facebook',

          url: '#'

        },

        {

          class: 'fa-twitter',

          url: '#'

        },

        {

          class: 'fa-instagram',

          url: '#'

        },

        {

          class: 'fa-linkedin',

          url: '#'

        },
      ],

      //Link Footer
      footerLinks: [

        {

          name: '382 NE 191st St # 87394 Miami, FL 33179-3899',

          url: '#',

          address: true,

        },

        {

          name: '+1(305)547-9909(9am - 5pm EST, Monday - Friday)',

          url: '#',

          address: true,

        },

        {

          name: 'support@MaxCoach.com',

          url: '#',

          address: true,

        },

        {

          name: 'Start Here',

          url: '#',

          explore : true

        },

        {

          name: 'Blog',

          url: '#',

          explore : true

        },

        {

          name: 'About Us',

          url: '#',

          explore : true

        },

        {

          name: 'Success Story',

          url: '#',

          explore : true

        },

        {

          name: 'Courses',

          url: '#',

          explore : true

        },

        {

          name: 'Contact Us',

          url: '#',

          explore : true

        },

        {

          name: 'Membership',

          url: '#',

          information : true

        },

        {

          name: 'Purchase guide',

          url: '#',

          information : true

        },

        {

          name: 'Privacy Policy',

          url: '#',

          information : true

        },

        {

          name: 'Terms of services',

          url: '#',

          information : true

        },

      ],

    }

  }

}
</script>

<style lang="scss">
#app{
  font-family: 'Questrial';
}
</style>
