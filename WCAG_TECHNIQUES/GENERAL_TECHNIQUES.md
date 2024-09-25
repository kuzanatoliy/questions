# General techniques

<details>
  <summary>What abjective of adding a link at the top of each page that goes directly to the main content area?</summary>

The objective of this technique is to provide a mechanism to bypass blocks of material that are repeated on multiple Web pages by skipping directly to the main content of the Web page. The first interactive item in the Web page is a link to the beginning of the main content. Activating the link sets focus beyond the other content to the main content. This technique is most useful when a Web page has one main content area, rather than a set of content areas that are equally importatn, and when there are not multiple navigation sections on the page.

**Procedure:**

1. Check that a link is the first focusable control on the Web page.
2. Check that the description of the link communicates that it links to the main content.
3. Check that the link is either always visible or visible when it has keyboard focus.
4. Check that activating the link moves the focus to the main content.
5. Check that after activationg the link, the keyboard focus has moved to the main content.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G1)

</details>

<details>
  <summary>What abjective of allowing the content to be paused and restarted from where it was paused?</summary>

The objective of this technique is to provide a way to pause movement or scrolling of content. If the user needs to pause the movement, to reduce distraction or to have time to read it, they can do so, and then restart it as needed. This mechanism can be provided either through interactive controls that conform to WCAG or through keyboard shortcuts. If keyboard shortcuts are used, they are documented.

**Procedure:**

1. Use the mechanism provided in the Web page or by the user agent to pause the moving or scrolling content.
2. Check that the moving or scrolling has stopped and does not restart by itself.
3. Use the mechanism provided to restart the moving content.
4. Check that the movement or scrolling has resumed from the point where it was stopped.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G4)

</details>

<details>
  <summary>What abjective of allowing users to complete an activity without any time limit?</summary>

The objective of this technique is to provide users with all the time they need to complete an activity. This technique involves providing a speciafied activity which does not require timed interaction. Users are allowed as much time as they need to interact with the activity.

**Procedure:**

1. Determine if any timed interactions are present.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G5)

</details>

<details>
  <summary>What abjective of providing a movie with extended audio descriptions?</summary>

The objective of this technique is to provide a second version of video content that provides extended audion descriptions. One of the difficult things about creating traditional audio descriptions is that the narrotor somethimes has to provide a lot of information during very short pauses in dialogue. Extended audion description temporatily pauses the audion and video to allow critical information to be delivered when pauses in dialogue are insufficient for adequeate description.

**Procedure:**

1. Open the version of the movie that includes extended audio descriptions.
2. Check that the video halts for extended audio description when there is not enough space to include necessary narration between the natural dialogue.
3. Check that the necessary information is in the audio description.
4. If the alternate version(s) are on a separate page, check for the availability of link(s) to allow the user to get to the other versions.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G8)

</details>

<details>
  <summary>What abjective of creating captions for live synchronized media?</summary>

The objective of this technique is to allow users who cannot hear to be able to access real-time synchronized media broadcasts. It is more difficult to create accurate real-time captions because there is little time to correct mistakes or to listen a second time or consult someone to be sure the words are accurately reproduced. It is also harder to simplify or paraphrase information if is flowing too quickly.

**Procedure:**

1. Check that a procedure and policy are in place to ensure that captions are delivered in real-time.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G9)

</details>

<details>
  <summary>What abjective of creating components using a technology that supports the accessibility API features of the platforms on which the user agents will be run to expose the names and roles, allow user-settable properties to be directly set, and provide notification of changes?</summary>

The objective of this technique is to allow assistive technology to understand Web content so that it can convey equivalent information to the user through an alternate user interface.

**Procedure:**

1. Render content using an accessible User Agent.
2. Use an Accessibility Tool designed for the Accessibility API of the User agent to evaluate each user interface component.
3. Check that name and role for each user interface component is found by the tool.
4. Change the values on the component.
5. Check that the Accessibility tool is alerted.
6. Check that the component works with assistive technologies.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G10)

</details>

<details>
  <summary>What abjective of creating content that blinks for less than 5 seconds?</summary>

The objective of this technique is to minimize the distraction cuased by blinking content and enable users to re-focus on the other content on the page.

**Procedure:**

