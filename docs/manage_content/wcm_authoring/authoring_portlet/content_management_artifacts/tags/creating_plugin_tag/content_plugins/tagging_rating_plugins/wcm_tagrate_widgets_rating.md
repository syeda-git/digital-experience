---
id: wcm_tagrate_widgets_rating
title: Adding a rating widget to web content
---




You can add a rating widget to a content item by adding a `[Plugin:ratings]` component to your presentation template. By default the plug-in component is rendered using the `HTML - Rating Widget Light` design, which is included in the web content library `Web Resources v70`, or you can create your own design.

!!! note
    When using tagging and rating with web content, ensure that synchronization of the tagging and rating scopes has been set up for the portal.

1.  To add a rating widget to a content item, include the rating plug-in in your presentation template.

    For example:

    ```
    <div id="ratings">[Plugin:ratings]</div>
    ```

    The rating plug-in supports the following parameters that are specified in a `key=value` format:

    -   **`design=path`**

        The `design` parameter indicates which design to use when rendering the rating widget. Specify the `path` information using the full library path to the HTML component that contains the design template for the rating widget. For example:

        ```
        [Plugin:ratings design="Web Content/folder/myRatingDesign"]
        ```

        If the `design` parameter is not specified, a default design is defined in the `HTML - Rating Widget Light` component, which is provided with `Web Resources v70` library that is included in the product. During rendering the system checks the following locations for the default design:

        1.  The current web content library
        2.  The web content library `Web Resources v70`
    -   **`actionScope=scope`**

        The `actionScope` parameter indicates the scope of tags that you want to show in this widget. For a list of possible values see the description of the `ratingScope` parameter used with the inline tag widget. For example:

        ```
        [Plugin:ratings actionScope="community"]
        ```

    **Stylesheet class note:** The presentation template that includes the widget must ensure that the `lotusui30` stylesheet class is assigned to the markup that contains the widget. You can specify this stylesheet class in the following ways:

    -   In the presentation template, enclose the widget within a <div\> element that references the class. For example, `<div class="lotusui30"> ... </div>`.
    -   Create a design for the widget that specifies the class, and reference the design from the `Plugin` tag with the `design` parameter.

