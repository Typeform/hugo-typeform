# Typeform for Hugo static sites

A few partials to integrate [Typeform.com](http://typeform.com) into your [Hugo](https://gohugo.io) static sites.

One big advantage over other options is that you don't have to expose your email address in your site config. Plus, you can use [Integrations](https://www.typeform.com/help/connect-typeform-to-your-favorite-tools/) with Typeform to route the form data to a ton of different places, like Google Docs, Mailchimp, Trello or Evernote.

## Setup

Follow these steps to add a Typeform to your site.

First, copy `layouts/partials/typeform.html` to your Hugo site directory, in the same strucure.
```
cp layouts/partials/typeform.html ../my-hugo-site/layouts/partials/
```

A Typeform page is just like a regular Hugo page. But it must include the field `id` with the value `typeform`.

```toml
+++
title = "Contact"
id = "typeform"
+++
```

To enable the form in your page, just add your form ID and user name (optionally) in the `config.toml` file. In addition, you can optionally configure the height/width.

```toml
[params]
typeformid = "u6nTL7" # Required
typeformuser = "myuser" # Optional
typeformwidth = "100%" # Optional
typeformheight = "800px" # Optional
 ```
