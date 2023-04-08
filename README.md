## Add Menu Page
```
add_action( 'admin_menu', 'wpse_91693_register' );
function wpse_91693_register()
{
    add_menu_page( 'Add Users To Course','Add Subscription Manually', 'manage_options', 'add-course', 'wpse_91693_render','dashicons-database-add',24 );
add_submenu_page('Add Users To Course','Add Subscription Manually', 'manage_options', 'add-course', 'wpse_91693_render');
    // add_submenu_page('add-course','Add new','Add new', 'activate_plugins', 'add_new_course', 'wpse_91694_render');

}
function wpse_91693_render()
{
echo "hello";
}
```

References: 

### [add_menu_page](https://developer.wordpress.org/reference/functions/add_menu_page/)
