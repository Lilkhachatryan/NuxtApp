<template>
  <div>
  <b-navbar toggleable="lg" type="light" variant="white">
    <b-navbar-brand href="#">
      <img src="~/assets/img/logo.svg"  width="200" height="46" class="d-inline-block align-top" alt="Logo">
    </b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav class="ml-auto mr-auto">
            <b-nav-item href="#">Compare Policies</b-nav-item>
            <b-nav-item-dropdown text="Health Funds" class="f-w-open" no-caret>
                <b-dropdown-text>
                  <b-container>
                    <b-row class="justify-content-center mb-3">
                      <b-col lg="2" md="3">
                        <a href="" class="d-block dropdown-menu-list">
                          <h4 class="dropdown-menu-list__title">BURA</h4>
                          <p class="m-0 text-white">Bupa has existed for over 60 years and is one of Australia’s leading health fund...</p>
                        </a>
                      </b-col>
                      <b-col lg="2" md="3">
                        <a href="" class="d-block dropdown-menu-list">
                          <h4 class="dropdown-menu-list__title">NIB</h4>
                          <p class="m-0 text-white">Originally known as Newcastle Industrial Benefits (nib) Hospital Fund, nib was set...</p>
                        </a>
                      </b-col>
                      <b-col lg="2" md="3">
                        <a href="" class="d-block dropdown-menu-list">
                          <h4 class="dropdown-menu-list__title">AHM</h4>
                          <p class="m-0 text-white">AHM has been around for over 40 years, having started out as a small club in 1971</p>
                        </a>
                      </b-col>
                      <b-col lg="2" md="3">
                        <a href="" class="btn btn-success btn-default btn-block btn-r">Compare Policies</a>
                        <a href="" class="req-call-link"><fa :icon="fas.faPhoneAlt"/>  Request a call</a>
                      </b-col>
                    </b-row>
                    <b-row class="justify-content-center">
                      <b-col lg="2" md="3">
                        <a href="" class="d-block dropdown-menu-list">
                          <h4 class="dropdown-menu-list__title">HCF</h4>
                          <p class="m-0 text-white">Originally known as the Metropolitan Hospital Contributions Fund, HCF was set up i...</p>
                        </a>
                      </b-col>
                      <b-col lg="2" md="3">
                        <a href="" class="d-block dropdown-menu-list">
                          <h4 class="dropdown-menu-list__title">HBA</h4>
                          <p class="m-0 text-white">HBA is a private health insurance provider that is owned by Bupa Group Internation...</p>
                        </a>
                      </b-col>
                      <b-col lg="2" md="3">
                        <a href="" class="d-block dropdown-menu-list">
                          <h4 class="dropdown-menu-list__title">HBF</h4>
                          <p class="m-0 text-white">The Hospital Benefit Fund, or HBF, was established in 1941 as a not-for-profit org...</p>
                        </a>
                      </b-col>
                      <b-col lg="2" md="3" class="text-center">
                        <a href="" class="btn btn-default btn-outline-light mt-4">View All</a>
                      </b-col>
                    </b-row>
                  </b-container>
                </b-dropdown-text>
            </b-nav-item-dropdown>
            <b-nav-item-dropdown text="Guides" class="f-w-open" no-caret>
                <b-dropdown-text>
                  <b-container>
                    <b-row class="justify-content-center mb-3">
                      <b-col md="3">
                        <a href="" class="link-w-icon text-white text-sm"><fa :icon="fas.faHeart"/> By Relationship Status</a>
                        <a href="" class="link-w-icon text-white text-sm"><fa :icon="fas.faChessBishop"/> By State</a>
                        <a href="" class="link-w-icon text-white text-sm"><fa :icon="fas.faChartLine"/> Rate Rise Hub</a>
                      </b-col>
                      <b-col md="3">
                        <a href="" class="link-w-icon text-white text-sm"><fa :icon="fas.faListAlt"/> By Cover Type</a>
                        <a href="" class="link-w-icon text-white text-sm"><fa :icon="fas.faChild"/> For Children</a>
                      </b-col>
                      <b-col md="3">
                        <a href="" class="link-w-icon text-white text-sm"><fa :icon="fas.faUsers"/> By Life Stage</a>
                        <a href="" class="link-w-icon text-white text-sm"><fa :icon="fas.faBook"/> General Guides</a>
                      </b-col>
                      <b-col md="2" class="text-center">
                        <a href="" class="btn btn-success btn-default btn-block btn-r">Compare Policies</a>
                        <a href="" class="req-call-link"><fa :icon="fas.faPhoneAlt"/>  Request a call</a>
                        <a href="" class="btn btn-default btn-outline-light mt-4">See All</a>
                      </b-col>
                    </b-row>
                  </b-container>
                </b-dropdown-text>
            </b-nav-item-dropdown>
            <b-nav-item-dropdown text="Calculators" class="f-w-open" no-caret>
                <b-dropdown-text>
                  <b-container>
                    <b-row class="justify-content-center mb-3">
                      <b-col lg="3">
                        <a href="" class="link-w-icon text-white"><fa class="text-success text-sm" :icon="fas.faPlay"/> Waiting Period Calculator</a>
                        <a href="" class="link-w-icon text-white"><fa class="text-success text-sm" :icon="fas.faPlay"/> Medicare Levy Calculator</a>
                      </b-col>
                      <b-col lg="3">
                        <a href="" class="link-w-icon text-white"><fa class="text-success text-sm" :icon="fas.faPlay"/> Rebate Calculator</a>
                        <a href="" class="link-w-icon text-white"><fa class="text-success text-sm" :icon="fas.faPlay"/> Waiting List Calculator</a>
                      </b-col>
                      <b-col lg="3">
                        <a href="" class="link-w-icon text-white"><fa class="text-success text-sm" :icon="fas.faPlay"/> Policy Cost Calculator</a>
                        <a href="" class="link-w-icon text-white"><fa class="text-success text-sm" :icon="fas.faPlay"/> Premium Increase Calculator</a>
                      </b-col>
                      <b-col lg="3" class="text-center">
                        <a href="" class="btn btn-success btn-default btn-block btn-r">Compare Policies</a>
                        <a href="" class="req-call-link"><fa :icon="fas.faPhoneAlt"/>  Request a call</a>
                      </b-col>
                    </b-row>
                  </b-container>
                </b-dropdown-text>
            </b-nav-item-dropdown>
            <b-nav-item-dropdown text="About Us" class="f-w-open" no-caret>
                <b-dropdown-text>
                  <b-container>
                    <b-row class="justify-content-center mb-3">
                      <b-col lg="3">
                        <a href="" class="link-w-icon text-white"><fa class="text-success text-sm" :icon="fas.faPlay"/> What We Do</a>
                        <a href="" class="link-w-icon text-white"><fa class="text-success text-sm" :icon="fas.faPlay"/> How Our Service Works</a>
                        <a href="" class="link-w-icon text-white"><fa class="text-success text-sm" :icon="fas.faPlay"/> How We Make Money</a>
                      </b-col>
                      <b-col lg="3">
                        <a href="" class="link-w-icon text-white"><fa class="text-success text-sm" :icon="fas.faPlay"/> Meet The Team</a>
                        <a href="" class="link-w-icon text-white"><fa class="text-success text-sm" :icon="fas.faPlay"/> Concierge</a>
                        <a href="" class="link-w-icon text-white"><fa class="text-success text-sm" :icon="fas.faPlay"/> Customer Reviews</a>
                      </b-col>
                      <b-col lg="3">
                        <a href="" class="link-w-icon text-white"><fa class="text-success text-sm" :icon="fas.faPlay"/> Industry Newsroom</a>
                        <a href="" class="link-w-icon text-white"><fa class="text-success text-sm" :icon="fas.faPlay"/> Privacy Policy</a>
                        <a href="" class="link-w-icon text-white"><fa class="text-success text-sm" :icon="fas.faPlay"/> Contact Us</a>
                      </b-col>
                      <b-col lg="3" class="text-center">
                        <a href="" class="btn btn-success btn-default btn-block btn-r">Compare Policies</a>
                        <a href="" class="req-call-link"><fa :icon="fas.faPhoneAlt"/>  Request a call</a>
                      </b-col>
                    </b-row>
                  </b-container>
                </b-dropdown-text>
            </b-nav-item-dropdown>
            <b-nav-item href="#">Health & Lifestyle</b-nav-item>

            <b-nav-form class="nav-search">
              <b-button 
                :variant="isSearchActive ? 'success' : ''" class="text-sm" 
                @click="toSearch">
                  <fa :icon="fas.faSearch"/>
              </b-button>
              <b-form-input v-model="text" 
                :class="{'active': isSearchActive}" 
                placeholder="Enter keyword..." ></b-form-input>
            </b-nav-form>

            <b-nav-item href="tel:1300163402" class="nav-item--phone">
              <span class="fa-icon text-white text-sm bg-success d-inline-block">
                <fa :icon="fas.faPhoneAlt"/>
              </span>
                1300 163 402 <small>Mon-Fri 8am-8pm AEST <br> Sat 10am-5pm AEST</small>
            </b-nav-item>
        </b-navbar-nav>
    </b-collapse>
  </b-navbar>
  <nuxt/>
  </div>
</template>

<script>
import { fas } from '@fortawesome/free-solid-svg-icons'
import { fab } from '@fortawesome/free-brands-svg-icons'

export default {
  computed: {
    fas () {
        return fas
    },
    fab () {
        return fab
    },
  },
  data:() => {
    return {
      isSearchActive: false,    
      text: '',
    }
  },
  methods: {
    toSearch() {
      if(!this.isSearchActive) {
        this.isSearchActive = !this.isSearchActive;
        return
      }

      this.isSearchActive = !this.isSearchActive;
      this.$router.push({name: 'search', query: {s: this.text}});
      this.text = '';
    },
  }
}
</script>
