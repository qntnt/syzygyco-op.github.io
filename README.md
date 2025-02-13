# syzygyco-op.github.io

A simple public website for Syzygy

## How do I edit this site?

1. Get familiar with [the basics of GitHub](https://guides.github.com/activities/hello-world/) and [GitHub Pages](https://pages.github.com/).
1. Create a GitHub account if you don't have one already.
1. Ask to join the syzygyco-op organization on GitHub.
1. From here, you can either clone this repository to your local machine or edit it directly in the GitHub web interface.
1. Don't commit directly to `main`. Instead, create a new branch for your changes. Unless you're just editing this README or really know what you're doing ;)
1. Make your changes and commit them to your branch.
1. Open a pull request to merge your changes into the `main` branch.
1. GitHub will automatically create a preview of the proposed changes (look for a comment from "github-actions" with a link like <https://syzygyco-op.github.io/pr-preview/pr-sth>). It will take a few minutes after the pull request is created for this to become available. Good idea feary 🧚: [Check how it looks on mobile devices and various screen sizes](https://developer.chrome.com/docs/devtools/device-mode/).
1. Once you're sure your finished, merge your branch into the `main` branch.
1. Your changes will be automatically deployed to the live site in a few minutes.

## Help!

Feel free to ask for help the #website channel on Discord.

It may be helpful to know that most web browsers offer you the ability to inspect the HTML elements of a page (and a lot of other handy diagnostic tools). If you're having difficulty with the code itself, this can be like having super powers. There's no harm that can be done by poking around in there. Any changes you make are only made to your own copy of the web page, and will be discarded, e.g. when you close the web browser or refresh the page.

https://github.com/user-attachments/assets/93bbe61b-dd36-4db7-941f-7e1972d64d9e

For anyone who's interested, the [Mozilla Developer Network](https://developer.mozilla.org/en-US/) is a great authoritative source for educational materials on web development. On the other hand, you don't necessarily need to know very much to competently edit HTML. [The section on HTML below](/#a-bit-of-html) might help. 

## Philosophy

### Technological primitivism.

Keep it as simple as possible, but not simpler. Use the simplest tools, code, that meet our needs.

Note that having multiple HTML files may create the need for intra-site navigation, which may drive technical complexity. All we really need is a landing page that prominently displays the information we most want visitors to see above the fold, at a glance. One this page, we can link to or embed other websites that represent more detailed information about specific domains, and which may offer no-code solutions for creating and maintaining them. For example:
- Embed our public Google calendar to show an up-to-date view of our upcoming events.
- Link to our Discord server so people can chat with us.
- Link to pages in our Notion workspace to showcase our projects.

We can head off the need for multiple HTML files by having multiple sections with menu links implemented [by linking to fragments within the landing page](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/a#href), as long as we're mindful about page load times.

### Break the mold.

If we're going to have a website where we have full control over the HTML, CSS, and JavaScript, we might as well take advantage of the expressive potential that offers us. For example, despite the note about multiple pages above,
we could, in addition to the landing page, create a point-and-click skueomorphic multimedia experience that offers a whimsical alternative to the straight-laced landing page.

Let the website be a canvas for our creativity. Use the website to showcase our work, values, culture and community.

## A bit of HTML

```html
<!-- I am an HTML comment. I have no effect on anything except you, dear reader. Or so I hope. -->

<h1 id="the-header">I am an H1 (level 1 header) element.</h1>
<!--
  Replace the 1 in "h1" with any number between 2-6 to create a smaller, lower-level header.
  Note that there is an opening and closing tag with the same name inside, that is, "h1".

  Note that this H1 element has an "id" attribute.
-->

<a href="example.com">I am a link to another website (example.com)</a>

<!--
  Click the link below and the page will scroll if necessary to show the above header.
  This is because a link is established via the "href" and "id" attributes. Note the
  pound sign (#) in the href attribute. 
-->
<a href="#the-header">I am a link to the header above.</a>

<!--
  Below is an embedded image. A very cute one, judging by my 'src' attribute!
  Note that there's no closing img tag (</img>)!
-->
<img
  src="cats.gif"
  alt="This text will be shown while that image is loading, read by screen readers, and shown in a tooltip."
>

<div>
  I am a generic container for text and <b>any other elements</b>!
  I'm useful for grouping things together and creating structure.
</div>
```
