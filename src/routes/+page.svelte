<script>
    // You can fetch data or define your layout logic here
    let artworks = [
      {
        title: "Queen",
        img: "/images/image-1.jpg",
        description: "A short description for your design."
      },
      {
        title: "Arctic Monkeys Poster",
        img: "/images/image-2.jpg",
        description: "Another example item."
      },
      {
        title: "666",
        img: "/images/dinosaur-666.jpg",
        description: ""
      },
      {
        title: "Featured Poster",
        img: "/images/skeleton-shades.jpg",
        description: "Some details about this piece."
      },
      {
        title: "Featured Poster",
        img: "/images/untitled.jpg",
        description: "Some details about this piece."
      },
      {
        title: "See the cat. See the cradle",
        img: "/images/cat-cradle.jpg",
        description: ""
      },
      
      
      
      
      
      // Add as many as you like...
    ];
  </script>
  
  <div class="container mx-auto p-4">
    <!-- Hero / Header Section -->
    <header class="text-center mb-10">
      <h1 class="text-4xl mb-2">ADM the Linocutter</h1>
      <p class="text-gray-600">A short subtitle or tagline here.</p>
    </header>

    <section id="newsletter" class="bg-base-200 p-6 rounded-lg">
        <h2 class="text-2xl font-bold mb-4 text-center">Get The Newsletter</h2>
        <p class="text-center mb-6">Sign up with to receive the latest about new work</p>
    
        <!-- Mailchimp Embed Form -->
        <div class="flex justify-center">
          <!-- This is a placeholder. Replace with your actual Mailchimp embed code. -->
          <div id="mc_embed_shell">
            <link href="//cdn-images.mailchimp.com/embedcode/classic-061523.css" rel="stylesheet" type="text/css">
        <style type="text/css">
              #mc_embed_signup{ false;clear:left; font:14px Helvetica,Arial,sans-serif; max-width: 600px;}
              /* Add your own Mailchimp form style overrides in your site stylesheet or in this style block.
                 We recommend moving this block and the preceding CSS link to the HEAD of your HTML file. */
      </style>
      <div id="mc_embed_signup">
          <form action="https://gmail.us19.list-manage.com/subscribe/post?u=b98f98981dc46f2bf330170ee&amp;id=928f2ce7ef&amp;f_id=00cfc2e1f0" method="post" id="mc-embedded-subscribe-form" name="mc-embedded-subscribe-form" class="validate" target="_blank">
              <div id="mc_embed_signup_scroll">
                  <div class="indicates-required">
                    <span class="asterisk">*</span> indicates required
                  </div>
                  <div class="mc-field-group">
                    <label for="mce-EMAIL">Email Address <span class="asterisk">*</span></label>
                    <input type="email" name="EMAIL" class="required email" id="mce-EMAIL" required="" value="">
                  </div>
                  <div class="mc-field-group">
                    <label for="mce-FNAME">First Name </label>
                    <input type="text" name="FNAME" class="text" id="mce-FNAME" value="">
                  </div>
                  <div class="mc-field-group">
                    <label for="mce-LNAME">Last Name </label>
                    <input type="text" name="LNAME" class="text" id="mce-LNAME" value="">
                  </div>
                  <div class="mc-address-group">
                    <div class="mc-field-group">
                      <label for="mce-ADDRESS-addr1">Address </label>
                      <input type="text" maxlength="70" name="ADDRESS[addr1]" id="mce-ADDRESS-addr1" class="" value="">
                    </div>
                    <div class="mc-field-group">
                      <label for="mce-ADDRESS-addr2">Address Line 2</label>
                      <input type="text" maxlength="70" name="ADDRESS[addr2]" id="mce-ADDRESS-addr2" value="">
                    </div>
                    <div class="mc-address-fields-group">
                      <div class="mc-field-group fg-city">
                        <label for="mce-ADDRESS-city">City</label>
                        <input type="text" maxlength="40" name="ADDRESS[city]" id="mce-ADDRESS-city" class="" value="">
                      </div>
                      <div class="mc-field-group fg-state">
                        <label for="mce-ADDRESS-state">State/Province/Region</label>
                        <input type="text" maxlength="20" name="ADDRESS[state]" id="mce-ADDRESS-state" class="" value="">
                      </div>
                      <div class="mc-field-group fg-postal">
                        <label for="mce-ADDRESS-zip">Postal / Zip Code</label>
                        <input type="text" maxlength="10" name="ADDRESS[zip]" id="mce-ADDRESS-zip" class="" value="">
                      </div>
                    </div>
                    <div class="mc-field-group">
                      <label for="mce-ADDRESS-country">Country</label>
                      <select name="ADDRESS[country]" id="mce-ADDRESS-country" class="">
                        <option value="Canada">Canada</option>
                        <option value="USA" selected="">USA</option>
                      </select>
                    </div>
                  </div>
              <div id="mce-responses" class="clear foot">
                  <div class="response" id="mce-error-response" style="display: none;"></div>
                  <div class="response" id="mce-success-response" style="display: none;"></div>
              </div>
          <div style="position: absolute; left: -5000px;" aria-hidden="true">
              /* real people should not fill this in and expect good things - do not remove this or risk form bot signups */
              <input type="text" name="b_b98f98981dc46f2bf330170ee_928f2ce7ef" tabindex="-1" value="">
          </div>
              <div class="optionalParent">
                  <div class="clear foot">
                      <input type="submit" name="subscribe" id="mc-embedded-subscribe" class="button btn-primary btn-lg" value="Signup">
                  </div>
              </div>
          </div>
      </form>
      </div>
      <script type="text/javascript" src="//s3.amazonaws.com/downloads.mailchimp.com/js/mc-validate.js"></script><script type="text/javascript">(function($) {window.fnames = new Array(); window.ftypes = new Array();fnames[0]='EMAIL';ftypes[0]='email';fnames[1]='FNAME';ftypes[1]='text';fnames[2]='LNAME';ftypes[2]='text';fnames[3]='ADDRESS';ftypes[3]='address';fnames[4]='PHONE';ftypes[4]='phone';}(jQuery));var $mcj = jQuery.noConflict(true);</script></div>
      
        </div>
      </section>
  
    <!-- Gallery Section -->
    <section class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6 mb-10 mt-10">
      {#each artworks as art}
        <div class="card shadow-xl bg-base-100">
          <figure>
            <img src={art.img} alt={art.title} class="object-cover w-full " />
          </figure>
          <div class="card-body">
            <h2 class="card-title text-2xl font-normal tracking-wide">{art.title}</h2>
            <p>{art.description}</p>
            
          </div>
        </div>
      {/each}
    </section>    
  </div>
  