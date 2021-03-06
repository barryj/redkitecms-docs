RedKite CMS Practical Manual - Part 2
=====================================

Welcome to the second part of RedKite CMS Practical Manual.

This second part is focused on pages management.

Add a new page
~~~~~~~~~~~~~~

.. image:: //bundles/redkitelabswebsite/media/bootbusiness/img17.jpg

Click on the toolbar down tab to open it and click on the "Pages" button to open
the pages management panel.

.. image:: //bundles/redkitelabswebsite/media/bootbusiness/img18.jpg

Type "product 1" in the "Page name" textbox, choose "product" from the "Templates" combobox,
and click the "Published" checkbox to immediately publish the page when you deploy the website
for production.

Click the "SEO" tab and type "redkite content management system" into the "Permalink" 
textarea. The permalink is the real name of the page, so it is important to choose a 
significant name since this information will be indexed by search engines.

Don't worry about the spaces, RedKite CMS "slugifies" the page name and permalink for 
you, so page name is converted to "product-1" and permalink is converted to
"redkite-content-management-system".

While it is not mandatory, you should fill the "Title" and the "Description" information 
because it is important when search engines will index your page.

Another important section for SEO (Search Engines Optimization) is the "Sitemap" one,
where you can assign the priority to page.

When you are done, click the "Save" button to add the page to your website, then close
the panel by clicking the bottom of panel.

Manage menu links on main toolbar
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. image:: //bundles/redkitelabswebsite/media/bootbusiness/img19.jpg

Place the cursor over the toolbar container's area and click into it.

.. image:: //bundles/redkitelabswebsite/media/bootbusiness/img20.jpg

Click on the red icon under the first link to remove it, then repeat the operation
for the other one, then click into the toolbar and click the "Add" button.

.. image:: //bundles/redkitelabswebsite/media/bootbusiness/img21.jpg

Choose the "Nav dropdown" block to add a dropdown menu to the toolbar. 

.. note:: 

    All these steps will be simplified when the "Move" function is implemented.

.. image:: //bundles/redkitelabswebsite/media/bootbusiness/img22.jpg

Put your mouse into the dropdown block's area and click to start editing the block.

Click into the "Button Text" textbox and type "Products and Services", then click the "Menu items"
button. 

.. image:: //bundles/redkitelabswebsite/media/bootbusiness/img23.jpg

Click on the "Item 1" and choose "redkite-content-management-system" to assign the page 
to a link.

.. image:: //bundles/redkitelabswebsite/media/bootbusiness/img24.jpg

Now right-click "Item 1", choose "Rename" and type "RedKite CMS". Click the 
Save button to confirm.

Moving through pages
~~~~~~~~~~~~~~~~~~~~

You have two options to navigate to the new page:

    1. Click a link on the page when the page is not in edit mode
    2. Choose the page from the "Nav" section
    
Click the "Stop" button to exit from edit mode, open the "Products and Services" dropdown
menu and click the "RedKite CMS" link, to navigate to the selected page.

Here we should talk about the RedKite CMS product by adding an image that describes 
this product, and start editing the contents. However this is not the purpose of this tutorial, so
feel free to play with contents on this page in your own time. 

When you are done, click the nav button to open the navigation menu.

.. image:: //bundles/redkitelabswebsite/media/bootbusiness/img26.jpg

From this panel, you may choose the language and the page to move to. This panel is very
useful because it gives you access to all the pages of the website, so when a page is
not linked you can open it using this menu.

Choose index from the pages combobox and automatically RedKite CMS will move to 
the website's home page.

Add more pages
~~~~~~~~~~~~~~

Add these pages and always check the "Published" checkbox:

    - Page name: works - Template: empty
    - Page name: partnership - Template: two_columns
    - Page name: leadership - Template: empty    
    - Page name: news - Template: two_columns
    - Page name: events - Template: empty    

.. note:: 

    if you don't provide a permalink, the page name is used. Please do not 
    do this for your website when page names are poor as the ones you've just added.

Add a new "Nav dropdown" to the top navbar, name it "About", open the "Menu items"
and link the first three pages.

.. image:: //bundles/redkitelabswebsite/media/bootbusiness/img27.jpg

Now you must add a new item, so right click the "Menu" node and click "Create" from the
contextual menu, rename the item just added as "News" and add the last Events item.

The works page
~~~~~~~~~~~~~~

Navigate to works page. This page contains the company's works and in the original design
each work is represented by an image.

I think a thumbnail is more appropriate to better represent a work, so I use this block 
instead of images. 

.. image:: //bundles/redkitelabswebsite/media/bootbusiness/img29.jpg

Change the "Page title" in "Our works" ad main title and  "the portfolio" ad subtitle,
then remove the block in the middle of the page.

.. image:: //bundles/redkitelabswebsite/media/bootbusiness/img30.jpg

Add a new "Thumbnail list" block.

.. image:: //bundles/redkitelabswebsite/media/bootbusiness/img31.jpg

Add now two thumbnails in this block, then add another "Thumbnail list" block for other works.

The partnership page
~~~~~~~~~~~~~~~~~~~~

Now open the partnership page. This page shows the company's partners. Each partner 
is identified by an image with a long description. The block used is the Text block, 
so feel free to play with this content type.

The leadership page
~~~~~~~~~~~~~~~~~~~

Now open the leadership page. This page shows the company's team members. Each member
has a picture and a long description that describes the team member.

To represent a member there is a dedicated block, so remove the default content
and add a new "Bootbusiness Member". Feel free to play with this Block.

The news page
~~~~~~~~~~~~~

The news page works exactly the same as the partnership page. 

The events page
~~~~~~~~~~~~~~~

Open the events page. Here is a listing of the company's events. 

.. image:: //bundles/redkitelabswebsite/media/bootbusiness/img34.jpg

To represent each event there is a dedicated block, the "Bootbusiness Event", so remove 
the default content and add a new Event block.

It is represent by a circled date, you can easily customize this with the Text editor and
a long description with a link, and it is always editable with the text editor.

Now add two more pages and always check the "Published" checkbox:

    - Page name: faq - Template: empty
    - Page name: contacts - Template: contacts

and link them in the top toolbar, adding two Link blocks.

The faq page
~~~~~~~~~~~~

.. image:: //bundles/redkitelabswebsite/media/bootbusiness/img35.jpg

Open the faq page. This page shows a frequently questions list, which is managed by
an Accordion block, so remove the main content and add a new Accordion.

.. image:: //bundles/redkitelabswebsite/media/bootbusiness/img36.jpg

This block is a list, so it is managed exactly like the main toolbar's links, while each
accordion item is managed by a Text block.

The contacts page
~~~~~~~~~~~~~~~~~

Open now the contacts page. This page shows a form on the left to allow the user
to send a quick message to the company, and lists on the right the contacts for each 
office around the world.

To manage the form you need to develop it as a normal Symfony2 form, then read `this tutorial`_
where there is an explanation of how to change content at runtime, to display it on the page

Offices are managed with the dedicated Bootbusiness Contact Office block. The contacts
template adds an office by default, so feel free to add a new office and to customize 
the contacts on your own. 

.. class:: fork-and-edit

Found a typo ? Something is wrong in this documentation ? `Just fork and edit it !`_

.. _`Just fork and edit it !`: https://github.com/redkite-labs/redkitecms-docs
.. _`this tutorial`: http://redkite-labs.com/how-to-change-a-content-at-runtime















