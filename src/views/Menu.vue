<template>
    <sidebar-menu :menu="menu" />
</template>

<script>

    export default {
        // width:{type:String,default:"350px"}
        data() {
            return {

                menu: [
                    {
                        header: true,
                        title: '',
                        // component: componentName
                        // visibleOnCollapse: true
                        // class: '',
                        attributes: {},


                    },
                    {
                        href: '/',
                        title: 'Sub 2',
                        icon: 'fa fa-user',

                        // custom icon
                        icon: {
                            element: 'span',
                            class: 'fa fa-user',
                            attributes: {}
                        }
                    },
                    {
                        href: '/',
                        title: 'Sub 3',
                        icon: 'fa fa-user',

                        // custom icon
                        icon: {
                            element: 'span',
                            class: 'fa fa-user',
                            attributes: {}
                        }

                        // disabled: true
                        // class: ''
                        // attributes: {}
                        // alias: '/path'
                        /*
                        badge: {
                            text: 'new',
                            class: 'default-badge'
                            // attributes: {}
                            // element: 'span'
                        }
                        */
                    },
                    {
                        title: 'SUB 4',
                        icon: 'fa fa-chart-area',
                        child: [
                            {
                                href: '/charts/sublink',
                                title: 'Sub Link',
                            }
                        ]
                    }
                ],
            }
        }
    }
</script>

<style scoped lang="scss">
    @import url('https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.8.2/css/all.min.css');
    @import url('https://fonts.googleapis.com/css?family=Lato:400,700&display=swap');
    .v-sidebar-menu{
        background: linear-gradient(135deg,#3b5daa,rgba(130,218,245,.5));

    }
    .v-sidebar-menu .vsm-title{
        text-align: left;
    }

</style>