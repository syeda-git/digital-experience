# Topics Latest List

Displays a list of the most recent topics, based on content items created by using the Topics content template.


# Usage

This portlet can be used anywhere on your site to display a list of the most recent topics.

# Adding the portlet to a page

1.  Go to the page where you want to add a Topics Latest portlet.

2.  Click **Edit Mode**.

3.  Click **Create** \> **Content** \> **Lists**.

4.  Drag the **Topics Latest List** to the page and save the page.


# Creating content to display in the portlet

1.  To access the authoring portlet, go to **Applications \> Content**.

2.  Create a content item by using the **Topics** content template.

3.  Publish the item.


# Content author customization options

## Portlet configuration options

By clicking **Open Edit Form** from the portlet menu the content author can edit the list title.

# Site designer customization options

With the portal in edit mode, sight designers can make the same customization changes as content authors and more. Additionally, site designers can copy and change the building blocks of each portlet.

## List component

East list portlet uses a component to define what content items are displayed in the portlet. The Topics Latest portlet uses the following portlet:

-   CTC Design/List Components/Landing Latest Items by Publish Date

If you need to customize this component, you must create a copy and save it into your own design library. By clicking **Open Edit Form** from the portlet menu, you then select the new component in the List component parameter of the portlet configuration document.

You can also select a different list component to use from the CTC Design library. These components are located under: CTC Design/List Components/

## List presentation

East list portlet uses a list presentation to define the design of the body, header, and footer of the items that are returned by the selected list component. The Topics Latest portlet uses the following list presentation

-   CTC Design/List Presentation Components / Landing Combination List Design with Publish Date

If you need to customize this component, you must create a copy and save it into your own design library. By clicking **Open Edit Form** from the portlet menu, you then select the new component in the List component parameter of the portlet configuration document.

You can also select a different list presentation to use from the CTC Design library. These components are located under: CTC Design/List Presentation Components/

## CSS Style

The default stylesheet that is used by this portlet is **contentComboList**. To customize this CSS file, first make a copy of the CSS file, edit the copy, and then enter the name of the new CSS file in the CSS Style parameter in the portlet configuration document.

CSS files are stored in this WebDAV folder: dav://server:port/wps/mycontenthandler/dav/fs-type1/themes/Portal8.5/CTC/css.

## List Templates

The authoring templates that are selected in the List Templates section of the portlet configuration document determine what items are returned by the Landing Latest Items by Publish Date component. The default template that is used by this portlet configuration is CTC Design/Topics. If you have created a customized copy of this template, you must specify so that your topics content items are displayed.

