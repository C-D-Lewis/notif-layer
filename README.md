# notif-layer

Simple top-down notification Layer subclass for Pebble.

![](screenshots/screenshot.gif)


## How to use

1. Create as with a normal `Layer`, specifying the `Window` it will display
   within:

      NotifLayer *notif_layer = notif_layer_create(some_parent_window);

2. Show a notification. Long text will automatically scroll:

      notif_layer_show(notif_layer, "This is an example notification!");

3. Destroy the `NotifLayer` when the parent `Window` is exiting:

      notif_layer_destroy(notif_layer);
