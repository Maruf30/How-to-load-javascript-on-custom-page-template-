# How-to-load-javascript-on-custom-page-template-


add_action('wp_enqueue_scripts','Load_Template_Scripts_wpa83855');
function Load_Template_Scripts_wpa83855(){
    if ( is_page_template('template-scrollcontent.php') ) {
        wp_enqueue_script('my-script', '/wp-content/themes/theme_name/js/shadowbox/shadowbox.js');
       wp_enqueue_script('my-scripts', '/wp-content/themes/theme_name/js/jquery.tools.minc619.js');
    } 
}
