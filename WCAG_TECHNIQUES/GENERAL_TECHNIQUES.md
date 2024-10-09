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

<details>
  <summary>What abjective of providing a short text alternative that describes the purpose of live audio-only and live video-only content?</summary>

This technique provides a short text alternative for Live audio-only and live video-only content. This text may be used in combination with a full text alternative for time-based media, or in combination with audio description. Those alternatives, however, are not part of this technique. The purpose of this technique is to ensure that the user can determine what the non-text content is, even if they cannot access it.

**Procedure:**

1. Remove, hide, or mast the non-text content.
2. Display the sort text alternative(s).
3. CHeck that the purpose of the non-text content is clear, even if content is lost.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G68)

</details>

<details>
  <summary>What abjective of providing an alternative for time based media?</summary>

The purpose of this technique is to provide an accessible alternative way of presenting the information in a synchronized media presentation.

**Procedure:**

1. View the synchronized media presentation while referring to the alternative for time-based media.
2. Check that the dialogue in the alternative for time-based media matches the dialogue in the synchronized media presentation.
3. Check that the alternative for time-based media has descriptions of sounds.
4. Check that the alternative for time-based media has descriptions of setting ans setting changes.
5. Check that the alternative for time-based media has descriptions of actions and expressions of any 'actors' (people, animals etc).
6. If the alternate version(s) are on a separate page, check for the availability of link(s) to allow the user to get to the other versions.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G69)

</details>

<details>
  <summary>What abjective of providing a function to search an online dictionary?</summary>

The objective of this technique is to provide the definition of words, phrases, jargon, or abbreviation expansions by adding a mechanism to access an on-line dictionary to the Web page. This technique uses existing resources on the Web to provide the definition rather than requiring the author to create a glossary or other mechanism within the site. By providing access from within the Web page, a user can easily locate the desired definition. This technique can only be used if the online dictionary returns the correct defintion.

**Procedure:**

1. Check that a mechanism exists within the Web page to search for the word, phrase, or abbreviation via an on-line dictionary.
2. Check that the result of the search of the dictionary for the word, phrase, or abbreviation is the correct definition.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G70)

</details>

<details>
  <summary>What abjective of providing a help link on every Web page?</summary>

The objective of this technique is to provide context sensitive help for users as they enter data in forms by providing at least one link to the help information on each Web page. The link targets a help page with information specific to that Web page. Another approach is to provide a help link for every interactive control. Positioning this link immediately before or after the control allows users to easily tab to it if they have problems in the control. Displaying the help information in a nyw browser window ensures that any data that has already been entered into the form will not be lost.

**Procedure:**

1. Identify a Web page that contais forms. Determine if there is at least one link to help information explaining how to complete the form on this Web page.
2. Determine if there is at least one linkg to help information explaining how to completer the form on this Web page.
3. Determine of there are links either before or after each interective control to information specific to that control.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G71)

</details>

<details>
  <summary>What abjective of providing a long description in another location with a link to it that is immediately adjacent to the non-text content?</summary>

The objective of this technique is to provide a way to link to remove long descriptions in technologies that do not have a long description feature built directly into them or where the feature is known to not be supported.

**Procedure:**

1. Check for the presence of a link immediately before or after the non-text content.
2. Check that the link is a valid link that points directly to the long description of this particular non-text content.
3. Check that the long description conveys the same information as the non-text content.
4. Check for the availability of a link or back function to get the user back to the original location of the non-text content.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G73)

</details>

<details>
  <summary>What abjective of providing a long description in text near the non-text content, with a reference to the location of the long description in the short description?</summary>

The objective of this technique is to provide a long description without requiring the user to jump off to another location for the description. It also allows all users to see the description which may be useful to anyone who might miss some features in the non-text content.

**Procedure:**

1. Check that the short text alternative includes the location of the long description.
2. Check that the long description is near the non-text content both visually and in the linear reading order.
3. Check that the long description conveys the same information as the non-text content.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G74)

</details>

<details>
  <summary>What abjective of providing a mechanism to postpone any updating of content?</summary>