1. Find all items that blink.
2. For each item that blinks, determine if the interval between the start and end of the blinking is less than five seconds.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G11)

</details>

<details>
  <summary>What abjective of describing what will happen before a change to a form control that causes a change of context to occur is made?</summary>

The objective of this technique is to provide infromtation to users about what will happen when a chage to a form control results in a change of context. Because changing the value of a form control does not typically result in a change of context it is important that authors provide instructions that make the user aware of the behavior in advance. where possible, it is a good idea to programmatically assocate the instructions describing the change with the form control itself.

**Procedure:**

1. Locate content where changing the setting of a form contrl results in a change of context.
2. Check to see that an explanation of what will happen when the control is changed is available prior to the controls activation.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G13)

</details>

<details>
  <summary>What abjective of ensuring that information conveyed by color differences is also available in text?</summary>

The objective of this technique is to ensure that when color differences are used to convey information, such as required form fields, the information conveyed by the color differences are also conveyed explicitly in text.

**Procedure:**

1. Check taht the information conveyed is also available in thext and that the text is not conditional content.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G14)

</details>

<details>
  <summary>What abjective of using a tool to ensure that content does not violate the general flash threshold or red flash threshold?</summary>

The purpose of testing for violations of the general and red flash thresholds is to allow people who have photosensitive seizures to viwe Web sites without encountering material that is likely to cause a seizure. Warnings can be provided but people may miss them and children may not be able to read or understand them. With this technique all material is checked and if it violates flash or red flash thresholds it is either not put on the site or it is modified so that it does not violate the thresholds.

**Procedure:**

1. Check to see that content does not violate the general flash and/or red flash threshold use a toll to detmine that neither the General Flash nor Red Flash threshold were exceeded.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G15)

</details>

<details>
  <summary>What abjective of ensuring that a contrast ratio of at least 7:1 exists between text and background behind the text?</summary>

The obective of this technique is to make sure that users can read text that is presented over a background. This technique goes beyond the 4.5:1 contrast technique to provide a higher level of contrast to make it easier for people with low vision to read.

**Procedure:**

1. Measure the relative luminance of each letter using the formula: L = 0.2126 _ R + 0.7152 _ G + 0.0722 \* B.
2. Measure the relative luminance of the background pixels immediately next to the letter using same formula.
3. Calculate the contrast ratio using the following formula: (L1 + 0.05) / (L2 + 0.05), where:

- L1 is the relative luminance of the lighter of the foreground or background colors;
- L2 is the relative luminance of the darker of the foreground or background colors.

4. Check that the contrast ratio is equal to or greater than 7:1.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G17)

</details>

<details>
  <summary>What abjective of ensuring that a contrast ratio of at least 4.5:1 exists between text and background behind the text?</summary>

The obective of this technique is to make sure that users can read text that is presented over a background. For Success Criterion 1.4.3, this technique describes the minimym contrast ration for text that is less than 18(if not blod) point ad less than 14 point(if blod). For Success Criterion 1.4.6, this technique relaxes the 7:1 contrast ratio requirement for text that is at least 18 point (if not blod) or at least 14 point (if blod).

**Procedure:**

1. Measure the relative luminance of each letter using the formula: L = 0.2126 _ R + 0.7152 _ G + 0.0722 \* B.
2. Measure the relative luminance of the background pixels immediately next to the letter using same formula.
3. Calculate the contrast ratio using the following formula: (L1 + 0.05) / (L2 + 0.05), where:

- L1 is the relative luminance of the lighter of the foreground or background colors;
- L2 is the relative luminance of the darker of the foreground or background colors.

4. Check that the contrast ratio is equal to or greater than 4.5:1.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G18)

</details>

<details>
  <summary>What abjective of ensuring that no component of the content flashes more than three times in any 1-second period?</summary>

The obective of this technique is to avoid flashing at rates that are known to cause seizures if the flashes are bright and large enough. Since some users may be using screen enlargers, this technique limits the flashing of any size content to no more than three flashes in any 1-second period.

**Procedure:**

1. Check that there are no more than three flashes during any 1-second period.
2. If there are three flashes, check that the Light/Dark status at the end of the 1-second period is the same as at the start.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G19)

