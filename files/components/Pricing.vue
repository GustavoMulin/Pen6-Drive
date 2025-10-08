<template>
  <section class="pricing-one" id="pricing">
    <div class="container">
      <div class="block-title text-center">
        <h3>Escolha o <span>plano</span> que mais combina com você</h3>
      </div><!-- /.block-title text-center -->
      <ul class="list-inline text-center switch-toggler-list" role="tablist" id="switch-toggle-tab">
        <li :class="`${month ? 'month active' : 'month'}`"><a href="#">Mensal</a></li>
        <li>
          <!-- Rounded switch -->
          <label :class="`${year ? 'switch off' : 'switch on'}`">
            <span @click="handleToggle" class="slider round"></span>
          </label>
        </li>
        <li :class="`${year ? 'year active' : 'year'}`"><a href="#">Anual</a></li>
      </ul><!-- /.list-inline -->

      <div class="tabed-content">
        <div id="month" :style="`display: ${month ? 'block' : 'none'}`">
          <div class="row">
            <div class="col-lg-4 animated fadeInLeft">
              <div class="pricing-one__single">
                <div class="pricing-one__inner">
                  <i class="oapee-icon-send"></i>
                  <p>Basic Pack</p>
                  <h3><span class="fonte">$20.00</span></h3>
                  <ul class="list-unstyled pricing-one__list">
                    <li><i class="fa fa-check"></i>Extra features</li>
                    <li><i class="fa fa-check"></i>Lifetime free support</li>
                    <li><i class="fa fa-check"></i>Upgrate options</li>
                    <li><i class="fa fa-check"></i>Full access</li>
                  </ul><!-- /.list-unstyled pricing-one__list -->
                  <a href="#" class="thm-btn pricing-one__btn"><span>Choose Plan</span></a>
                  <!-- /.thm-btn -->
                </div><!-- /.pricing-one__inner -->
              </div><!-- /.pricing-one__single -->
            </div><!-- /.col-lg-4 -->
            <div class="col-lg-4 animated fadeInUp">
              <div class="pricing-one__single">
                <div class="pricing-one__inner">
                  <i class="oapee-icon-shuttle"></i>
                  <p>Standard Pack</p>
                  <h3><span class="fonte">$30.00</span></h3>
                  <ul class="list-unstyled pricing-one__list">
                    <li><i class="fa fa-check"></i>Extra features</li>
                    <li><i class="fa fa-check"></i>Lifetime free support</li>
                    <li><i class="fa fa-check"></i>Upgrate options</li>
                    <li><i class="fa fa-check"></i>Full access</li>
                  </ul><!-- /.list-unstyled pricing-one__list -->
                  <a href="#" class="thm-btn pricing-one__btn"><span>Choose Plan</span></a>
                  <!-- /.thm-btn -->
                </div><!-- /.pricing-one__inner -->
              </div><!-- /.pricing-one__single -->
            </div><!-- /.col-lg-4 -->
            <div class="col-lg-4 animated fadeInRight">
              <div class="pricing-one__single">
                <div class="pricing-one__inner">
                  <i class="oapee-icon-send"></i>
                  <p>Ultimate Pack</p>
                  <h3><span class="fonte">$49.00</span></h3>
                  <ul class="list-unstyled pricing-one__list">
                    <li><i class="fa fa-check"></i>Extra features</li>
                    <li><i class="fa fa-check"></i>Lifetime free support</li>
                    <li><i class="fa fa-check"></i>Upgrate options</li>
                    <li><i class="fa fa-check"></i>Full access</li>
                  </ul><!-- /.list-unstyled pricing-one__list -->
                  <a href="#" class="thm-btn pricing-one__btn"><span>Choose Plan</span></a>
                  <!-- /.thm-btn -->
                </div><!-- /.pricing-one__inner -->
              </div><!-- /.pricing-one__single -->
            </div><!-- /.col-lg-4 -->
          </div><!-- /.row -->
        </div><!-- /#month -->
        <div id="year" :style="`display: ${year ? 'block' : 'none'}`">
          <div class="row">
            <div class="col-lg-4 animated fadeInLeft">
              <div class="pricing-one__single">
                <div class="pricing-one__inner">
                  <i class="oapee-icon-send"></i>
                  <p>Basic Pack</p>
                  <h3><span class="fonte">$59.00</span></h3>
                  <ul class="list-unstyled pricing-one__list">
                    <li><i class="fa fa-check"></i>Extra features</li>
                    <li><i class="fa fa-check"></i>Lifetime free support</li>
                    <li><i class="fa fa-check"></i>Upgrate options</li>
                    <li><i class="fa fa-check"></i>Full access</li>
                  </ul><!-- /.list-unstyled pricing-one__list -->
                  <a href="#" class="thm-btn pricing-one__btn"><span>Choose Plan</span></a>
                  <!-- /.thm-btn -->
                </div><!-- /.pricing-one__inner -->
              </div><!-- /.pricing-one__single -->
            </div><!-- /.col-lg-4 -->
            <div class="col-lg-4 animated fadeInUp">
              <div class="pricing-one__single">
                <div class="pricing-one__inner">
                  <i class="oapee-icon-shuttle"></i>
                  <p>Standard Pack</p>
                  <h3><span class="fonte">$79.00</span></h3>
                  <ul class="list-unstyled pricing-one__list">
                    <li><i class="fa fa-check"></i>Extra features</li>
                    <li><i class="fa fa-check"></i>Lifetime free support</li>
                    <li><i class="fa fa-check"></i>Upgrate options</li>
                    <li><i class="fa fa-check"></i>Full access</li>
                  </ul><!-- /.list-unstyled pricing-one__list -->
                  <a href="#" class="thm-btn pricing-one__btn"><span>Choose Plan</span></a>
                  <!-- /.thm-btn -->
                </div><!-- /.pricing-one__inner -->
              </div><!-- /.pricing-one__single -->
            </div><!-- /.col-lg-4 -->
            <div class="col-lg-4 animated fadeInRight">
              <div class="pricing-one__single">
                <div class="pricing-one__inner">
                  <i class="oapee-icon-send"></i>
                  <p>Ultimate Pack</p>
                  <h3><span class="fonte">$99.00</span></h3>
                  <ul class="list-unstyled pricing-one__list">
                    <li><i class="fa fa-check"></i>Extra features</li>
                    <li><i class="fa fa-check"></i>Lifetime free support</li>
                    <li><i class="fa fa-check"></i>Upgrate options</li>
                    <li><i class="fa fa-check"></i>Full access</li>
                  </ul><!-- /.list-unstyled pricing-one__list -->
                  <a href="#" class="thm-btn pricing-one__btn"><span>Choose Plan</span></a>
                  <!-- /.thm-btn -->
                </div><!-- /.pricing-one__inner -->
              </div><!-- /.pricing-one__single -->
            </div><!-- /.col-lg-4 -->
          </div><!-- /.row -->
        </div><!-- /#year -->
      </div><!-- /.tabed-content -->

    </div><!-- /.container -->
  </section>
</template>

<script>
  export default {
    name: "Pricing",
    data(){
      return {
        month: true,
        year: false
      }
    },
    methods: {

      handleToggle(){
        const month = this.month;
        const year = this.year;

        if(month){
          this.year = true;
          this.month = false;
        }
        if(year){
          this.year = false;
          this.month = true;
        }

      }
    }
  }
</script>

<style scoped>

</style>
