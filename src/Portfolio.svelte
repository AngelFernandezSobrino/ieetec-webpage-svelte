<script>
  import { images } from "./imgData.js";
  import { categories } from "./imgData.js";

  import ButtonContainer from "./ButtonContainer.svelte";
  import Gallery from "./Gallery.svelte";

  let selected = "all";

  const filterSelection = (e) => (selected = e.target.dataset.name);
</script>

<!-- Start Portfolio -->
<section id="mu-portfolio">
  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <div class="mu-portfolio-area">
          <!-- Title -->
          <div class="row">
            <div class="col-md-12">
              <div class="mu-title">
                <h2>Ejemplos de proyectos realizados&nbsp;</h2>
                <p>
                  Aqui se recopilan algunos de los tipos de proyectos que
                  podemos desarrollar e instalar para nuestros clientes
                </p>
              </div>
            </div>
          </div>

          <div class="row">
            <!-- Start Portfolio Filter -->
            <div class="mu-portfolio-filter-area">
              <ul class="mu-simplefilter">
                <li class="active" data-filter="all">All<span>/</span></li>
                <li data-filter="1">Automatizacion<span>/</span></li>
                <li data-filter="2">HVAC<span>/</span></li>
                <li data-filter="3">Clean Room<span>/</span></li>
                <li data-filter="4">Mantenimiento</li>
                <!-- <li data-filter="5">Branding</li> -->
              </ul>
            </div>

            <!-- Start Portfolio Content -->
            <div class="mu-portfolio-content">
              <div class="filtr-container">
                <div
                  class="col-xs-6 col-sm-6 col-md-4 filtr-item"
                  data-category="1"
                >
                  <a
                    class="mu-imglink"
                    href="/assets/images/portfolio/img-1.jpg"
                    title="CONTROL DE CALIDAD"
                  >
                    <img
                      class="img-responsive"
                      src={img1}
                      alt="CONTROL DE CALIDAD"
                    />
                    <div class="mu-filter-item-content">
                      <h4 class="mu-filter-item-title">CONTROL DE CALIDAD</h4>
                      <span class="fa fa-long-arrow-right" />
                    </div>
                  </a>
                </div>

                <div
                  class="col-xs-6 col-sm-6 col-md-4 filtr-item"
                  data-category="2"
                >
                  <a
                    class="mu-imglink"
                    href="/assets/images/portfolio/img-1.jpg"
                    title="CONTROL DE CALIDAD"
                  >
                    <img
                      class="img-responsive"
                      src={img1}
                      alt="CONTROL DE CALIDAD"
                    />
                    <div class="mu-filter-item-content">
                      <h4 class="mu-filter-item-title">CONTROL DE CALIDAD</h4>
                      <span class="fa fa-long-arrow-right" />
                    </div>
                  </a>
                </div>

                <div
                  class="col-xs-6 col-sm-6 col-md-4 filtr-item"
                  data-category="3"
                >
                  <a
                    class="mu-imglink"
                    href="/assets/images/portfolio/img-1.jpg"
                    title="CONTROL DE CALIDAD"
                  >
                    <img
                      class="img-responsive"
                      src="/assets/images/portfolio/img-1.jpg"
                      alt="CONTROL DE CALIDAD"
                    />
                    <div class="mu-filter-item-content">
                      <h4 class="mu-filter-item-title">CONTROL DE CALIDAD</h4>
                      <span class="fa fa-long-arrow-right" />
                    </div>
                  </a>
                </div>
              </div>
            </div>
            <!-- End Portfolio Content -->
          </div>
        </div>
      </div>
    </div>
  </div>
</section>
<!-- End Portfolio -->
