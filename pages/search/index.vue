<template>
    <div>
        <div class="top-space">

        </div>
        <b-container>
            <div class="article-content bg-white">
                <b-row>
                    <b-col lg="8" class="blog-box article-content-wrapper">
                        <div class="article-title">
                            <h2 class="inner-main-title title-color">Search Results for: {{searchFor}}</h2>
                            <div class="divide"></div>
                        </div>

                        <article class="blog-post">
                            <h2 class="blog-post__title">This ten-minute phone call could save you hundreds</h2>
                            <div class="blog-post__date">
                                <i class="icon-fa text-success text-sm"><fa :icon="fas.faCalendarAlt"/></i>
                                <span class="main-blog-post-date">Friday, October 25, 2019</span>
                            </div>
                            <img class="img img-fluid mb-5" src="~/assets/img/adult-cutting-daylight-facial-expression.jpg" alt="blog post image">
                            <p class="main-blog-excerpt mb-4">Rude call centre staff. Irritatingly chipper elevator music. You’ve been put on hold three times in the past half hour,......</p>
                            <div class="text-right">
                                <a href="" class="btn btn-default btn-r btn-success btn-w-shadow">Read More <fa :icon="fas.faArrowRight"/></a>
                            </div>
                        </article>

                          <div class="overflow-auto">
                            <b-pagination
                                v-model="currentPage"
                                :total-rows="rows"
                                :per-page="perPage"
                                aria-controls="my-table"
                                :hide-goto-end-buttons="true">

                                <template v-slot:prev-text><span class="text-danger">Prev</span></template>
                                <template v-slot:next-text><span class="text-warning">Next</span></template>
                                <template v-slot:ellipsis-text>...</template>
                            </b-pagination>
                        </div>
                    </b-col>

                    <search :zipcodeList="zipcodeList" @onSearch="onSearch"/>

                </b-row>
            </div>
        </b-container>
    </div>

</template>

<script>
import { fas } from '@fortawesome/free-solid-svg-icons'
import { fab } from '@fortawesome/free-brands-svg-icons'
import axios from 'axios'
import Search from '~/components/Search'

export default {
    async asyncData ({ params }) {
        try {
            let { data } = await axios.get(`http://cdn.alternativemedia.com.au/geodata.json`);

            data = data.map(item => {
                return item.join(' ');
            })

            return { zipcodeList: data }
        } catch (e) {
            return { zipcodeList: [] }
        }
    },
    components: {
        Search,
    },
    data() {
        return {
            searchFor: 'something',
            categorySelect: 'default',
            text: '',
            perPage: 3,
            currentPage: 1,
            items: new Array(20),
        }
    },
    computed: {
        fas () {
            return fas
        },
        fab () {
            return fab
        },
        rows() {
            return this.items.length
        }
    },
    created(){
        this.searchFor = this.$route.query.s;
    },
    methods: {
        toSearch() {
            this.searchFor = this.text;
            this.$router.push({name: 'search', query: {s: this.text}})
        },
        onSearch(v) {
            this.searchFor = v;
        }
    }
}
</script>

<style lang="scss">

</style>
