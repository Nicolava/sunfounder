.. note::

    Hello, welcome to the SunFounder Raspberry Pi & Arduino & ESP32 Enthusiasts Community on Facebook! Dive deeper into Raspberry Pi, Arduino, and ESP32 with fellow enthusiasts.

    **Why Join?**

    - **Expert Support**: Solve post-sale issues and technical challenges with help from our community and team.
    - **Learn & Share**: Exchange tips and tutorials to enhance your skills.
    - **Exclusive Previews**: Get early access to new product announcements and sneak peeks.
    - **Special Discounts**: Enjoy exclusive discounts on our newest products.
    - **Festive Promotions and Giveaways**: Take part in giveaways and holiday promotions.

    👉 Ready to explore and create with us? Click [|link_sf_facebook|] and join today!

.. _1.6_scratch:

1.6 Vanishing Vase
========================

Now let's do a little magic trick, do nothing, and then the vase somehow disappears.

.. image:: img/1.6_header.png

Required Components
------------------------------

In this project, we need the following components. 

.. image:: img/1.6_component.png

It's definitely convenient to buy a whole kit, here's the link: 

.. list-table::
    :widths: 20 20 20
    :header-rows: 1

    *   - Name	
        - ITEMS IN THIS KIT
        - LINK
    *   - Raphael Kit
        - 337
        - |link_Raphael_kit|

You can also buy them separately from the links below.

.. list-table::
    :widths: 30 20
    :header-rows: 1

    *   - COMPONENT INTRODUCTION
        - PURCHASE LINK

    *   - :ref:`cpn_gpio_extension_board`
        - |link_gpio_board_buy|
    *   - :ref:`cpn_breadboard`
        - |link_breadboard_buy|
    *   - :ref:`cpn_wires`
        - |link_wires_buy|
    *   - :ref:`cpn_reed_switch`
        - |link_reed_switch_buy|

Build the Circuit
---------------------

.. image:: img/1.6.png

Load the Code and See What Happens
---------------------------------------

Load the code file (``1.6_vanishing_vase.sb3``) to Scratch 3.

When you use a magnet near the reed switch module, a vase will appear on the stage, take away the magnet and the vase will disappear.

Tips on Sprite
----------------

Select Sprite1 and click **Costumes** in the top left corner; upload **desk1.png** and **desk2.png** from the ``~/raphael-kit/scratch/picture`` path via the **Upload Costume** button; delete the default 2 costumes, and rename the sprite to **desk**.

.. image:: img/1.6_vase.png

Tips on Codes
--------------

.. image:: img/1.6_reed2.png
  :width: 400

When the magnet is close to the reed switch module, gpio17 is low, and the costume of the **desk** sprite is switched to **desk1** (the vase is still on the desk).

.. image:: img/1.6_reed3.png
  :width: 400

After taking away the magnet, gpio17 is high, at this time the costume of the **desk** sprite is switched to **desk2** (only one desk).
