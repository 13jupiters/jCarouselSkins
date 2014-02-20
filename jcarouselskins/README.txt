
jCarouselSkins
===============

jCarouselSkins is barely a module, in that it consists of a single function - jcarouselskins_jcarousel_skin_info.

But it's all you need to properly add new skins to jCarousel.

This mini-module includes one skin, jcBasic.


Requirements
============

jCarousel must be installed for this module to be of any use.


Description
===========

jCarouselSkins allows you to add new skins to jCarousel. One sample skin is provided - jcBasic, an approximation of a very
common carousel.

Implementation
==============

To add a new skin, follow these two steps:

1) place your skin folder in jCarouselSkins/skins. If your skin is called Awesome, your folder structure will be: jCarouselSkins/skins/Awesome.

2) add your skin info to jcarouselskins_jcarousel_skin_info():

  $skins['Awesome'] = array(
    'title' => t('Awesome'),
    'file' => 'skins/Awesome/jcarousel-awesome.css',
  );

Your skin will now be available in jCarousel settings for any views that use the jCarousel plugin. You may have to clear caches for your skin to appear.
