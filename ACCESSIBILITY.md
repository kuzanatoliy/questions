# Accessibility

<details>
  <summary>What is accessibility?</summary>

Accessibility is the practice of making your websites usable by as many people as possible. We traditionally think of this as being about people with disabilities, but the practice of making sites accessible also benefits other groups such as those using mobile devices, or those with slow network connections.

</details>

<details>
  <summary>What disabilities types?</summary>

- Visual;
- Auditory (Hearing impairments);
- Speech;
- Motor/Physical;
- Cognitive.

</details>

<details>
  <summary>What tips might help to make website accessible for the people with visually impaired?</summary>

- Provide sufficient contrast using colors and textures;
- Limit and prioritize color in the interface;
- Allow manual font size adjustment;
- Grant keyboard accessibility;
- Use explicit and descriptive labels for links and buttons;
- Provide alt text or descriptions for non-text content;
- Use headings to organize page content;
- Use descriptive titles for every page.

</details>

<details>
  <summary>What tips might help to make website accessible for the people with auditory impaired?</summary>

- video player-supporting mechanisms that enable subtitles and transcripts;
- audio player-supporting mechanisms that enable transcripts;
- multiple contact options (Don’t just provide a phone number on your website, as deaf people cannot hear well on the phone. Add communication channels like email, skype, live web chat, or online forms).

</details>

<details>
  <summary>What tips might help to make website accessible for the people with motor impaired?</summary>

- All functions are accessible and easy to use via the keyboard;
- The TAB order must be logically displayed on the Webpage or Web application;
- Appropriate labels for controls are included.

</details>

<details>
  <summary>What tips might help to make website accessible for the people with cognitive impaired?</summary>

- Avoid clutter; include sufficient white space;
- Use high contrast between text and background;
- Avoid too many choices, or too much information on one screen;
- Avoid lengthy scrolling; provide links to additional content;
- Identify where on the site the user currently is.

</details>

<details>
  <summary>What conformance levels are contained into WCAG(The Web Content Accessibility Guidelines) standard?</summary>

- WCAG Level A – Basic accessibility: Level A focuses on the basic accessibility needs of a wide range of users, and achieving conformance at this level is essential.
- WCAG Level AA – Strong accessibility: Level AA is the most commonly required level of accessibility compliance in accessibility legislation, and it is also the recommended level to aim for.
- WCAG Level AAA – Excellent accessibility: Level AAA is the highest possible conformance level and the most difficult level to attain in WCAG.

</details>

<details>
  <summary>What are regions?</summary>

Most pages have a visual structure with a block of content (typically logo, navigation, search, etc.) at the top, a main content area, a footer, and sometimes sidebars with related information. Page regions such as <header>, <nav>, <main>, <aside>, and <footer> programmatically define the essential semantic structure of a page.

</details>

<details>
  <summary>What are landmarks?</summary>

Landmarks is a powerful way to identify the organization and structure of a web page. Screen readers exploit landmark roles to provide keyboard navigation to important sections of a page. Landmark regions can also be used as targets for "skip links" and by browser extensions to enhanced keyboard navigation.

</details>

<details>
  <summary>How to controll a focus order or a navigation order?</summary>

The focus order begins with elements that have a positive tabindex attribute (if there are any) and moves from the smallest positive number to the largest (such as 1, 2, 3). It then proceeds through elements with a tabindex of zero according to their order in the DOM. Any elements with a negative tabindex are removed from the natural focus order.

</details>

<details>
  <summary>What advantages for using label tag?</summary>

- The label text is visually and programmatically associated with its corresponding form control. This means that a screen reader will read out the label when the user is focused on the form input, making it easier for an assistive technology user to understand what data should be entered.
- When a user clicks or touches/taps a label, the browser passes the focus to its associated input. That increased hit area for focusing is advantageous to anyone trying to activate it — including those using a touch-screen device.

</details>

<details>
  <summary>What is non-aria labels and names?</summary>

In order to make a website accessible to all users, it's important to use descriptive and meaningful text labels and names for all elements on the page. This helps to ensure that assistive technologies can accurately convey information about the page's content and structure to users with disabilities, making it easier for them to understand and interact with the website.

</details>

<details>
  <summary>What techniques would be used if the user inputs invalid data on a form field?</summary>

- when the user exits the field, an alert dialog can appear to describe the error so the user can fix it.
- after the user submits the form, the server returns the form, with the user's data still present, and indicates clearly in text at the top of the page that there were input errors. The text describes the nature of the error(s) and clearly indicates which field had the problem so the user can easily navigate to it to fix the problem.
- when the user attempts to submit the form, client side scripting detects the error, cancels the submission, and modifies the document to provide a text description after the submit button describing the error, with links to the field(s) with the error. The script also modifies the labels of the fields with the problems to highlight them.

</details>

<details>
  <summary>Why text alternative for non-text content is beneficial?</summary>

- it helps people who have difficulty perceiving visual content. Assistive technology can read text aloud, present it visually, or convert it to braille;
- it may help some people who have difficulty understanding the meaning of photographs, drawings, and other images, graphs, charts, animations, etc;
- it helps people who are deaf, are hard of hearing, or who are having trouble understanding audio information for any reason;
- people who are deaf-blind can read the text in braille.

</details>
