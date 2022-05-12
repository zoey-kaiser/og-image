# Open Source OG-Image Generator

The `og-image` generator, is a [kubernetes](https://kubernetes.io/) based node application, that allows developers, to easily and quickly generate their own og images. It is inspiered by [`vercel/og-image`](https://github.com/vercel/og-image), which is a simular tool, however it runs over a nextjs middleware, rather then a scaleable cluster. 

This project is supported by [SideStream](https://www.sidestream.tech/) and was planned to help me better understand nodeJS applications and setting up my own scaleable kubernetes cluster.

## What is an OG-Image?

When optimising your website for search engines and social media sites, developers use [The Open Graph protocol](https://ogp.me/). This protocol is a universally adopted method of conveying, meta data about your site to search engines and social media sites.  

OG-Image refers to the method of including link previews for your site. This generally increases the chance that users will click on your link, as it appears more polished and makes the link more noticeable. 

Simplified there are two methods of including OG-Images. Static images, will always look the same and are not linked to the state of the website. On the other hand, generated images take the state of the website into account, therefore looking different once the data changes. 

A prime example of this would be a blog. You could either display the same image for every blog post, or you could generate custom images with the blog title, content or more information. 

The application, streamlines the development of such images, by providing a template system, that can be modified to create new images. By default there are a handful of pre made templates, that users can already use. These take in specific data and display it inside the image.

## Usage

There are two methods of using the OG-Image generator. Once the first version releases, there will be a public version, you can use by including our link and providing the data via arguments. 
Alternatively, developers can start the cluster on their own systems, allowing them to make custom templates and more. However this requires a bit of technological knowledge.  

In order to add a open graph image to your page add the following code to your document head:

```html
<head>
  <title>Title</title>
  <meta property="og:image" content="http://example.com/logo.jpg" />
</head>
```

## Setup
```bash
# install dependencies
$ npm install

# serve with hot reload at localhost:3000
$ npm run dev

# build for production and launch server
$ npm run build
$ npm run start

# generate static project
$ npm run generate

# for component development
$ npm run storybook

# to run jest tests
$ npm run test
```