</details>

<details>
  <summary>What abjective of ensuring that users are not trapped in content?</summary>

The obective of this technique is to ensure that keyboard users do not become trapped in a subset of the content that can only be exited using a mouse or pointing device. A common example is content rendered by plug-ins. Plug-ins are user agents tat render content inside the user agent host window and respond to all user actions that takes place while the plug-in has the focus. If the plug-in does not provide a keyboard mecahnism to return forcus to the parent window, users who must use the keyboard may become trapped in the plug-in content.

**Procedure:**

1. Tab through content from start to finish.
2. Check to see that keyboard focus is not trapped in any of the content.
3. If keyboard focus appears to be trapped in any of the content, check that help information is available expaining how to exit the content and can be accessed via the keyboard.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G21)

</details>

<details>
  <summary>What abjective of identifying the purpose of a link using link text combined with the text of the enclosing sentence?</summary>

The obective of this technique is to identify the purpose of a link from the link and its sentence context. The sentence enclosing the link provides context for an otherwise unclear link. The description lets a user distinguish this link from links in the Web page that lead to other destinations and helps the user determine whether to follow the link. Note that simply providing the URI of the destination is generally not sufficiently descriptive.

**Procedure:**

1. Check that the link is part of a sentence.
2. Check that text of the link combined with the text of its enclosing sentence describes the purpose of the link.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G53)

</details>

<details>
  <summary>What abjective of including a sign language interpreter in the video stream?</summary>

The obective of this technique is to allow users who cannot hear or read text rapidly to be able to access synchronized media material.

**Procedure:**

1. Have someone watch the program who can hear and is familiar with the sign language being used.
2. Check to see if there is a sign language interpreter on screen.
3. Check to see that dialogue and important sounds are being conveyed by the interpreter visible on screen.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G54)

</details>

<details>
  <summary>What abjective of linking to definitions?</summary>

The obective of this technique is to make the definition of a word, phrase, or abbreviation available by providing the definition, either within the same Web page or in a different Web page, and establishing a link between the item and its definition.

**Procedure:**

1. Check that at least the first instance of the item is a link.
2. Check that each link navigates to the definition of the item.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G55)

</details>

<details>
  <summary>What abjective of mixing audio files so that non-speech sounds are at least 20 decibels lower than the speech audio content?</summary>

The obective of this technique is to allow authors to include sound behind speech without making it too hard for people with hearing problems to understand the speech. Making sure that the foreground speech is 20 db louder than the background sound makes the speech 4 times louder than the background audio. For information on Decibels.

**Procedure:**

1. Locate loud values of background content between foreground speech.
2. Measure the volume in dB SPL.
3. Measure the volume of the foreground speech in dB SPL.
4. Subtract the values.
5. Check that the result is 20 or greater.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G56)

</details>

<details>
  <summary>What abjective of ordering the content in a meaningful sequence?</summary>

The obective of this technique is to ensure that the order of content presented to assistive technologies allows the user to make sense of the content. Some techniques permit the content to be rendered visually in a meaningful sequence even if this is different from the order in which the content is encoded in the underlying source file.

**Procedure:**

1. Linearize content using a standard approach for the technology.
2. Check to see if the order of content yields the same meaning as the original.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G57)

</details>

<details>
  <summary>What abjective of placing a link to the alternative for time-based media immediately next to the non-text content?</summary>

With this technique, a link to the collated document of captions and audio description is provided. The collated document could be at another location on the same Web page or at another URI. A link to the collated document is immediately adjacent to the non-text content. The link can be immediately before or after the synchronized media content. If the collated document is on the same Web page as other content the put "End of document" at the end so that they know when to stop reading and retur nto their previous place. If a Back button will not take the person back to the point from which they jumped, then a link back to the non-text content location is provided.

**Procedure:**

1. Check for the presence of a link immediately before of after the non-text content.
2. Check that it is a valid link that points directly to the collated document of this particular synchronized media.
3. Check for the availability of a link or back function to get the user back to the original location of the synchronized media content.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G58)

</details>

<details>
  <summary>What abjective of placing the interactive elements in an order that follows sequences and relationships within the content?</summary>

