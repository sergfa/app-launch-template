<template>
    <section id="features" class="bg-dark py-5 text-light">
        <div class="container">
            <div class="row">
                <div v-for="(item,index) in items" :key="index" class="col-md-6 col-lg-4 d-flex py-5">
                    <i class="fas fa-2x mr-3 align-self-center" :class="'fa-' + item.icon"></i>
                    <div class="feature-body">
                        <h2 class="text-uppercase">{{item.name}}</h2>
                        <p>{{item.desc}}</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
<script>
export default {
    data () {
        return {
            items: [{name:'Inovation', icon:'bomb', desc: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Minus distinctio eveniet commodi ut ad aperiam blanditiis officiis placeat laborum impedit?'},
            {name:'Performance', icon: 'spinner', desc: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Minus distinctio eveniet commodi ut ad aperiam blanditiis officiis placeat laborum impedit?'},
            {name:'Security', icon: 'lock', desc: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Minus distinctio eveniet commodi ut ad aperiam blanditiis officiis placeat laborum impedit?'}]
        }
    }
}
</script>
