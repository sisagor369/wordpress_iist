# wordpress_iist
~~~html
register_custom_post register_post_type
index.php file er kaj eta 

 <div class="services" id="blog">
              <h1 class="h1">MY SKILL</h1>
              <?php
        $args = array (
          'post_type'    => 'My Skill',
          'post_per_page'=> 4,
          'order'        => 'ASC'
        );
        $loop = new WP_Query($args);
        while ($loop-> have_posts()) : $loop -> the_post();
        ?>
            <div class="first f_undr">
                <!-- <i class="fab fa-html5"></i> -->
                <h1><?php the_title();?> </h1>
                <p><?php echo get_field('skill_details');?></p>
            </div>
            <?php endwhile; ?>
        </div>
~~~