The objective of this technique is to ensure that users can pospone automatic updates of content, or other non-emergency interruptions. This can be accomplished either through a preference or by alerting users of an imminent update and allowing them to suppress it. If a preference is provided, automatic content update can be disabled by defautl and users can specify the frequency of automatic content updates if they choose to enable the setting.

**Procedure:**

1. Find pages with content that automatically updates.
2. For each automatic update, look for a mechanism to adjust the timing of the updates.
3. Check that automatic updating is disabled by default or that the user is warned before an automatic update occurs and allowed to suppress it.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G75)

</details>

<details>
  <summary>What abjective of providing a mechanism to request an update of the content instead of updating automatically?</summary>

The objective of this technique is to let the user control if and when content is updated, in order to avoid confusion or disorientation caused by automatic refreshes that cause a change of context. Users of screen readers may find automatic updates confusing because it is not always clear what is happening. When a page is refreshed, the screen reader's "virtual cursor", which marks the user's current location on the page, is moved to the top of the page. People who use screen magnification software and people with reading disabilities may also be disoriented when pages are refreshed automatically.

**Procedure:**

1. Find mechanisms to update the content.
2. For each such mechanism, check if it allows the user to request an update.
3. For each such mechanism, check if it can cause an automatic update.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G76)

</details>

<details>
  <summary>What abjective of providing a second, user-selectable, audio track that includes audio descriptions?</summary>

The objective of this technique is to provide an audio (spoken) version of information that is provided visually so that it is possible for people who cannot see to be able to understand audio-visual material.

**Procedure:**

1. Check that the ability exists to turn on the audio track that includes audio descriptions. For example, by using a control within the content itself or by selecting a control or preference in the media player or operating sustem.
2. Listen to the synchronized media.
3. Check to see if gaps in dialogue are used to convey important information regarding visual content.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G78)

</details>

<details>
  <summary>What abjective of providing a spoken version of the text?</summary>

Some users who have difficulty sounding out (decoding) words in written text find it very helpful to hear the text read aloud. This service can now be provided easily uding either recorded human speech or synthetic speech. For example, there are a number of products that authors can use to convert text to synthetic speech, then save the spoken version as an audio file. A link to the spoken version can then be provided within the content. Const depends in part on the quality of the voice used and whether the text is likely to change frequently.

**Procedure:**

1. Check if a spoken version of the content is available.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G79)

</details>

<details>
  <summary>What abjective of providing a submit button to initiate a change of context?</summary>

The objective of this technique is to provide a mechanism that allows users to explicitly request changes of context. Since the intended use of a submit button is to generate an HTTP request that submits data entered in a form, this is an appropriate control to use for causing a change of context and is a practice that does not create confusion for users.

**Procedure:**

1. Find all forms in the content.
2. For each form, check that it has a sumit button.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G80)

</details>

<details>
  <summary>What abjective of providing a synchronized video of the sign language interpreter that can be displayed in a different viewport or overlaid on the image by the player?</summary>

The objective of this technique is to allow users who cannot hear or read text rapidly to be able to access synchronized media material without affecting the presentation of the material for all viewers.

**Procedure:**

1. Enable the display of the sign-language window in the player.
2. Have someone watch the program who can hear and is familiar with the sign language being used.
3. Check to see if there is a sign language interpreter on screen or in a separate window.
4. Check to see that dialogue and important sounds are being conveyed by the interpreter and are synchronized with the audio.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G81)

</details>

<details>
  <summary>What abjective of providing a text alternative that identifies the purpose of the non-text content?</summary>

The purpose of this technique is to provide useful information via the text alternative even if the full function of the non-text content cannot be provided.

**Procedure:**

1. Remove, hide, or mask the non-text content.
2. Replace it with the text alternative.
3. Check that the purpose of the non-text content is clear - even if function is lost.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G82)

</details>

<details>
  <summary>What abjective of providing text descriptions to identify required fields that were not completed?</summary>

The objective of this technique is to notify the user when a field that must be completed has not been completed. When users fail to provide input for any mandatory form fields, information is provided in text to enable the users to identify which fields were omitted. Another approach, using server-side validation, is to re-display the form (including any previously entered data), with either a text description at the location of the omitted mandatory field, or a text description that identifies the omitted mandatory fields.

