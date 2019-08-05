# Matter of Heart Psychotherapy



*Code Institute: User Centric Frontend Development - Milestone Project*



**[Live link to deployed project](https://loosenthedark.github.io/UCFD-milestone-project/)** (hosted on GitHub Pages)



---



**Matter of Heart Psychotherapy** is the name of a recently-established therapy practice based in Dublin.

As it is still in its infancy, the business lacks any sort of tangible online presence - something that is essential nowadays towards gaining a foothold within the industry and establishing a client base. I therefore set out to build a clearly laid out webpage with two overarching objectives.

Firstly, the site should serve as a 'shop window' of sorts for the therapist, allowing him to document his educational background, relevant qualifications and professional experience, as well as outlining his approach towards treating clients.

The second fundamental aim was to provide prospective clients with an easy-to-use, concise and visually appealing portal of information, featuring digestible resources and summaries pertaining to both the broad profession of psychotherapy itself and the more specific details of what it is Matter of Heart Psychotherapy can do for them.

## UX

In consultation with the site owner during the project's planning stages, he told me how he wanted me to design "something that stood out from the typical generic appearance of most psychotherapy sites with their soft pastel colours and Buddha and waterfall images". He also mentioned a preference for incorporating a vaguely art deco aesthetic if possible. These considerations collectively informed my choice of colours, fonts, images etc. to build a website with a distinctive feel and coherent structure.

As with any website, a number of user needs existed prior to construction. These needs are best summarised in the following three core User Stories:

1. _"As site owner, I need a welcoming, informative and user-friendly webpage where I can showcase my therapy practice by providing details about my background, qualifications and therapeutic approach. I would also like a means of pre-emptively answering a range of common queries that prospective clients are likely to have. My desired outcome will be an increase in my client base and overall growth of the company profile."_
2. _"As someone who knows a bit about psychotherapy and/or has availed of therapy before, I am looking to find out more about Matter of Heart Psychotherapy with a view towards potentially booking an appointment. In addition, I would like to be able to follow this practice on social media. My browsing time is very limited, and I generally access the web on my iPhone."_
3. _"As someone who knows little or nothing about psychotherapy, I would like to learn about what is involved in order to decide whether it is something I wish to avail of. I would also like the option of maybe booking an appointment if I am suitably motivated to do so. Ordinarily I use my work laptop for online research, but I have also recently bought a tablet."_

These three overlapping requirements dictated how I set about designing the site's layout. Adopting a mobile-first approach, I strived to maintain a flexible balance between providing too little and too much information - keeping in mind screen size limitations on smaller devices as well as competing end user needs. Measured use of Bootstrap components like an `.accordion` and `.carousel` made factoring in and meeting these needs more manageable, while I was also able to take advantage of Bootstrap's default display classes to make content visible or hidden as appropriate.

 
## Features

### Existing Features

+ The Bootstrap JavaScript Scrollspy plugin was enabled via `data-*` attributes in order to bring some colour and life to the `.navbar`, as well as to engender a sense of progress and flow as users navigate between the various page `section`s. Guidance on how to do this was obtained from the following W3Schools [reference](https://www.w3schools.com/bootstrap/bootstrap_ref_js_scrollspy.asp) and [tutorial](https://www.w3schools.com/bootstrap/bootstrap_scrollspy.asp).
+ In order to create a smooth scrolling effect as users navigate between anchor links on the site, I firstly read up on [optional means of enabling this](https://stackoverflow.com/questions/7717527/smooth-scrolling-when-clicking-an-anchor-link). I subsequently decided against using pure CSS due to cross-browser compatibility concerns, and instead followed the advice of [Traversy Media's YouTube tutorial](https://www.youtube.com/watch?v=y9nlfqT4s9s) in order to enable it using jQuery (see local `index.js` file for further details).
+ A fixed-position responsive `.navbar` (collapsed on extra-small and small devices; visible on landscape phones and all larger screen sizes) ensures simple, fluid movement and safeguards against users getting 'lost' anywhere within the site.
+ Several built-in Bootstrap components and JavaScript plugins were utilised to achieve certain design goals:
  + The Collapse JS plugin was used to create a functioning [`.navbar toggler icon` (aka 'hamburger icon')](https://getbootstrap.com/docs/4.0/components/navbar/#toggler) in the top right-hand corner of the screen on smaller devices. Additional styling of this icon (primarily applying a colour change to its `span` elements to ensure consistency with the site's overall colour scheme) was facilitated by this [Stack Overflow thread](https://stackoverflow.com/questions/42586729/bootstrap-4-change-hamburger-toggler-color), and in particular its [linked code demo](https://www.codeply.com/go/4FdZGlPMNV).
  + On smaller devices an [`.accordion`](https://getbootstrap.com/docs/4.0/components/collapse/#accordion-example) was created, again using Bootstrap's Collapse JS plugin, to organise and condense the information contained in the FAQ `section`. An extension of default `.collapse` behaviour using the `.card` component was necessary here.
  + On larger devices, a similar need was met via Bootstrap's [`.carousel`](https://getbootstrap.com/docs/4.0/components/carousel/) slideshow component, which again uses a mix of JavaScript and CSS 3D transforms to present relevant details to the user in a manner that is easy to digest and make sense of.
+ Bespoke background `:hover` effects were added behind the `iframe` media elements within the FAQ `section` to produce a subtle visual differentiation between embedded video and audio links. A similar, albeit more dynamic, effect was achieved in the text boxes throughout the Blog `section`: the custom 'sweep-to-left' and 'sweep-to-right' classes produce a sleek and symmetrical look that is pleasing to the eye. All of this was made possible thanks to [Ian Lunn's convenient collection of transitions](http://ianlunn.github.io/Hover/).
+ A complication involving an obscured/cropped `border` surrounding the Contact `form` at the bottom of the page was resolved by following the advice of [this Stack Overflow solution](https://stackoverflow.com/questions/6312067/border-radius-background-color-cropped-border).

### Features Left to Implement



## Technologies Used

1. HTML (HTML5)
2. CSS (CSS3)
3. [Bootstrap (v4.3.1)](https://getbootstrap.com/)
4. [jQuery (v3.3.1)](https://jquery.com/)
5. [Google Fonts](https://fonts.google.com/)
6. [Font Awesome](https://fontawesome.com/)
7. Hover.css: [site](http://ianlunn.github.io/Hover/) | [repo](https://github.com/IanLunn/Hover)
8. [Popper.js](https://popper.js.org/)

## Testing


All testing was performed manually, and on a near-constant basis as the project evolved. [Google Chrome DevTools](https://developers.google.com/web/tools/chrome-devtools/?utm_source=dcc&utm_medium=redirect&utm_campaign=2018Q2) served as the foundation for this testing process, while ongoing testing of the site's responsiveness was conducted using [Responsinator](https://www.responsinator.com/).

Additionally, the site was tested in a variety of browsers (Chrome, Safari, Firefox, Amazon Silk) across several devices and screen sizes (Samsung Galaxy S5, Huawei P20 Pro, MacBook Pro, iPad, Kindle Fire) to ensure compatibility.

In terms of addressing the goals outlined above in the core User Stories, the following can all be said to have been rigorously tested and verified throughout the design process:

1. _"As site owner, the landing page boasts eye-catching `header` branding, as well as a motivating synopsis of why the user should choose to enlist my services. There is a prominent call-to-action `button` along with a secondary 'Read More' prompt encouraging the user to explore the site further. My academic and professional background, together with a bitesized account of my integrative approach, can all be viewed in the About Me `section`, which also features a professional-looking photo of me. Again, there is a well-positioned call-to-action `button`, should the user wish to book an appointment right away. Still-undecided users can navigate further to the FAQ `section`, where they can view a host of detailed and relevant answers to some of the questions they may have in relation to the practice. There are also a couple of explainer media links for those who wish to avail of additional resources. Towards the bottom of the site, a well-organised Contact `form` makes both getting in touch and booking an appointment quick and uncomplicated, while a supplementary Blog `section` and social media links enable me to consolidate my web presence and increase client retention rates."_
2. _"Having undergone therapy several years ago, I had heard about Matter of Heart through word-of-mouth and was keen to learn more about the practice. I found the site easy to navigate and visually appealing. The `.accordion` layout of the FAQ `section` conveniently allowed me to skip the basic general queries about psychotherapy as a whole and focus instead on the more specific questions I had about this business. As an active social media user, I immediately decided to follow Matter of Heart on both Facebook and Twitter, as I rely on notifications from these channels to stay up-to-date. Although I haven't yet booked my first appointment, I will probably do so in the coming days, as I could see that the booking process is smooth and straightforward."_
3. _"This being my first visit to a psychotherapy website, I was pleasantly surprised by the array of reassuring and instructive content available. The FAQ `.carousel` contained a lot of detail presented in a compact manner. Likewise, the About Me `section` reassured me about the therapist's credentials and made me consider booking an introductory session. The following day, when I had more time available, I returned to the site to watch the video explaining 'How Psychotherapy Works', and that was enough to convince me to book an appointment."_


## Deployment

[GitHub Pages](https://pages.github.com/) was the hosting service chosen for website deployment. The site repository's `master` branch was selected as the publishing source by following the steps detailed in [this GH Help article](https://help.github.com/en/articles/configuring-a-publishing-source-for-github-pages). All new `commit`s made from the `master` branch will therefore automatically update the site.


In order to run this project locally, you can clone [the remote GH repository](https://github.com/loosenthedark/UCFD-milestone-project) for use and modification within your own local environment. This can be done quite easily by first of all changing the current working directory in your Terminal to the location where you want the cloned directory to be made. Once this is done, simply type `git clone` and then paste `https://github.com/loosenthedark/UCFD-milestone-project.git` into the command line. A more thorough explanation of all the steps involved in this cloning process can be found [here](https://help.github.com/en/articles/cloning-a-repository).

## Credits

### Content

All text featured across the Landing (Home), About Me and FAQ `section`s was provided by the site owner, with some minor edits made by me during construction. The text featured in the blurbs throughout the Blog `section` is copied from the introductions to corresponding Wikipedia articles - each of which is linked to via its respective 'Read More' button.

### Media

The profile image of the site owner was provided by him directly - some vertical cropping was later applied by me. The two logo images positioned below this lead image were sourced from the corresponding organisations' websites, namely [Irish Association for Counselling and Psychotherapy](https://www.iacp.ie/) ([image link](https://www.iacp.ie/images/logo.png)) and [Dublin Business School](https://www.dbs.ie/) ([image link](https://www.dbs.ie/images/default-source/logos/dbs-logo-2019-small.png)).
All other images used, namely the background images in the Landing and Contact `section`s and the box divider images in the Blog `section`, were taken from [Pexels](https://www.pexels.com/), a free-to-use library of high-quality stock photos.


The two embedded media files featured in the FAQ `section` on larger devices were taken, respectively, from [YouTube](https://www.youtube.com/watch?v=g-i6QMvIAA0) (video) and [SoundCloud](https://soundcloud.com/user-685330905/what-is-psychotherapy) (audio), and are both linked to clearly and appropriately.


Font Awesome Icons were inserted alongside the media files in the FAQ `section` and across the top of the Contact `form` on larger devices, as well as in the text boxes throughout the Blog `section` and along the `footer`.


The `shortcut icon` (favicon) displayed in the website's tab was supplied with permission by [Gregor Cresnar](https://www.flaticon.com/authors/gregor-cresnar) of [Flaticon](https://www.flaticon.com/).


Finally, credit is due to Code Institute UCFD student lead Anthony O'Brien for suggesting [TinyJPG](https://tinyjpg.com/) as an indispensable resource for compressing image files prior to upload in order to speed up site load time. This process was applied to almost all images used in this project.


### Acknowledgements

Thanks to my mentor Antonio for his timely feedback, encouragement and recommendations throughout this project. Anto pointed me towards [WrapBootstrap](https://wrapbootstrap.com/) for browsing a wide selection of Bootstrap templates and themes, which provided plenty of inspiration. He also suggested I use Responsinator for testing the site's responsive design throughout the construction process, and this proved to be an invaluable tool.


Other excellent pieces of advice came via @Anna_G and @Eventyret_mentor (among others) in Code Institute's Slack room. Thanks, guys!
