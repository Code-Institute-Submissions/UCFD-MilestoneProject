# User Centric Frontend Development Milestone Project

### The aim of this website is to introduce a popular Japanese pop rock duo Garnidelia to Western audiences.
## The site will include the following features:

- Landing page
- About page: includes the brief profile and biography of the duo
- Discography page: contains a shortlist of the duo's discography which also serves as a internal link to a
corresponding music video (embedded) if available.
- News page: provides users with the duo's latest news such as live event and new album releases.
- A contact form where visitors can use to send feedbacks of the website or contact host of the website directly on more specific issues.

Bootstrap will be used as a starting point for responsive design and CSS styling but adjustments will be made in order to achieve a more appealing result.

## Features in depth:

#### Navigation Bar
- Based on bootstrap's navbar, this particular navigation bar will function differently on different screen size:
  - Dropdown menu on smaller screens.
  - Horizontal navigation bar with additional social links to Facebook, YouTube and Twitter on the right hand side when viewed on larger screens.

#### Landing page
- A simple landing page with a photo of the duo as the background and the duo's name in the middle of the page, in large fonts.
- Font size will change depending on screen size so it will be kept in ratio with other elements on the page regardless of screen size.

#### About
- Utilizing bootstrap's grid system, responsive design for about page are achieved as follows:
  - Single column on smaller devices with a photo of the duo on top, followed by the duo's profile underneath.
  - On larger devices, the photo will be moved to the side with a 1:1 ratio to the profile section, hence two equal width column.
- The duo's profile is presented in chronological order and grouped into several categories. This is achieved using bootstrap's accordion.

#### Discography
- Responsive design for discography page are achieved as follows:
  - Smaller devices:
    - Single column.
    - On each item there is a YouTube icon at the end which is a external link to the music video of the said item.
  - Larger devices:
    - Two columns with a rough 1:2 ratio.
    - The same list is used but instead of providing user with a external link, internal links are used. This is reflected by the icon changing from YouTube logo to a video camera.
    - The internal links are simple anchors to the corresponding embedded YouTube video of a particular song on the page.
    - Code for embedded YouTube video are taken directly from YouTube and combining with code from https://benmarshall.me/responsive-iframes/ the frame size of embedded video changes with respect to screen size.
    - As the embedded videos are all presented in a single list, large margin has been used so that only 1 video is shown at a time to avoid confusion.

#### News
- Using similar format from discography, responsive design for news page is achieved as follows:
  - Smaller devices:
    - Single column.
    - Each item is presented as a panel of accordion, similar to about page.
  - Larger devices:
    - Instead of using accordion the similar concept from discography is used so that heading of each news is displayed on the left while the main article is displayed on the right.
    - Headings of news also double as anchor to the main article.
    - However unlike discography a smaller and fixed margin is used to separate main articles. This is due to the fact that each article are different in length.
    - To compensate that alternate spacing has been used so that a selected article will always be displayed from the top of the page.

#### Contact
- A bootstrap form with no backend attached (which is outside of the scope of this project).
- Paddings on the side varies depending on screen size.

## Technologies Used
- [Bootstrap 3.3.7](https://getbootstrap.com/)
	- Toolkit for frontend styling. It provides a framework for most of the styling without having to reinvent the wheel.
- [Font Awesome](https://fontawesome.com/) is also used to for certain icons used in this project.

## Testing
Since this project revolves around user experience so it is more natural to test the website manually for better measurement of UX. Test results are documented in test-documents folder of this project but to summarise:
- Tests are mainly involves checking if links are working as expected and UX transition between large and small screens.

### Responsive design
As part of requirements, web pages in this project needs to have a responsive design; that is layout of pages will change depending on screen size in order to maintain a high level of UX. Using a mobile first approach, the base design uses a single column layout and expanded to a 2 columns with 1:2 ratio design on large screens. Furthermore the navigation bar is a collapsible menu on small screens and expand to a full bar which is fixed on top when displayed on large screens.

## Deployment
As this project only involves frontend-only web pages there is no need for a proper deployment as the html files can be used as is; provided users have access to web browser, internet connection, as well as a copy of the project's html files. Nevertheless, for users that does not have access to the html files of this project, the need to host this project will rise and one of the simpler solution would be to host this project to [GitHub Pages](https://pages.github.com/). Since this project uses GitHub for version control it would be very easy to host this project on GitHub Pages.

## Credits
- Biography of GARNiDELiA in this projects are referred from [Wikipedia](https://en.wikipedia.org/wiki/Garnidelia)
- Articles in this project originate from [HERE](https://www.jrocknews.com/tag/garnidelia)
- Videos used in this project comes from GARNiDELiA official YouTube channel and the respective uploader.

### Update Log
#### 18/04/2018
- Testing document added.

#### 15/04/2018
- Contact form has been implemented in full.

#### 05/04/2018
- News page has been implemented in full.

#### 31/03/2018
- Discography page has been implemented in full.

#### 25/03/2018
- Changing from a header/ footer design to a header-only design.
- Adept to a more simple design (No background image other than landing page)
- Fixed problem caused by background image's z-index.

#### 23/03/2018
- Landing page implemented in full.
- About page implemented in full.

#### 19/03/2018
- Landing page first implemented.

#### 14/03/2018
- Project begins.
- Rough mockup and README file.
