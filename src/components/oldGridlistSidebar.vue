 <div class="panel panel-default" id="red-title">
          <!-- Heading    -->
          <div class="panel-heading" role="tab" id="headingFive">
            <h4 class="panel-title panel-title-tx">
              <a
                class="collapsed"
                role="button"
                data-toggle="collapse"
                data-parent="#accordion"
                href="#collapseFive"
                aria-expanded="true"
                aria-controls="collapseFive"
              >
                <i class="more-less glyphicon glyphicon-plus"></i>
                Search By Keyword
              </a>
            </h4>
          </div>
          <form
            method="get"
            action="https://carspot.scriptsbundle.com/search-cars/#red-title"
          >
            <!-- Content -->
            <div
              id="collapseFive"
              class="panel-collapse collapse"
              role="tabpanel"
              aria-labelledby="headingFive"
              aris-expanded="false"
            >
              <div class="panel-body">
                <div class="search-widget">
                  <input
                    id="autocomplete-dynamic"
                    autocomplete="off"
                    class="form-control"
                    placeholder="search"
                    type="text"
                    name="ad_title"
                    value
                  />
                  <button type="submit">
                    <i class="fa fa-search"></i>
                  </button>
                </div>
              </div>
            </div>
          </form>
        </div>

        <div class="panel panel-default" id="red-country">
          <!-- Heading -->
          <div class="panel-heading" role="tab" id="location_heading">
            <!-- Title -->
            <h4 class="panel-title">
              <a
                role="button"
                data-toggle="collapse"
                data-parent="#accordion"
                href="#ad-location"
                aria-expanded="true"
                aria-controls="ad-location"
              >
                <i class="more-less glyphicon glyphicon-plus"></i>
                Ads By Location
              </a>
            </h4>
            <!-- Title End -->
          </div>
          <!-- Content -->
          <form
            method="get"
            id="search_countries"
            action="https://carspot.scriptsbundle.com/search-cars/#red-country"
          >
            <div
              id="ad-location"
              class="panel-collapse collapse"
              role="tabpanel"
              aria-labelledby="location_heading"
            >
              <div class="panel-body countries">
                <ul>
                  <li>
                    <a href="javascript:void(0);" data-country-id="230">
                      United States
                      <span>(12)</span>
                    </a>
                  </li>
                </ul>
              </div>
            </div>
            <input type="hidden" name="country_id" id="country_id" value />
          </form>
          <div
            class="search-modal modal fade states_model"
            id="states_model"
            tabindex="-1"
            role="dialog"
            aria-hidden="true"
          >
            <div class="modal-dialog">
              <div class="modal-content">
                <div class="modal-header">
                  <button type="button" class="close" data-dismiss="modal">
                    <span aria-hidden="true">&#10005;</span>
                    <span class="sr-only">Close</span>
                  </button>
                  <h3 class="modal-title text-center">
                    <i class="icon-gears"></i>
                    Select Your Location
                  </h3>
                </div>
                <div class="modal-body">
                  <!-- content goes here -->
                  <div class="search-block">
                    <div class="row">
                      <div
                        class="col-md-12 col-xs-12 col-sm-12 popular-search"
                        id="countries_response"
                      ></div>
                    </div>
                  </div>
                </div>
                <div class="modal-footer">
                  <button
                    type="submit"
                    id="country-btn"
                    class="btn btn-lg btn-block"
                  >
                    Submit
                  </button>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="panel panel-default" id="red-price">
          <!-- Heading -->
          <div class="panel-heading" role="tab" id="headingfour">
            <h4 class="panel-title">
              <a
                class="collapsed"
                role="button"
                data-toggle="collapse"
                data-parent="#accordion"
                href="#collapsefour"
                aria-expanded="false"
                aria-controls="collapsefour"
              >
                <i class="more-less glyphicon glyphicon-plus"></i>
                Price
              </a>
            </h4>
          </div>
          <!-- Content -->
          <form
            method="get"
            action="https://carspot.scriptsbundle.com/search-cars/#red-price"
            class="carspot-price-form"
          >
            <div
              id="collapsefour"
              class="panel-collapse collapse"
              role="tabpanel"
              aria-labelledby="headingfour"
            >
              <div class="panel-body">
                <span class="price-slider-value">
                  Price ($ )
                  <span id="price-min"></span> -
                  <span id="price-max"></span>
                </span>
                <div id="price-slider"></div>
                <div class="input-group margin-top-10">
                  <input
                    type="text"
                    class="form-control"
                    name="min_price"
                    id="min_selected"
                    value="500"
                  />
                  <span class="input-group-addon">-</span>
                  <input
                    type="text"
                    class="form-control"
                    name="max_price"
                    id="max_selected"
                    value="100000"
                  />
                </div>
                <input type="hidden" id="min_price" value="500" />
                <input type="hidden" id="max_price" value="100000" />
                <input
                  type="submit"
                  class="btn btn-theme btn-sm margin-top-10"
                  value="Search"
                />
              </div>
            </div>
          </form>
        </div>
        <div class="panel panel-default" id="red-milage">
          <!-- Heading -->
          <div class="panel-heading" role="tab" id="ad-mileage">
            <h4 class="panel-title">
              <a
                class="collapsed"
                role="button"
                data-toggle="collapse"
                data-parent="#accordion"
                href="#mileage"
                aria-expanded="true"
                aria-controls="ad-mileage"
              >
                <i class="more-less glyphicon glyphicon-plus"></i>
                Ad Mileage (Km)
              </a>
            </h4>
          </div>
          <!-- Content -->
          <form
            method="get"
            id="get_mileage"
            action="https://carspot.scriptsbundle.com/search-cars/#red-milage"
          >
            <div
              id="mileage"
              class="panel-collapse collapse"
              role="tabpanel"
              aria-labelledby="ad-mileage"
            >
              <div class="panel-body">
                <div class="input-group margin-top-10">
                  <input
                    type="text"
                    class="form-control"
                    name="mileage_from"
                    data-parsley-type="digits"
                    data-parsley-required="true"
                    data-parsley-error-message="Value should be numeric"
                    placeholder="From"
                    id="mileage_from"
                    value
                  />
                  <span class="input-group-addon">-</span>
                  <input
                    type="text"
                    class="form-control"
                    data-parsley-required="true"
                    data-parsley-type="digits"
                    data-parsley-error-message="Value should be numeric"
                    placeholder="To"
                    name="mileage_to"
                    id="mileage_to"
                    value
                  />
                </div>
                <input
                  type="submit"
                  class="btn btn-theme btn-sm margin-top-10"
                  value="Search"
                />
              </div>
            </div>
          </form>
        </div>
        <div class="panel panel-default" id="red-years">
          <!-- Heading -->
          <div class="panel-heading" role="tab" id="headingYear">
            <h4 class="panel-title">
              <a
                class="collapsed"
                role="button"
                data-toggle="collapse"
                data-parent="#accordion"
                href="#Yearcollapse"
                aria-expanded="true"
                aria-controls="Yearcollapse"
              >
                <i class="more-less glyphicon glyphicon-plus"></i>
                Year
              </a>
            </h4>
          </div>
          <!-- Content -->
          <form
            method="get"
            action="https://carspot.scriptsbundle.com/search-cars/#red-years"
          >
            <div
              id="Yearcollapse"
              class="panel-collapse collapse"
              role="tabpanel"
              aria-labelledby="headingYear"
            >
              <div class="panel-body">
                <div class="input-group margin-top-10">
                  <span class="input-group-addon">From</span>
                  <select id="year_from" name="year_from" class="form-control">
                    <option value="2010">2010</option>
                    <option value="2011">2011</option>
                    <option value="2012">2012</option>
                    <option value="2013">2013</option>
                    <option value="2014">2014</option>
                    <option value="2015">2015</option>
                    <option value="2016">2016</option>
                    <option value="2017">2017</option>
                  </select>
                </div>
                <div class="input-group">
                  <span class="input-group-addon">To</span>
                  <select id="year_to" name="year_to" class="form-control">
                    <option value="2010">2010</option>
                    <option value="2011">2011</option>
                    <option value="2012">2012</option>
                    <option value="2013">2013</option>
                    <option value="2014">2014</option>
                    <option value="2015">2015</option>
                    <option value="2016">2016</option>
                    <option value="2017">2017</option>
                  </select>
                </div>
                <input
                  type="submit"
                  id="ad_year"
                  class="btn btn-theme btn-sm margin-top-10"
                  value="Search"
                />
              </div>
            </div>
          </form>
        </div>
        <div class="panel panel-default" id="red-transmission">
          <!-- Heading -->
          <div class="panel-heading" role="tab" id="body_transmission">
            <h4 class="panel-title">
              <a
                class="collapsed"
                role="button"
                data-toggle="collapse"
                data-parent="#accordion"
                href="#transmission"
                aria-expanded="true"
                aria-controls="body_transmission"
              >
                <i class="more-less glyphicon glyphicon-plus"></i>
                Transmission
              </a>
            </h4>
          </div>
          <!-- Content -->
          <form
            method="get"
            action="https://carspot.scriptsbundle.com/search-cars/#red-transmission"
          >
            <div
              id="transmission"
              class="panel-collapse collapse"
              role="tabpanel"
              aria-labelledby="body_transmission"
            >
              <div class="panel-body">
                <div class="skin-minimal">
                  <ul class="list">
                    <li>
                      <input
                        type="checkbox"
                        id="transmission-type-67"
                        value="Automatic"
                        name="transmission[]"
                      />
                      <label for="transmission-type-67">Automatic</label>
                    </li>
                    <li>
                      <input
                        type="checkbox"
                        id="transmission-type-151"
                        value="Manual"
                        name="transmission[]"
                      />
                      <label for="transmission-type-151">Manual</label>
                    </li>
                  </ul>
                </div>
              </div>
            </div>
          </form>
        </div>
        <div class="panel panel-default" id="red-engine-type">
          <!-- Heading -->
          <div class="panel-heading" role="tab" id="ad_body_type">
            <h4 class="panel-title">
              <a
                class="collapsed"
                role="button"
                data-toggle="collapse"
                data-parent="#accordion"
                href="#body_type"
                aria-expanded="true"
                aria-controls="ad_body_type"
              >
                <i class="more-less glyphicon glyphicon-plus"></i>
                Engine Type
              </a>
            </h4>
          </div>
          <!-- Content -->
          <form
            method="get"
            action="https://carspot.scriptsbundle.com/search-cars/#red-engine-type"
          >
            <div
              id="body_type"
              class="panel-collapse collapse"
              role="tabpanel"
              aria-labelledby="ad_body_type"
            >
              <div class="panel-body">
                <div class="skin-minimal">
                  <ul class="list">
                    <li>
                      <input
                        type="checkbox"
                        id="engine-type-81"
                        value="CNG"
                        name="engine_type[]"
                      />
                      <label for="engine-type-81">CNG</label>
                    </li>
                    <li>
                      <input
                        type="checkbox"
                        id="engine-type-96"
                        value="Diesel"
                        name="engine_type[]"
                      />
                      <label for="engine-type-96">Diesel</label>
                    </li>
                    <li>
                      <input
                        type="checkbox"
                        id="engine-type-126"
                        value="Hybrid"
                        name="engine_type[]"
                      />
                      <label for="engine-type-126">Hybrid</label>
                    </li>
                    <li>
                      <input
                        type="checkbox"
                        id="engine-type-176"
                        value="Petrol"
                        name="engine_type[]"
                      />
                      <label for="engine-type-176">Petrol</label>
                    </li>
                  </ul>
                </div>
              </div>
            </div>
          </form>
        </div>
        <div class="panel panel-default" id="red-engine-capacity">
          <!-- Heading -->
          <div class="panel-heading" role="tab" id="engince-capacity">
            <h4 class="panel-title">
              <a
                class="collapsed"
                role="button"
                data-toggle="collapse"
                data-parent="#accordion"
                href="#engine_capacity"
                aria-expanded="true"
                aria-controls="engince-capacity"
              >
                <i class="more-less glyphicon glyphicon-plus"></i>
                Engine Capacity (CC)
              </a>
            </h4>
          </div>
          <!-- Content -->
          <form
            method="get"
            action="https://carspot.scriptsbundle.com/search-cars/#red-engine-capacity"
          >
            <div
              id="engine_capacity"
              class="panel-collapse collapse"
              role="tabpanel"
              aria-labelledby="engince-capacity"
            >
              <div class="panel-body">
                <div class="skin-minimal">
                  <ul class="list">
                    <li>
                      <input
                        type="checkbox"
                        id="engine-capacity-29"
                        value="1000"
                        name="engine_capacity[]"
                      />
                      <label for="engine-capacity-29">1000 cc</label>
                    </li>
                    <li>
                      <input
                        type="checkbox"
                        id="engine-capacity-30"
                        value="1200"
                        name="engine_capacity[]"
                      />
                      <label for="engine-capacity-30">1200 cc</label>
                    </li>
                    <li>
                      <input
                        type="checkbox"
                        id="engine-capacity-31"
                        value="1500"
                        name="engine_capacity[]"
                      />
                      <label for="engine-capacity-31">1500 cc</label>
                    </li>
                    <li>
                      <input
                        type="checkbox"
                        id="engine-capacity-32"
                        value="2000"
                        name="engine_capacity[]"
                      />
                      <label for="engine-capacity-32">2000 cc</label>
                    </li>
                    <li>
                      <input
                        type="checkbox"
                        id="engine-capacity-42"
                        value="2500"
                        name="engine_capacity[]"
                      />
                      <label for="engine-capacity-42">2500 cc</label>
                    </li>
                    <li>
                      <input
                        type="checkbox"
                        id="engine-capacity-43"
                        value="3000"
                        name="engine_capacity[]"
                      />
                      <label for="engine-capacity-43">3000 cc</label>
                    </li>
                    <li>
                      <input
                        type="checkbox"
                        id="engine-capacity-44"
                        value="3500"
                        name="engine_capacity[]"
                      />
                      <label for="engine-capacity-44">3500 cc</label>
                    </li>
                    <li>
                      <input
                        type="checkbox"
                        id="engine-capacity-45"
                        value="800"
                        name="engine_capacity[]"
                      />
                      <label for="engine-capacity-45">800 cc</label>
                    </li>
                  </ul>
                </div>
              </div>
            </div>
          </form>
        </div>
        <div class="panel panel-default" id="red-body-type">
          <!-- Heading -->
          <div class="panel-heading" role="tab" id="bodytype">
            <h4 class="panel-title">
              <a
                class="collapsed"
                role="button"
                data-toggle="collapse"
                data-parent="#accordion"
                href="#ad_bodytype"
                aria-expanded="true"
                aria-controls="body_type"
              >
                <i class="more-less glyphicon glyphicon-plus"></i>
                Body Type
              </a>
            </h4>
          </div>
          <!-- Content -->
          <form
            method="get"
            action="https://carspot.scriptsbundle.com/search-cars/#red-body-type"
          >
            <div
              id="ad_bodytype"
              class="panel-collapse collapse"
              role="tabpanel"
              aria-labelledby="bodytype"
            >
              <div class="panel-body">
                <div class="skin-minimal">
                  <ul class="list">
                    <li>
                      <input
                        type="checkbox"
                        id="body-type-82"
                        value="Convertible"
                        name="body_type[]"
                      />
                      <label for="body-type-82">Convertible</label>
                    </li>
                    <li>
                      <input
                        type="checkbox"
                        id="body-type-85"
                        value="Coupe"
                        name="body_type[]"
                      />
                      <label for="body-type-85">Coupe</label>
                    </li>
                    <li>
                      <input
                        type="checkbox"
                        id="body-type-87"
                        value="Crossover"
                        name="body_type[]"
                      />
                      <label for="body-type-87">Crossover</label>
                    </li>
                    <li>
                      <input
                        type="checkbox"
                        id="body-type-100"
                        value="Electric"
                        name="body_type[]"
                      />
                      <label for="body-type-100">Electric</label>
                    </li>
                    <li>
                      <input
                        type="checkbox"
                        id="body-type-118"
                        value="Hatchback"
                        name="body_type[]"
                      />
                      <label for="body-type-118">Hatchback</label>
                    </li>
                    <li>
                      <input
                        type="checkbox"
                        id="body-type-127"
                        value="Hybrid"
                        name="body_type[]"
                      />
                      <label for="body-type-127">Hybrid</label>
                    </li>
                    <li>
                      <input
                        type="checkbox"
                        id="body-type-140"
                        value="Luxury"
                        name="body_type[]"
                      />
                      <label for="body-type-140">Luxury</label>
                    </li>
                    <li>
                      <input
                        type="checkbox"
                        id="body-type-203"
                        value="Sedan"
                        name="body_type[]"
                      />
                      <label for="body-type-203">Sedan</label>
                    </li>
                    <li>
                      <input
                        type="checkbox"
                        id="body-type-220"
                        value="SUV"
                        name="body_type[]"
                      />
                      <label for="body-type-220">SUV</label>
                    </li>
                    <li>
                      <input
                        type="checkbox"
                        id="body-type-226"
                        value="Truck"
                        name="body_type[]"
                      />
                      <label for="body-type-226">Truck</label>
                    </li>
                    <li>
                      <input
                        type="checkbox"
                        id="body-type-234"
                        value="Van/Minivan"
                        name="body_type[]"
                      />
                      <label for="body-type-234">Van/Minivan</label>
                    </li>
                    <li>
                      <input
                        type="checkbox"
                        id="body-type-243"
                        value="Wagon"
                        name="body_type[]"
                      />
                      <label for="body-type-243">Wagon</label>
                    </li>
                  </ul>
                </div>
              </div>
            </div>
          </form>
        </div>
        <div class="panel panel-default" id="red-color-family">
          <!-- Heading -->
          <div class="panel-heading" role="tab" id="ad-color-family">
            <h4 class="panel-title">
              <a
                class="collapsed"
                role="button"
                data-toggle="collapse"
                data-parent="#accordion"
                href="#ad-color"
                aria-expanded="true"
                aria-controls="ad-color-family"
              >
                <i class="more-less glyphicon glyphicon-plus"></i>
                Color Family
              </a>
            </h4>
          </div>
          <!-- Content -->
          <form
            method="get"
            action="https://carspot.scriptsbundle.com/search-cars/#red-color-family"
          >
            <div
              id="ad-color"
              class="panel-collapse collapse"
              role="tabpanel"
              aria-labelledby="ad-color-family"
            >
              <div class="panel-body">
                <div class="skin-minimal">
                  <ul class="list">
                    <li>
                      <input
                        type="checkbox"
                        id="ad_color-69"
                        value="Black"
                        name="color_family[]"
                      />
                      <label for="ad_color-69">Black</label>
                    </li>
                    <li>
                      <input
                        type="checkbox"
                        id="ad_color-70"
                        value="Blue"
                        name="color_family[]"
                      />
                      <label for="ad_color-70">Blue</label>
                    </li>
                    <li>
                      <input
                        type="checkbox"
                        id="ad_color-75"
                        value="Bronze"
                        name="color_family[]"
                      />
                      <label for="ad_color-75">Bronze</label>
                    </li>
                    <li>
                      <input
                        type="checkbox"
                        id="ad_color-113"
                        value="Gold"
                        name="color_family[]"
                      />
                      <label for="ad_color-113">Gold</label>
                    </li>
                    <li>
                      <input
                        type="checkbox"
                        id="ad_color-114"
                        value="Green"
                        name="color_family[]"
                      />
                      <label for="ad_color-114">Green</label>
                    </li>
                    <li>
                      <input
                        type="checkbox"
                        id="ad_color-115"
                        value="Grey"
                        name="color_family[]"
                      />
                      <label for="ad_color-115">Grey</label>
                    </li>
                    <li>
                      <input
                        type="checkbox"
                        id="ad_color-192"
                        value="Red"
                        name="color_family[]"
                      />
                      <label for="ad_color-192">Red</label>
                    </li>
                    <li>
                      <input
                        type="checkbox"
                        id="ad_color-206"
                        value="Silver"
                        name="color_family[]"
                      />
                      <label for="ad_color-206">Silver</label>
                    </li>
                    <li>
                      <input
                        type="checkbox"
                        id="ad_color-245"
                        value="White"
                        name="color_family[]"
                      />
                      <label for="ad_color-245">White</label>
                    </li>
                  </ul>
                </div>
              </div>
            </div>
          </form>
        </div>
        <div class="panel panel-default" id="red-ad-type">
          <!-- Heading -->
          <div class="panel-heading" role="tab" id="headingSeven">
            <h4 class="panel-title">
              <a
                class="collapsed"
                role="button"
                data-toggle="collapse"
                data-parent="#accordion"
                href="#collapseSeven"
                aria-expanded="true"
                aria-controls="collapseSeven"
              >
                <i class="more-less glyphicon glyphicon-plus"></i>
                Car Type
              </a>
            </h4>
          </div>
          <!-- Content -->
          <form
            method="get"
            action="https://carspot.scriptsbundle.com/search-cars/#red-ad-type"
          >
            <div
              id="collapseSeven"
              class="panel-collapse collapse"
              role="tabpanel"
              aria-labelledby="headingSeven"
            >
              <div class="panel-body">
                <div class="skin-minimal">
                  <ul class="list">
                    <li>
                      <input
                        tabindex="7"
                        type="checkbox"
                        id="minimal-radio-76"
                        name="ad_type[]"
                        value="Buy"
                      />
                      <label for="minimal-radio-76">Buy</label>
                    </li>
                    <li>
                      <input
                        tabindex="7"
                        type="checkbox"
                        id="minimal-radio-204"
                        name="ad_type[]"
                        value="Sell"
                      />
                      <label for="minimal-radio-204">Sell</label>
                    </li>
                  </ul>
                </div>
              </div>
            </div>
          </form>
        </div>
        <div class="panel panel-default" id="red-isurance">
          <!-- Heading -->
          <div class="panel-heading" role="tab" id="ad-insurance">
            <h4 class="panel-title">
              <a
                class="collapsed"
                role="button"
                data-toggle="collapse"
                data-parent="#accordion"
                href="#insurance"
                aria-expanded="true"
                aria-controls="ad-insurance"
              >
                <i class="more-less glyphicon glyphicon-plus"></i>
                Car Insurance
              </a>
            </h4>
          </div>
          <!-- Content -->
          <form
            method="get"
            action="https://carspot.scriptsbundle.com/search-cars/#red-isurance"
          >
            <div
              id="insurance"
              class="panel-collapse collapse"
              role="tabpanel"
              aria-labelledby="ad-insurance"
            >
              <div class="panel-body">
                <div class="skin-minimal">
                  <ul class="list">
                    <li>
                      <input
                        type="checkbox"
                        id="ad_color-170"
                        value="No"
                        name="insurance[]"
                      />
                      <label for="ad_color-170">No</label>
                    </li>
                    <li>
                      <input
                        type="checkbox"
                        id="ad_color-247"
                        value="Yes"
                        name="insurance[]"
                      />
                      <label for="ad_color-247">Yes</label>
                    </li>
                  </ul>
                </div>
              </div>
            </div>
          </form>
        </div>
        <div class="panel panel-default" id="red-assembly">
          <!-- Heading -->
          <div class="panel-heading" role="tab" id="ad-assembly-type">
            <h4 class="panel-title">
              <a
                class="collapsed"
                role="button"
                data-toggle="collapse"
                data-parent="#accordion"
                href="#ad-assembly"
                aria-expanded="true"
                aria-controls="ad-assembly-type"
              >
                <i class="more-less glyphicon glyphicon-plus"></i>
                Car Assembly
              </a>
            </h4>
          </div>
          <!-- Content -->
          <form
            method="get"
            action="https://carspot.scriptsbundle.com/search-cars/#red-assembly"
          >
            <div
              id="ad-assembly"
              class="panel-collapse collapse"
              role="tabpanel"
              aria-labelledby="ad-assembly-type"
            >
              <div class="panel-body">
                <div class="skin-minimal">
                  <ul class="list">
                    <li>
                      <input
                        type="checkbox"
                        id="ad-assembly-131"
                        value="Imported"
                        name="assembly[]"
                      />
                      <label for="ad-assembly-131">Imported</label>
                    </li>
                    <li>
                      <input
                        type="checkbox"
                        id="ad-assembly-139"
                        value="Local"
                        name="assembly[]"
                      />
                      <label for="ad-assembly-139">Local</label>
                    </li>
                  </ul>
                </div>
              </div>
            </div>
          </form>
        </div>
        <div class="panel panel-default" id="red-condition">
          <!-- Heading -->
          <div class="panel-heading" role="tab" id="headingThree">
            <h4 class="panel-title">
              <a
                class="collapsed"
                role="button"
                data-toggle="collapse"
                data-parent="#accordion"
                href="#collapseThree"
                aria-expanded="false"
                aria-controls="collapseThree"
              >
                <i class="more-less glyphicon glyphicon-plus"></i>
                Condition
              </a>
            </h4>
          </div>
          <!-- Content -->
          <form
            method="get"
            action="https://carspot.scriptsbundle.com/search-cars/#red-condition"
          >
            <div
              id="collapseThree"
              class="panel-collapse collapse"
              role="tabpanel"
              aria-labelledby="headingThree"
            >
              <div class="panel-body">
                <div class="skin-minimal">
                  <ul class="list">
                    <li>
                      <input
                        tabindex="7"
                        type="checkbox"
                        id="minimal-radio-166"
                        name="condition[]"
                        value="New"
                      />
                      <label for="minimal-radio-166">New</label>
                    </li>
                    <li>
                      <input
                        tabindex="7"
                        type="checkbox"
                        id="minimal-radio-231"
                        name="condition[]"
                        value="Used"
                      />
                      <label for="minimal-radio-231">Used</label>
                    </li>
                  </ul>
                </div>
              </div>
            </div>
          </form>
        </div>