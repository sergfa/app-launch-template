<template>
    <nav class="navbar navbar-expand-sm navbar-dark bg-dark p-3 fixed-top">
        <a href="#" class="navbar-brand text-uppercase">Food Compas</a>
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarBrand">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div id="navbarBrand" class="collapse navbar-collapse justify-content-end">
            <ul class="navbar-nav">
                <li  v-for="(item, index) in items" :key="index" class="nav-item" ><a :href="item.id" class="nav-link text-uppercase text-light">{{item.title}}</a></li>
            </ul>
        </div>
    </nav>
</template>
<script>
export default {
    data () {
        return {
            items: [{id: '#banner', title: 'Home' },
                    {id: '#features', title: 'Features' },
                    {id: '#team', title: 'Team' },
                    {id: '#filler', title: 'Download' },
                    {id: '#about', title: 'About' }
                    ]
        }
    }
}
</script>