The objective of this technique is to ensure that interactive elements receive focus in an order that follows sequences and relationships in the content. When designing the content, the interactive elements such as links and form controls are placed in the content so that the default tab order follows the sequences and relationships in the content. Each technology defines its defautl tab order, so the mechanism for placing the controls in the content will depend on the technology used.

**Procedure:**

1. Determine the order of interactive elements in the content.
2. Determine the logical order of interactive elements.
3. Check tat the order of the interactive elements in the content is the same as the logical order.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G59)

</details>

<details>
  <summary>What abjective of playing a sound that turns off automatically within three seconds?</summary>

The purpose of this technique is to allow autoris to play a sound on their Web page but avoid the problem of users not being able to use their screen readers due to interference by the content sound. It also allows the author to avoid putting controls on the Web page to control the sound - and the problem faced by users with screen readers in finding the control.

**Procedure:**

1. Load the Web page.
2. Check that all sound that plays automatically stops in 3 seconds or less.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G60)

</details>

<details>
  <summary>What abjective of presenting repeated components it the same relative order each time they appear?</summary>

The objective of this technique is to make content easiear to use by making the placement of repeated components more predictable. This technique helps maintain consistent layout or presentation between Web pages by presenting components that are repeated in these Web units in the same relative order each time they appear. Other components can be inserted between them, but their relative order is not changed.

**Procedure:**

1. List components that are repeated on teach Web page in a set of Web pages.
2. For each component check taht it appears in the same relative order with regard to other repeated components on each Web page where it appears.
3. For each navigational component, check that the links or programmatic references are always in the same relative order.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G61)

</details>

<details>
  <summary>What abjective of providing a gloassary?</summary>

The objective of this technique is to make the definition of a word, phrase, or abbreviation available by providign the definition in a glossary. A glossary is an alphabetical list of words, hprases, and abbreviations with their definitions. Glossaries are most appropriate when the words, phrases, and abbreviations used within the content relate to a specific descipline or technology area. A glossary can also provide the pronunciation of a word or phrase.

**Procedure:**

1. Check tat either

- The glossary is included in the Web page, or
- A mechanisms is available to locate the glossary.

2. Check that each word, phrase or abbreviation to be defined is defined in the glossary.
3. Check that the glossary contains only one definition for each item.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G62)

</details>

<details>
  <summary>What abjective of providing a site map?</summary>

The site map serves several purposes.

- It provides an overview of the entire siete.
- It helps users understand what the site contains and how the content is organized.
- It offers and alternative to complex navigation bars that may be different ad different parts of the site.

**Procedure:**

1. Check tat the site contains a site map.
2. Check that the links in the site map lead to the corresponding sections of the site.
3. For each link in the site map, check that the target page contains a link to the site map.
4. For each page in the site, check that the page can be reached by following some set of links that start at the site map.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G63)

</details>

<details>
  <summary>What abjective of providing a Table of Contents?</summary>

The table of contents serves two purposes:

- It gives users an overview of the document's contents and organization.
- It allows readers to go directly to a specific section of an on-line document.

**Procedure:**

1. Check tat a table of contents or a link to a table of contents exists in the document.
2. Check taht the values and order of the entries in the table of contents correspond to the names and order of the sections of the document.
3. Check that the entries in the table of contents link to the correct sections of the document.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G64)

</details>

<details>
  <summary>What abjective of providing a breadcrumb trail?</summary>

A breadcrumb trail helps the user to visualize how content has been structured adn how to navigate back to previous Web pages, and may identify the current location within a series of Web pages. A breadcrumb trail either displays locations in the path the user took to reach the Web page, or it displays the location of the current Web page within the organization of the site.

**Procedure:**

1. Navigate to a Web page.
2. Check that a breadcrumb trail is displayed.
3. Check that the breadcrumb trail displays the correct navigational sequence to reach the current location or the correct hierarchical path to the current location within the site structure.
4. For a breadcrumb trail that does not include the current location:

- Check that all elements in the breadcrumb trail are implemented as links.

5. For a breadcrumb trail that does include the current location:

- Check that all elements except for the current location are implemented as links.
- Check that the current location is not implemented as a link.

6. Check that all links navigate to the correct Web page as specified by teh breadcrumb trail.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G65)

</details>
