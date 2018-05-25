<template>
    <section id="team" class="bg-primary py-5">
        <div class="container">
            <div class="row mb-5">
                <div class="col text-center">
                    <h1 class="text-uppercase font-weight-bold">team</h1>
                </div>
            </div>
            <div class="row">
                <div v-for="(item, index) in items" :key="index" class="col-sm-6 col-lg-3 mb-5 mt-5">
                    <div class="card text-center">
                        <div class="card-body">
                            <img :src="item.image" alt="member" class="img-fluid rounded-circle mb-2 team-member" style="width:175px">
                            <h2 class="text-capitalize" v-once>{{item.name}}</h2>
                            <h6 class="text-capitalize" v-once>{{item.job}}</h6>
                            <p class="text-left">{{item.desc}}</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
<script>
import imageTeam1 from '../assets/team1.jpg'
export default {
    data () {
        return {
            items: [{image: imageTeam1, name: 'Code Monkey', job: 'developer', desc:' Lorem ipsum dolor sit amet consectetur adipisicing elit. Corporis, sequi!'},
            {image: imageTeam1, name: 'Artist Monkey', job: 'desiner', desc:' Lorem ipsum dolor sit amet consectetur adipisicing elit. Corporis, sequi!'},
            {image: imageTeam1, name: 'Big Monkey', job: 'manager', desc:' Lorem ipsum dolor sit amet consectetur adipisicing elit. Corporis, sequi!'},
            {image: imageTeam1, name: 'IT Monkey', job: 'devops', desc:' Lorem ipsum dolor sit amet consectetur adipisicing elit. Corporis, sequi!'}
            ]
        }
    }
}
</script>
<style>
.team-member {
    margin-top: -100px;
}
.card:hover {
    background-color: darkgray;
    color: #F7F6F4;
}
</style>