**Procedure:**

1. Fill out a form, deliverately leaving one or more required fields blank, and submit it.
2. Check that a text description is provided identifying the mandatory field(s) that was not completed.
3. Check that other data previously entered by the user is re-displayed, unless the cata is in a security related field where it would be inappropriate to retain the data for re-display.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G83)

</details>

<details>
  <summary>What abjective of providing a text description when the user provides information that is not in the list of allowd values?</summary>

When users enter input that is validated, and errors are detected, the nature of the error needs to be described to the user in manner they can access. One approach is to present and alert dialog that describes fields with errors when the user attempts to submit the form. Another approach, if validation is done by the server, is to return the form and a text description at the top of the page that indicates the fact that there was a validation problem, describes the nature of the problem, and provides ways to locate the field(s) with a problem easily. The "in text" portion of the Success Criterion underscores that it is not sufficient simply to indicate that a field has an error by putting an asterisk on its label or turning the label red. A text description of the problem should be provided.

**Procedure:**

1. Enter invalid data in a form filed.
2. Check that information is provided in text about the problem.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G84)

</details>

<details>
  <summary>What abjective of providing a text description when user input falls outside the required format or values?</summary>

The objective of this technique is to provide assistance in correctiong input errors where the information supplied by the user is not accepted. When users enter data input that is validated, and input errors are detected, information about the nature and location of the input error is provided in text to enable the users to identify the problem. One approach is to use client-side validation and provide an alert dialog box that described the error immediately when users enter invalid data in field. Another approach, using server-side validation, is to re-display the form, and a text description at the top of the page that indicates the fact that there was an error, describes the nature of the problem, and provides ways to easily loccate the field(s) with a problem.

**Procedure:**

1. Fill out a form, deliberately enter user input that falls outside the required format or values.
2. Check that a text description is provided that identifies the field in error and provides some information about the nature of the invalid entry and how to fix it.
3. Check that other data previously entered by the user is re-displayed, unless the data is in a security related field where it would be inappropriate to retain the data for re display.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G85)

</details>

<details>
  <summary>What abjective of providing a text summary can be understood by people with lower secondary education level reading ability?</summary>

The objective of this technique is to provide a summary of complex content. The summary is provided in addition to the original content.

**Procedure:**

1. Measure the readability of the summary.
2. Check that the summary requires reading ability less advanced than the lower secondary education level.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G86)

</details>

<details>
  <summary>What abjective of providing closed captions?</summary>

The objective of this technique is to provide a way for people who have hearing impairments or otherwise have trouble hearing the dialogue in synchronized media material to be able to view the material and see the dialogue and sounds without requiring people who are not deaf to watch the captions. With this technique all of the dialogue and important sounds are embedded as text in a fashion that causes the text not to be visible unless the user requests it. As a result they are visible only when needed. This requires special support for captioning in the user agent.

**Procedure:**

1. Turn on the closed caption fature of the media player.
2. View the synchronized media content.
3. Check that captions.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G87)

</details>

<details>
  <summary>What abjective of providing descriptive titles?</summary>

The objective of this technique is to give each Web page a descriptive title. Descriptive titles help users find content, orient themselves within it, and navigate through it. A descriptive title allows a user to easily identify what Web page they are using and to tell when the Web page has changed. The title can be used to dientify the Web page without requiring users to read or interpret page content. Users can more quickly identify the content they need when accurate, descriptive titles apear in site maps or lists of search results. When descriptive titles are used within link text, they help users navigate more precisely to the content they are interested in.

**Procedure:**

1. Check that the Web page has a title.
2. Check that the title is relevant to the content of the Web page.
3. Check that the Web page can be identified using the title.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G88)

</details>

<details>
  <summary>What abjective of providing expected data format and example?</summary>

The objective of this technique is to help the user avoid input errors by informing them about restrictions on the format of data that they must enter. This can be done by describing characteristics of the format or providing a sample of the format the data should have.

**Procedure:**

1. Identify form controls that will only accept user input data in a given format.
2. Determine if each of the form controls identified in 1 provides information about the expected format.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G88)

</details>
