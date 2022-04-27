## App Architecture

### Markup

Layouts -> Templates -> Sections

_Layouts_
Layouts are the base of the theme, through which all templates are rendered.

_Templates_
Templates control what's rendered on each type of page in a theme.

_Sections_
Sections are reusable modules of content that can be customized by merchants.

_Snippets_

### Styles

With `node sass` installed globally run `npm run sass` to compile your styles. Main sass file is `_style.scss` which compiles to `style.css`. Any child stylesheets should be prefixed with `_`.

Styles that associated with layout, templates, sections or snippets should be prefixed with `_layout`, `_template`, `_section`, `snippet`.

### Creating New Pages

- In order to create custom pages you must first visit your online store.
  - Visit `{your-store}.myshopify.com/admin/pages/new` and create your new page
  - Visit `{your-store}.myshopify.com/admin/themes/{store-id}/editor` and select edit code from the dropdown
  - In the editor create your new section then the page
  - Visit `{your-store}.myshopify.com/admin/pages/{page-id}` and set the template

The _"Team"_ page is currently in the project directory as an example for local usage and needs to be constructed on the store admin.
