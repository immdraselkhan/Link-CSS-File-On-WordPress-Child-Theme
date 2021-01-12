# Add this code on your function.php file

// Enter a name of the css on unique-id-1 & unique-id-2. Keep in mind always this name should be unique. And finally enter your CSS URL.

function child_enqueue_styles() {
  wp_enqueue_style( 'unique-id-1', 'URL of CSS', array());
  wp_enqueue_style( 'unique-id-2', 'URL of CSS', array());
}
add_action( 'wp_enqueue_scripts', 'child_enqueue_styles', 15 );
