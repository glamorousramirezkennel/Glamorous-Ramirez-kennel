<?php $year = date('Y'); ?></main><footer class="site-footer"><div class="container">
<div>© <?php echo $year; ?> Glamorous Ramirez Kennel — Based in Missouri • All rights reserved.</div>
</div><?php wp_footer(); ?></footer></body></html>

<?php get_header(); ?><section class="section"><h1>Glamorous Ramirez Kennel</h1>
<p>Where Elegance Meets Loyalty.</p>
</section><?php get_footer(); ?>
<?php
function grk_setup(){ add_theme_support('title-tag'); add_theme_support('post-thumbnails'); register_nav_menus(array('primary'=>'Primary Menu')); }
add_action('after_setup_theme','grk_setup');
function grk_scripts(){ wp_enqueue_style('grk-style', get_stylesheet_uri(), array(), '1.0'); }
add_action('wp_enqueue_scripts','grk_scripts');
?>
- index.html (main site, mobile-responsive, shimmer on load)
- thank-you.html (confirmation page after payment)
- /assets (logos, favicon, crown-shimmer.css, social icons)
- /glamorous-ramirez-kennel (WordPress theme folder)
<?php ?><!doctype html><html <?php language_attributes(); ?>><head>
<meta charset="<?php bloginfo('charset'); ?>"><meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="icon" href="<?php echo esc_url(get_template_directory_uri().'/assets/favicon.ico'); ?>" sizes="any">
<?php wp_head(); ?></head><body <?php body_class(); ?>>
<header class="site-header"><div class="container brand">
<img class="logo" src="<?php echo esc_url(get_template_directory_uri().'/assets/logo-transparent.png'); ?>" alt="Glamorous Ramirez Kennel">
<div class="tagline">Where Elegance Meets Loyalty</div>
<nav class="navbar"><?php wp_nav_menu(array('theme_location'=>'primary','container'=>false,'fallback_cb'=>false)); ?></nav>
</div></header><main class="container">
STRIPE
- "Reserve Now" buttons use your checkout link:
  https://buy.stripe.com/9B628r2Er2R94Ipf5Cbwk01
   Thank you for reserving your Doberman puppy!
Your deposit has been received. We’ll be in touch shortly to confirm your details and send updates about your puppy’s progress.
If you have any questions, please reach out:
📞 (636) 849-5577 • 📧 glamorousramirezkennel@gmail.com
Return to Home

- (Optional) Add individual links per puppy later by editing index.html.
- index.html (main site, mobile-responsive, shimmer on load)
- thank-you.html (confirmation page after payment)
- /assets (logos, favicon, crown-shimmer.css, social icons)
- /glamorous-ramirez-kennel (WordPress theme folder)
