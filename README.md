# README #

This repository contains the Open Event Data Model website. It is a Jekyll powered static site.

## Structure ##

In order to maximize content separation from system diles the content has been arranges as follows:

- root
    - _entities (content: schema entities pages)
    - _includes (system folder)
    - _layouts (system folder)
    - _posts (content: blog posts)
    - css (system folder)
    - fonts (system folder)
    - images (content: image assets)
    - js (system folder)
    - news (content: news/blog index page)
    
In order to update the content, only the folders labelled as *content* should be updated.
Each folder contains a different type of content with specific navigation patterns.

## Features ##

The following features and capabilities are included in this site:

- Clean content separation from system folders
- Responsive theme based on Bootstrap
- Lean navigation, optimized for mobile devices: single level main menu and breadcrumbs
- Dedicated layouts per content type: entity, news, page and post
- Dedicated Terms and Conditions page
- Dedicated styling helper page (it is recommended to disable this one on production)
- Navigation menu fixed to the top of the browser window and collapsed to a hamburger icon in small devices
- Blog pagination
- Blog navigation: previous, next

## Content included in initial release ##

At the moment of the site development not all information was available to create the site. That is why some dummy content and placeholders have been created.

### Home ###
- Location: `/index.html`
- Website path: /

The home page is filled in with the content provided. It has three sections.
The news are inserted dynamically (refer to the [News](#News) section to find out about the blog posts.

### Schema ###
- Location: `/_pages/schema.md`
- Website path: /schema/

This page was created as specified in the [OEDM Site content][gdoc] and [Wireframe][wire] documents, with the exception of adding to it the list of available entities. This reduces the navigation depth in one level.

#### Entities ####
- Location: `/_entities/*.md`
- Website path: /schema/:entity/

Entities are a Jekyll collection. This allows them to be grouped in a dedicated folder and to have a dedicated template to display them. Each one of the available entities is a different file. Keep in mind that the entity page *Person/Group/Organisation* was split in two separate entities: *Person* and *Organisation*.

All entity JSON examples are dummy placeholder content, copied from the *Event* entity. These must be updated for the entity pages to be correct.

### Applications ###
- Location: `/_pages/applications.md`
- Website path: /apps/

Originally the [documentation][gdoc] and the [wireframes][wire] provided required multipl pages for the *Projects* section. As there is very little information at this point of time it was chosen to leave all the existing applications of the OEDM in a single page. Until more applications are added this is a conveninent way  to keep the site simple.

All content provided in this page is dummy and must be updated.

### Documentation ###
- Location: `/_pages/documentation.md`
- Website path: /docs/

The data provided in the [OEDM Site content document][gdoc] was very limited. That is why many sections have been added to it as placeholders for the corresponding documentation pages. These placeholders include:

- OEDM explained
- OEDM presentation pack
- OEDM technical documents
- Getting Started: A simple introduction to OEDM and how to use it for marking up your site.
- Releases: Full history of recent releases. --> This may link to Github.
- Frequently asked questions
- OEDM Blog --> linked to the *News* section.
- Feedback form: Please give us feedback, report bugs, etc. --> If a feedback form is to be included the corresponding form processing service must be added to the site.
- Terms and conditions --> Linked to the *T&Cs* page.
- Styles --> Linked to the *Styles* page.

#### Terms and conditions ####
- Location: `/_pages/terms.md`
- Website path: /docs/terms/

Added page to hold the legal terms and conditions. All content is dummy, with four placeholder sections to serve as a starting point to write it.

#### Styles ####
- Location: `/_pages/styles.md`
- Website path: /docs/styles/

Added page to provide a style guide and a markdown help for editors.
It is recommended to remove the page from the production site.

### News ###
- Location: `/news/index.html`
- Website path: /news/

This is the blog feature of the website. It has been renamed *News* as it will be sued to add updates to the site.
It includes a pagination widget. The posts displayed in each of the pages include the title, the date and the content extract.

All posts included are dummy. Multiple posts were added to demonstrate the pagination behaviour.

#### Posts ####
- Location: `/_posts/*.md`
- Website path: /:yyyy/:mm/:dd/:post.title/

Independent page display for each post. They behave in the same way that the rest of the pages but have a very different path designed to optimize the retrieval and organization of the posts chronologically.

Previous/Next navigation was added, as supplementary to the Breadcrumbs.

All the posts included in the initial release are dummy content and must be replaced with real ones.

### About ###
- Location: `/_pages/about.md`
- Website path: /about/

There was no data in the [OEDM Site content document][gdoc] regarding this section, but it was included in the [Wireframe document][wire]; therefore it was included with dummy content, including the sections outlined in the wireframe.

### Footer (system component) ###
- Location: `/_includes/footer.html`
- Website path: -

The footer has two rows of data, the first one with three columns containing the details of Southbank Centre and Barbican, and the three latest news headlines. The second row has a *Last updated* tag, to identify the exact version of the site published online. All the blocks stack gracefully in responsive mode.

The images included for the contact details logos are stored in `images` folder and should be replaced with ones with a transparent background.

The footer holds two links to the T&Cs page and the style guide and markdown examples page. It is recommended to remove the link to the Styles page in production as it is intended to be just a visual guide for editors.

Any changes to those elements must be done in this file.

[gdoc]: https://docs.google.com/document/d/1V28efLVDtJYG9b5i6b9agBL5F8Aihd0uCxxyVE-kRWo/edit#heading=h.2s1dycp87si
[wire]: https://drive.google.com/file/d/0BygJF_yBftCGMkE1cUxKT1pBcE0/view?usp=sharing