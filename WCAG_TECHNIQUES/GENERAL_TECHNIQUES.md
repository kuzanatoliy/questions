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

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G89)

</details>

<details>
  <summary>What abjective of providing keyboard-triggered event handlers?</summary>

The objective of this technique is to permit individuals who rely on keyboard interface to access the functionality of the content. To do this, make sure that all event handlers triggered by non-keyboard interface to access the functionality of the content. To do this, make sure that all event handlers triggered by non-keyboard UI events are also associated with a keyboard-based event, or provide redundant keyboard-based mechanisms to accomplish the functionality provided by other device specific functions.

**Procedure:**

1. Check that all functionality can be accessed using only the keyboard.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G90)

</details>

<details>
  <summary>What abjective of providing link text that describes the purpose of a link?</summary>

The objective of this technique is to describe the purpose of a link in the text of the link. The description lets a user distinguish this link from links in the Web page that lead to other destinations and helps the user determine whether to follow the link.

**Procedure:**

1. Check that text of the link desctives the purpose of the link.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G91)

</details>

<details>
  <summary>What abjective of providing long description for non-text content that serves the same purpose and presents the same information?</summary>

The objective of this technique is to provide a long text alternative that serves the same purpose and presents the same information as the original non-text content when a short text alternative is not sufficient.

**Procedure:**

1. Remove, hide, or mask the non-text content.
2. Display the long description.
3. Check that the long description conveys the same information conveyed by the non-text content.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G92)

</details>

<details>
  <summary>What abjective of providing open (always visible) captions?</summary>

The objective of this technique is to provide a way for people who are deaf or otherwise have trouble hearing the dialogue in audio visual material to be able to view the material. With this technique all of the dialogue and important sounds are embedded as text in the video track. As a result they are always visible and no special support for captioning is required by the user agent.

**Procedure:**

1. Watch the synchronized media with closed captioning turned off.
2. Check that captions are visible.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G93)

</details>

<details>
  <summary>What abjective of providing short text alternative for non-text content that serves the same purpose and presents the same information as the non-text content?</summary>

The objective of this technique is to create a text alternative that serves the same purpose and presents the same information as the original non-text content. As a result, it is possible to remove the non-text content and replace it with the texxt alternative and no functionality or information would be lost. This text alternative should not necessarily describe the non-text content. It should serve the same purpose and convey the same information. This may sometimes result in a text alternative that looks like a description of the non-text content. But this would only be true if that was the best way to serve the same purpose.

**Procedure:**

1. Remove, hide, or mask the non-text content.
2. Replace it with the text alternative.
3. Check that nothing is lost.
4. If the non-text content contains words that are important to understanding the content, the words are included in the text alternative.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G94)

</details>

<details>
  <summary>What abjective of providing short text alternatives that provide a brief description of the non-text content?</summary>

This technique is used when the text needed to serve the same purpose and present the same information as the original non-text content is too lengthy or when this goal cannot be achieved with text alone. In that case this technique is used to probide a short text alternative that briefly describes the non-text content.

**Procedure:**

1. Check for the presence of a short text alternative that provides a brief description of the non-text content.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G95)

</details>

<details>
  <summary>What abjective of providing textual identification of items that otherwise rely only on sensory information to be understood?</summary>

The objective of this technique is to ensure that items within a Web page are referenced in the content not only by shape, size, sound or location, but also in ways that do not depend on that sensofy perception. For example, a reference may also describe the function of the item or its label.

**Procedure:**

1. Check that the reference contains additional information that allows the item to be located and identified without any knowledge of its shape, size, or relatibe position.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G96)

</details>

<details>
  <summary>What abjective of providing the first use of an abbreviation immediately before or after the expanded form?</summary>

The objective of this technique is to make the expanded forma of an abbreviation available by associating the expanded form with its abbreviation the first time it occurs within a Web page. The expansion of any abbreviation can be found by searching the Web page for the first use.

**Procedure:**

1. Search for the first use of that abbreviation in the authored component.
2. Check that the first use is immediately preceded or followed by the expanded form of the abbreviation.
3. Check that the expanded form is the correct expanded form for the use of the abbreviation.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G97)

</details>

<details>
  <summary>What abjective of providing the ability for the user to review and correct answers before submitting?</summary>

The objective of this technique is to provide users with a way to ensure their imput is correct before completing an irreversible transaction. Testing, financial, and legal applications permit transactions to occur which cannot be "undone". It is therefore important that there be no errors in the data submission, as the user will not have the opportunity to correct the error once the transaction has been committed.

**Procedure:**

1. Check that the user is promted to review and confirm data.
2. If user data are collected in multiple steps, the user is allowd to return to previous stpes to review and change data.
3. Determine if a summary of all data input by the user is provided before the transaction is committed and a method is provided to correct errors if necessary.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G98)

</details>

<details>
  <summary>What abjective of providing the ability to recover deleted information?</summary>

When a Web application provides the capability of deleting information, the server can provide a means to recover information that was deleted in error by a user. One approach is to delay deleting the data by merely marking it for deletion or moving it to a holding area and waiting some period of time before actually deleting it. During this time period, the user can request that the data be restored or can retrive it ffrom the holding area. Another approach is to record all delete transactions in such a way that data can be restored if requested by the user such as in the edit history stored by wikis and source control applications. The retrievable information that is stored should be that which would be needed to correct the transaction.

**Procedure:**

1. Identify functionality that allows deleting content.
2. Delete content and attempt to recover it.
3. Check if deleted information can be recovered.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G99)

</details>

<details>
  <summary>What abjective of providing a short text alternative which is the accepted name or a descriptive name of the non-text content?</summary>

The objective of this technique is to allow users to identify the non-text content even if the non-text content is intended to provide a specific sensory experience. For example, a deafperson may want to know what an audio instrumental file is - even if they cannot hear it. Similarly, a blind person may want to know what the subject of a visual image is - even if they cannot see it.

**Procedure:**

1. Check that short text alternative provides a descriptive name.
2. Check that short text alternative provides a name that has be previously been given to the non-text content by the author or another.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G100)

</details>

<details>
  <summary>What abjective of providing the definition of a word or phrase used in an unusual or resticted way?</summary>

The objective of this technique is to provide a definition for any word used in an unusual or restricted way.

A word is used in an unusual or restricted way when:

- dictionalries give several definitions of the word but one specific definition must be used in order to understand the content;
- a specific definition must be used in order to understand the content and dictionaries list that definition as rare, archaic, obsolete, etc.;
- the author creates a new definition that must be used in order to understand the content.

**Procedure:**

1. Check that a definition is provided for the word or phrase.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G101)

</details>

<details>
  <summary>What abjective of providing the expansion or explanation of an abbreviation?</summary>

The objective of this technique is to provide information necessary to understand an abbreviation.

**Procedure:**

1. If the abbreviation has no expanded form, an explanation is provided.
2. If the expanded form of the abbreviation is in a different language than the content, an explanation is provided.
3. Otherwise, the expanded form is provided.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G102)

</details>

<details>
  <summary>What abjective of providing visual illustrations, pictures, and symbols to help explain ideas, events, and processes?</summary>

The objective of this technique is to provide visual illustrations that help users with reading disabilites understand difficult text that describes concepts or processes. The illustrations are provided in addition to the text.

**Procedure:**

1. Identify text taht discusses ideas or processes that must be understood in order to use the content.
2. Check if visual illustations are available in the content or through links within the content.
3. Check that visual illustrations show the concepts or processes discussed in the text.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G103)

</details>

<details>
  <summary>What abjective of using "activate" rather than "focus" as a trigger for changes of context?</summary>

The objective of this technique is to provide a method for activating things that is predictable by the user. Users with cognitive disabilities and people using screen readers or screen magnifiers may be confused by an unexpected event such as automatic form submission or activation of a function that causes a change of context.

**Procedure:**

1. Using a keyboard, cycle focus through all content.
2. Check that not changes of context occur when any component receives focus.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G107)

</details>

<details>
  <summary>What abjective of using markup features to expose the name and role, allow user-settable properties to be directly set, and provide notification of changes?</summary>

The objective of this technique is to allow assistive technology to understand Web content so that it can convey equivalent information to the user through and alternate user interface and allow them to operate controls through the AT.

**Procedure:**

1. Visually inspect the markup or use a tool.
2. Check that proper markup is used such that the name and role, for each user interface component can be determined.
3. Check taht proper markup is used such that the user interface components that accept user input can all be operated from AT.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G108)

</details>

<details>
  <summary>What abjective of using an instant client-side redirect?</summary>

The objective of this technique is to enable redirects on the client side without confusing the user. Redirects are preferably implemented on the server side, because a server-side redirect does not cause new content to be displayed before the server sends the content located at the new URI. However, authors do not always have control over server-side technologies; in that case, they can use a client-side redirect. A client-side redirect is implemented by code inside the content that instructs the user agent to retrieve content from a different URI. It is important that the redirecting page or Web page only contains information related to the redirect.

**Procedure:**

1. Find each link or programmatic reference to another page or Web page.
2. For each link or programmatic reference, check if the referenced Web page contains code that causes a client-side redirect.
3. For each link or programmatic reference that causes a client-side redirect, check if the redirect is implemented without a time limit or delay and that the page only contatins information related to the redirect.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G110)

</details>

<details>
  <summary>What abjective of using color and pattern?</summary>

The objective of this technique is to ensure that when color differentces are used to convey information within non-text content, patterns are included to convey the same information in a manner that does not depend on color.

**Procedure:**

1. Check that all information that is conveyed using color is also conveyed using patterns that do not rely on color.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G111)

</details>

<details>
  <summary>What abjective of using inline definitions?</summary>

The objective of this technique is to provide a definition in context for any word used in an unusual or restricted way. The definition is provided in the text, either just before or just after the word is used. The definition may be included in the same sentence as the word that is being defined, or in a separate sentence.

**Procedure:**

1. Check that the word is defined in text either before or after the first occurrence of the word.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G112)

</details>

<details>
  <summary>What abjective of using semantic elements to mark up structure?</summary>

The objective of this technique is to mark up the structure of the Web content using the appropriate semantic elements. In other words, the elements are used according to their meaning, not because of the way they appear visually.

**Procedure:**

1. Check if there are parts of the content that have a semantic function.
2. For each part that has a semantic function, if corresponding semantic markup exists in the technology, check that the content has been marked up using that semantic markup.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G115)

</details>

<details>
  <summary>What abjective of using text to convey information that is conveyed by variations in presentation of text?</summary>

The objective of this technique is to ensure that information conveyed through variations in the formatting of text is conveyed in text as well. When the visual appearance of text is varied to convey information, state the infroamtion explicitly in the text. Variations in the visual appearance can be made by changes in font face, font size, underline, strike through and various other text attributes. When these types of variations convey information, that information needs to be available elsewhere in the content via text. Including additional sections in the document or an inline description where the variation in presentation of text occurs can be used to convey the information.

**Procedure:**

1. Find items where variations in presentation of text are used to convey information.
2. For those items, check to determine if information conveyed visually is also stated explicitly in text.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G117)

</details>

<details>
  <summary>What abjective of providing the pronunciation immediately following the word?</summary>

The objective of this technique is to make the pronunciation of a word available by providing the pronunciation after the word at least the first time it occurs within a Web page.

**Procedure:**

1. Search for the first use of that word in the Web page.
2. Check that the first use is immediately followed by the pronunciation of the word.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G120)

</details>

<details>
  <summary>What abjective of linking to pronunciations?</summary>

The objective of this technique is to make the pronunciation of a word available by providing information about the pronunciation, either within the same Web page or in a different Web page, and establishing a link between the item and its pronunciation.

**Procedure:**

1. Check that at least the first instance of the item is a link.
2. Check that each link navigates to information about the pronunciation of the item.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G121)

</details>

<details>
  <summary>What abjective of adding a link at the beginning of a block of repeated content to go to the end of the block?</summary>

The objective of this technique is to provide a mechanism to bypass a block of matterial by skipping to the end of the block. The first link in the block or the link directly preceding the block moves focus to the content immediately after the block. Activating the link advances the keyboard focus past the block. When there are multiple blocks to be skipped, the user skips from block to block via these links.

**Procedure:**

1. Check taht a link is the last focusable control before the block of repeated content or the first link in the block.
2. Check that teh description of the link communicates that it skips the block.
3. Check that the link is either always visible or visible when it has keyboard focus.
4. Check that after activating the link, the keyboard focus has moved to the content immediately after the block.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G123)

</details>

<details>
  <summary>What abjective of adding links at the top of the page to each area of the content?</summary>

The objective of this technique is to provide a mechanism to bypass blocks of material by providing a list of links to the different sections of the content. The links in this list, like a small table of contents at the beginning a list of links to the different sections of the content. The links in this list, like a small table of contents at the beginning of the content, set focus to the different sections of the content. This technique is particularly useful for pages with many independent sections, such as portals. It may also be combined with other techniquest for skipping blocks within a section.

**Procedure:**

1. Check that the only controls in the Web page that precede the link are other links in the set.
2. Check that the description of each link communicates that it links to some section of the content.
3. Check that the link is either always visible or visible when it has keyboard focus.
4. Check that activating the link moves the focus to that section of the content.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G124)

</details>

<details>
  <summary>What abjective of providing links to navigate to related Web pages?</summary>

The objective of this technique is to make it possible for user to locate additional inforamtion by providing links to related Web pages. It is one of a series of techniques for locating content that are sufficient for addressing Success Criterion 2.4.5. Links are a basic component of the World Wide Web. They are the mechanism that makes the Web an interconnected Web of content. Most authors employ this technique automatically when creating Web pages.

**Procedure:**

1. Check whether the link leads to related information.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G125)

</details>

<details>
  <summary>What abjective of providing a list of links to all other Web pages?</summary>

The objective of this technique is to provide a list of links to all the Web pages in the set on each Web page. It is one of a series of techniques for locating content that are sufficient for addressing Succes Criterion 2.4.5. This technique is only effective for small sets of Web pages; if the list of links is longer than the rest of the content in the Web page, it may make the Web page more difficult for users to understand and use.

**Procedure:**

1. Check that each Web page contains a list of links to the other Web pages in the site.
2. Check that the links in the list lead to the corresponding Web pages.
3. Check that the list contents a link for every Web page in the site.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G126)

</details>

<details>
  <summary>What abjective of identifying a Web page's relationship to a larger collection of Web pages?</summary>

The objective of this technique is to enable users to identify the relationship between the current Web page and other Web pages in the same collection. In some cases this can be done programmatically - for example by using the rel attribute of the link element in HTML. In other cases the information is provided by inluding the relevant information in the title of the Web page.

**Procedure:**

1. Check if the title of the Web page describes the Web page's relationship to the collection to which it belongs.
2. Check if the Web page includes metadata identifying the Web page's relationship to the collection to which it belongs.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G127)

</details>

<details>
  <summary>What abjective of indicating current location within navigation bars?</summary>

The objective of this technique is to help orient the user by providing information about the current location via the navigational user iterface component. This technique is especially useful when the Web pages are steps in a task that must be processed in order. Providing this indication helps the user to better understand their place in the sequence. The location may be indicated by adding an icon or text, or by changing the state of the item.

**Procedure:**

1. Check that the user is given an indication of the currently selected item within the navigational unit.
2. Check that the selected item matches the content which is being displayed.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G128)

</details>

<details>
  <summary>What abjective of providing descriptive headings?</summary>

The objective of this technique is to make section headings within Web content descriptive. Descriptive headings and titles work together to give users and overview of the content and its organization. Descriptive headings identiy sections of the content in relation both to the Web page as a whole and to other sections of the same Web page.

**Procedure:**

1. Determine if the Web page contains headings.
2. Check that each heading identifies its section of the content.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G130)

</details>

<details>
  <summary>What abjective of providing descriptive headings?</summary>

The objective of this technique is to ensure that the label for any interactive component within Web content makes the component's purpose clear. Using the appropriate technology specific techniques for technologies for associating labels with interactive controls allows assistive technology to recognize the label and present it to the user, therefore allowing the user to identify the purpose of the control. The label may also be used to include text or a text symbol indicating that input is required.

**Procedure:**

1. Identify the purpose of the interface component.
2. Check that each hlabel makes the component's purpose clear.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G131)

</details>

<details>
  <summary>What abjective of providing a checkbox on the first page of a multipart form that allows users to ask for longer session time limit or no session time limit?</summary>

The objective of this technique is to minimize the risk that users with disabilities will lose their work by providing a checkbox to request additional time to complete multipart forms. The checkbox can allow the user to requiest a specific amount of additional time or an indefinite extension.

**Procedure:**

1. Check that the Web page includes a checkbox to request additional time to complete the form.
2. Check that if the checkbox is checked, additional time is provided to complete the form.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G133)

</details>

<details>
  <summary>What abjective of using the accessibility API features of a technology to expose names and roles, to allow user-setable properties to be directly set, and to provide notification of changes?</summary>

The objective of this technique is to allow assistive technology to understand Web content so that it can convey equivalent information to the user through an alternate user interface.

**Procedure:**

1. Render content using an accessible User Agent.
2. Use an Accessibility Tool designed for the Accessibility API of the User agent to evaluate each user interface component.
3. Check that name and role for each user interface component are found by the tool.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G135)

</details>

<details>
  <summary>What abjective of providing a link at the beginning of a nonconforming Web page that points to a conforming alternate version?</summary>

The objective of this technique is to enable users to access alternate content that conforms to WCAG if the primary content or the default content that users encounter when visiting a particular URI, does not conform. The alternate page or conforming alternate version, may make some design or functionality compromises in order to conform, but must meet the requirements described in the definition in order to be a conforming alternate version.

**Procedure:**

1. Identify a page that does not conform to WCAG at the claimed conformance level.
2. Determine if the page contains a link to a conforming alternate version of the page.
3. Determine if the alternate version is a conforming alternate version of the original page and that it conforms to WCAG 2.0 at the climed conformance level.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G136)

</details>

<details>
  <summary>What abjective of using semantic markup whenever color cues are used?</summary>

The objective of this technique is to combine color and semantic markup to convey information. Most users can quickly scan the contnet to locate information conveyed by using color. For users who cannot see color, semantic markup can provide a different type of cue. User agents can then make this type of structure perceivable to the user, for example using a different visual presentation for different types of structures or by using a different voice or pitch in an auditory presentation.

**Procedure:**

1. Check that the same information is available through semantic markup.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G138)

</details>

<details>
  <summary>What abjective of creating a mechanism that allows users to jump to errors?</summary>

The objective of this technique is to help users find input errors where the information supplied by the user is not accepted. This includes fields with missing required information and fields with incorrect information. When users enter data input that is checked, and input errors are detected, a link to that the user does not have to search for it. One approach is to use server-side validation, and to re-display the form, and a text description at the top of the page that indicates the fact that there was an input error, describes the nature of the problem, and provides a link the field(s) with a problem.

**Procedure:**

1. Fill out a form, deliverately leaving a required (mandatory) field blank, and make an input error on another field and submit the form.
2. Check that a text message is provided that identifies the field that is missing required data.
3. Check that a text message is provided that identifies the field with the input error.
4. Check that there is a link to each field that is missing required data from the missing data message.
5. Check that there is a link to the list of errors from the error message.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G139)

</details>

<details>
  <summary>What abjective of separating information and structure from presentation to enable different presentations?</summary>

The objective of this technique is to facilitate the interaction of assistive technology with content by logically separationg the content's structural encoding from the presentational encoding. Structural encoding is the indication of elements such as headings, paragraphs, lists, tables, etc., and is done by using technology features reserved for the purpose. By contrast, presentational encoding is the indication of formatting effects, such as typeface, color, size, position, borders, etc., and is also supported by technology features.

**Procedure:**

1. Examine the encoding of a docuemnt.
2. Check that structural information and functionality are explicitly provided and is logically separated from presentational information.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G140)

</details>

<details>
  <summary>What abjective of organizing a page using headings?</summary>

The objective of this technique is to ensure that sections have headings that identify them. Success Criterion 1.3.1 requires that the headings be marked such taht they can be programmatically identified.

**Procedure:**

1. Examine a page with content organized into sections.
2. Check that a heading for each section exists.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G141)

</details>

<details>
  <summary>What abjective of using a technology that has commonly-available user agents that support zoom?</summary>

The objective of this technique is to ensure content can be scaled uniformly by using a Web technology supported by user agents that change text size via a Zoom tool.

**Procedure:**

1. Display content in a user agent.
2. Zoom content to 200%.
3. Check whether all content and functionality is available.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G142)

</details>

<details>
  <summary>What abjective of providing a text alternative that describes the purpose of the CAPTCHA?</summary>

The objective of this technique is to provide information via the text alternative that identifies the non-text content as a CAPTCHA. Such tests often involve asking the user to type in text taht is presented in an obscured image or audio file. From the text alternative, the user can tell that the CAPTCHA requires completing a task and what type of task it is.

**Procedure:**

1. Remove, hide or mask the CAPTCHA.
2. Replace it with the text alternative.
3. Check taht the text alternative describes the purpose of the CAPTCHA.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G143)

</details>

<details>
  <summary>What abjective of ensuring that the Web Page contains another CAPTCHA serving the same purpose using a different modality?</summary>

The objective of this technique is to reduce occasions in which a user with a disability cannot complete a CAPTCHA task. Because there are alternate CAPTCHA tasks that use different modalities, a user is more likely to be able to completer one of the tasks successfully.

**Procedure:**

1. Remove, hide or mask the CAPTCHA.
2. Replace it with the text alternative.
3. Check taht the text alternative describes the purpose of the CAPTCHA.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G144)

</details>

<details>
  <summary>What abjective of ensuring that a contrast ratio of at least 3:1 exists between text and background behind the text?</summary>

The objective of this technique is to make sure that users can read text that is presented over a background. This technique relaxes the 4.5:1 contrast ratio requirement for text that is at least 18 point or at least 14 point.

**Procedure:**

1. Measure the relative luminance of each letter using the formula: L = 0.2126 _ R + 0.7152 _ G + 0.0722 \* B.
2. Measure the relative luminance of the background pixels immediately next to the letter using same formula.
3. Calculate the contrast ratio using the following formula.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G145)

</details>

<details>
  <summary>What abjective of using liquid layout?</summary>

The objective of this technique is to be able to present content without introducing horizontal scroll bars by using layout techniques that adapt to the available horizontal space. Liquid layouts define layout regions that both resize with text, and reflow as needed to display the region on the screen. Althogh the exact layout therefore varies, the relationship of elements and the reading order remains the same. This is an effective way to create designs that present well on different devices and for users with different font size preferences.

**Procedure:**

1. Display content in a user agent.
2. Increase text size to 200%.
3. Check whether all content and functionality is available with no horizontal scrolling.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G146)

</details>

<details>
  <summary>What abjective of not specifying background color, not specifying text color, and not using technology features that change those defaults?</summary>

The objective of this technique is to make sure that users can read text that is presented over a background. With this technique the author avoids having to do any contrast measures by simply not specifying the text color and not specifying the background. As a result the colors of both are completely determined by the user agent.

**Procedure:**

1. Loo in all places that text color can be specified.
2. Check that text color is not specified.
3. Look in all areas that background color or image used as a background can be specified.
4. Check that no background color or image used as background is specified.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G148)

</details>

<details>
  <summary>What abjective of using user interface components that are highlighted by the user agent when they receive focus?</summary>

The objective of this technique is to ensure that the fucused component can be visually identified by the user by relying on user agent support. It is common for user agents to highlight standard controls in some way when they receive focus. UAAG-conformant user agents do so when they statisfy checkpoint 10.2 "Highlight selection, content focus, enable elements, visited links". When authors use standard controls for which the user agent provides this support, users are informed of the focus location in a standard, predictable way.

**Procedure:**

1. Set focus to the control.
2. Check whether the user agent has highlighted the control in some way.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G149)

</details>

<details>
  <summary>What abjective of providing text based alternatives for live audio-only content?</summary>

The objective of this technique is to allow users who cannot hear to be able to access real-time audio broadcasts. It is more difficult to create accurate real-time alternatives because there is little time to correct mistakes, to listen a second time or to consult someone to be sure the words are accurately reproduced. It is also harder to simplify or paraphrase information if it is flowing too quickly.

**Procedure:**

1. Check that a procedure and policy is in place to ensure that text alternatives are delivered in real-time.
2. Check that procedure and policy are working by conducting a random sample to see if text alternatives appear.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G150)

</details>

<details>
  <summary>What abjective of providing a link to a text transcript of a prepared statement or script if the script is followed?</summary>

The objective of this technique is to provide a transcript or script if the live audio content is following a set script. Because it is prepared in advance, the script can be more accurate and complete than live transcription. However, the script will not be synchronized with the audio as it plays. Live audio should not deviate from the script for this technique.

**Procedure:**

1. Check for the presence of a link that points directly to the script or transcript.
2. Check that the live audio follows the script.
3. If the alternate version(s) are on a separate page, check for the availability of link(s) to allow the user to get to the other version.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G151)

</details>

<details>
  <summary>What abjective of setting amimated gif images to stop blinking after n cycles (within 5 seconds)?</summary>

The objective of this technique is to ensure that animated gif images stop blinking within five seconds. There are three aspects of the design of animated gif images that work together to determine how long the image blinks.

**Procedure:**

1. Display an animated gif and time how long it animates.
2. Alternatively, use an image editor to determine the number of frames, the frame rate, and the number of repetitions. Calculate the product of the number of frames multiplied by the frame rate times the number of repetitions. If frame rates are not uniform, calcuate the product of the sum of the frame rates multiplied by the number of repetitions.
3. Using either method, the duration of animation should be less than or equal to 5 seconds.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G152)

</details>

<details>
  <summary>What abjective of making the text easier to read?</summary>

The objective of this technique is to ensure that the text of the Web page is not difficult to read. Users with disabilities that make it difficult to decode words and sentences are likely to have trouble reading and understanding complex text. If the text does not require reading ability more advanced than the lower secondary education level, no supplements or alternative versions are needed.

**Procedure:**

1. Measure the readability of the text.
2. Check that the text requires reading ability less advanced than the lower secondary education level.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G153)

</details>

<details>
  <summary>What abjective of providing a checkbox in addition to submit button?</summary>

The objective of this technique is to provide a checkbox that users must select to indicate they have reviewd their input and are ready for it to be commited. This is important when the nature of the transaction is such that it may not be reversible if input errors are susequently discovered or when the result of an action is that data is deleted. The author provides a checkbox that is not selected when the page loads, with a label like "I confirm that the input is correct and am ready to submit" or "I confirm that I wish to delete this data". The checkbox should be located near the submitted, the input is rejected and the user is prompted to review their entry, select the checkbox, and resubmit. Only if the checkbox is selected will the input be accepted and the transaction processed.

**Procedure:**

1. Check that a checkbox indication user confirmation of the input or action is provided in addition to the submit button.
2. Check tha if the checkbox is not selected when the form is submitted, the inptu is rejected and the user is prompted to review their entry, select the checkbox, and resubmit.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G155)

</details>

<details>
  <summary>What abjective of using a technology that has commonly-available user agents that can change the foreground and background of blocks of text?</summary>

Some people with cognitive disabilities require specific color combinations of foreground text and background to help them successfully understand the contents of the Web page. Most popular browsers provide the option to change colors settings globally within the browser. In this case the colors selected by the user wverride the foreground and background colors specified byt the Web author.

In order to meet this success criterion, the Web author would design the page so that it works with browsers that have these controls, and the author does not override these controls.

**Procedure:**

1. Open the Web page in a browser that allows users to change colors of HTML content.
2. Change the foreground and background colors in the browser settings so they are different than those specified in the content.
3. Return to the page and check that the new specified foreground text and background colors in the browser override the colors specified in the content.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G156)

</details>

<details>
  <summary>What abjective of incorporationg a live audio captioning service into a Web page?</summary>

The objective of this technique is to use a real-time caption service to provide a text version of live audio content. Such services use a trained human operator who listens in to what is being said and uses a special keyboard to enter the text with only a small delay. They are able to capture a live event with a high degree of fidelity, and also to insert notes on any non spoken audio which is essential to understanding the event. The viewport containing the caption text is available on the same Web page as the live audion conent.

**Procedure:**

1. Check that the Web page contains a viewport associated with the live audion content.
2. Check that the text of the live audion content appears in the viewport with less than 30 seconds delay.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G157)

</details>

<details>
  <summary>What abjective of providing an alternative for time-based media for audio-only content?</summary>

The purpose of this technique is to provide an accessible alternative way of presenting the information in an audio-only presentation.

**Procedure:**

1. View the audio-only content while referring to the alternative for time-based media.
2. Check that the dialogue in the transcript matches the dialogue and information presented in the audio-only presentation.
3. If the audio includes multiple voices, check that the transcript identifies who is speaking for all dialogue.
4. Check that at least one of the following is true:

- The transcript itself can be programmatically determined from the text alternative for the audio-only content.
- The transcript is referred to from the programmatically determined text alternative for the audio-only content.

5. If the alternate version(s) are on a separate page, check for the availability of link(s) to allow the user to get to the other versions.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G158)

</details>

<details>
  <summary>What abjective of providing an alternative for time-based media for video-only content?</summary>

The purpose of this technique is to provide an accessible alternative way of presenting the information in a video-only presentation.

**Procedure:**

1. View the video-only content while referring to the alternative for time-based media.
2. Check that the information in the transcript includes the same information that is in the video-only presentation.
3. If the video includes multiple people or characters, check that the transcript identifies which person or character is associated with each action described.
4. Check that at least one of the following is true:

- The transcript itself can be programmatically determined from the text alternative for the video-only content.
- The transcript is referred to from the programmatically determined text alternative for the video-only content.

5. If the alternate version(s) are on a separate page, check for the availability of link(s) to allow the user to get to the other versions.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G159)

</details>

<details>
  <summary>What abjective of providing sign language versions of information, ideas, and processes that must be understood in order to use the content?</summary>

For some people who are deaf or have certain congnitive disabilities, sign language may be their first language. A sign language version of the page may be easier for them to understand than a written language version. The objective of this technique is to provide sign language content is provided in addition to the text.

**Procedure:**

1. Identify text that discusses ideas or processes that must be understood in order to use the content.
2. Check if sign language supplements to the text are available in the content or through links within the content.
3. Check that the sign language supplements show the concepts or processes discussed in the text.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G160)

</details>

<details>
  <summary>What abjective of providing a search function to help users find content?</summary>

Providing a search function that searches your Web pages is a design strategy that offers users a way to find content. Users can locate content by searching for specific words or phrases, without needing to understand or navigate through the structure of the Web site. This can be a quicker or easier way to find content, particularly on large sites.

**Procedure:**

1. Check that the Web page contains a search form or a link to a search page.
2. Type text into the search form that occurs in the set of Web pages.
3. Activate teh search.
4. Check taht the user is taken to a page that contains the search term.
5. Check that the user is taken to a page that contains a list of linsk to pages containing the serch term.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G161)

</details>

<details>
  <summary>What abjective of positioning labels to maximize predictability of relationships?</summary>

When labels for form fields are positioned where the user expects them visually, it is easier to understand complex forms and to locate specific fields. Labels for most fields are positioned immediately before the field, that is, for left-to-right languages, either to the left of the fields or above it, and for right-to-left languages, to the right of the field or above it. Labels for radio buttons and checkboxes are positioned after the field.

**Procedure:**

1. Check that the form field has a visible label.
2. If the form field is a checkbox or radio button, check that the label is immediately after the field.
3. If the form field is not a checkbox or radio button, check that the label is immediately before the field.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G162)

</details>

<details>
  <summary>What abjective of using standard diacritical marks that can be turned off?</summary>

The objective of this technique is to provide users with a mechanism turning standard diacritical marks on or off.

**Procedure:**

1. Check that the default version of the content users diacritical marks.
2. Check that there is a mechamism to turn diacritical marks on or off.
3. Check that using the mechanism to turn off diactirical marks results in content that does not display diacritical marks.
4. Check that using the mechanism to turn on diacritical marks results in content that displays diacritical marks.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G163)

</details>

<details>
  <summary>What abjective of providing a stated time within which an online request (or transaction) may be amended or canceled by the user after making the request?</summary>

The objective of this technique is to allow users to recover from errors made when placing an order by providing them with a period of time during which they can cancel or change the order. In general, a contract or an order is a leagal commitment and cannot be canceled. However, a Web site may choose to offer this capability, and it provides a way for users to recover from errors.

**Procedure:**

1. Check that the Web page describes the time period to cancel or change an order.
2. Check that the Web page describes the process for canceling or changing an order.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G164)

</details>

<details>
  <summary>What abjective of using the default focus indicator for the platform so that high visibility defautl focus indicators will carry over?</summary>

Operating systems have a native indication of focus, which is available in many user agents. The default rendering of the focus indicator isn't always highly visible and may even be difficult to see against certain backgrounds. However, many platforms allow the user to customize the rendering of this focus indicator. Assistive technology can also change the appearance of the native fucus indicator. If you use the native focus indicator any system-wide settings for its visibility will carry over to the Web page. If you draw your own focus indicator, for example by coloring sections of the page in response to user action, these settings will not carry over, and AT will not usually be able to find your focus indicator.

**Procedure:**

1. Use the features of your platform to customize the appearacne of the focus indicator.
2. Tab through the page, nothing the path of the focus.
3. Check that hte focus indicator for each control is visible.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G165)

</details>

<details>
  <summary>What abjective of providing audio that describes the important video content and describinig it as such?</summary>

Video-only content is inaccessible to people who are blind and to some who have low vision. Therefore, it is important for them to have an audio alternative. One way of doing this is to provide an audio track describing the information in the video. The audio should be a common audio format used on the internet. such as MP3.

**Procedure:**

1. Check that there is link to an audio alternative which describes the contents of the video immediately before or after the video-only content.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G166)

</details>

<details>
  <summary>What abjective of using an adjacent button to label the purpose of a field?</summary>

When a button invokes a function on an input field, has a clear text label, and is rendered adjacent to the input field, the button also acts as a label for the input field. This label helps users understand the purpose of the field without introducing repetive text on the Web page. Buttons that label single text fields typically follow the input field.

**Procedure:**

1. Check that the field and button are adjacent to one another in the programmatically determined reading sequence.
2. Check that the field and button are visually rendered adjacent to one another.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G167)

</details>

<details>
  <summary>What abjective of requesting confirmation to continue with selected action?</summary>

The abjective of the technique is to seek confirmation from the user that the selected action is their intended action. Use this technique in situations where the action can not be undone after it has been followed through. This will help users avoid submitting a form or deleting data by mistake.

**Procedure:**

1. Initiate the action that can not be reversed or changed.
2. Check that a request to confirma the selected actions is presented.
3. Check that the action can be confirmed and canceled.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G168)

</details>

<details>
  <summary>What abjective of aligning text on only one side?</summary>

Many people with cognitive disabilities have a great deal of trouble with blocks of text that are justified (aligned to both the left and the right margins). The spaces between words create "rivers of white" running down the page, which can make the text difficult for some people to read. This failure describes situatios where this confusing text layout occurs. The best way to avoid this problem is not to create text layout that is fully sustified.

**Procedure:**

1. Open the page in a common browser.
2. Verify that content is not justified (aligned to both the left and the right margins).

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G169)

</details>

<details>
  <summary>What abjective of providing a control near the beginning of the Web page that turns off sounds that play automatically?</summary>

The intent of this technique is to allow a user to turn off sounds that start automatically when a page loads. The control to turn off the sounds should be located near the beginning of the page to allow the control to be easily and quickly discovered by users. This is useful for those who utilize assistive technologies and those who may not.

**Procedure:**

1. Load a Web page.
2. Check for music or sounds that start automatically.
3. Check that a control that allows the user to turn off the sounds is provided near the beginning of the page.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G170)

</details>

<details>
  <summary>What abjective of playing sounds only on user request?</summary>

The intent of this technique is to allow a user to control the user of sounds in Web content. Someone that uses a screen reader may find it very distracting and difficult to listen to their screen reader if there are also sounds coming from Web content. Providing a way to play sounds only upon request will give a user the control needed to listen to any sounds or other audio without interfering with the output from a screen reader.

**Procedure:**

1. Load a Web page.
2. Check that no sounds play automatically.
3. Check that there is a way for a user to start sounds manually.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G171)

</details>

<details>
  <summary>What abjective of providing a mechanism to remove full justification of text?</summary>

The objective of this technique is to provide a version of the page that does not have full justification (justified both left and right).

**Procedure:**

1. Open a page with full justification.
2. Check that there si a feature to remove the full justification.
3. Check that the feature removes the full justification.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G172)

</details>

<details>
  <summary>What abjective of providing a version of a movie with audio descriptions?</summary>

The objective of this technique is to provide a second version of video content that provides audio descriptions so that it is possible for people who cannot see to be able to understand audio-visual material.

**Procedure:**

1. Open the version of the media that includes audio description.
2. Listen to the movie.
3. Check to see if gaps in dialogue are used to convey importatn information regarding visual content.
4. If the alternate version(s) are on a separate page, check for the availability of link(s) to allow the user to get to the other versions.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G173)

</details>

<details>
  <summary>What abjective of providing a control with a sufficient contrast ratio that allows users to switch to a presentation that uses sufficient contrast?</summary>

When the contrast between the text and its background for some portion of the page has not been designed to meet the contrast level for Success Criterion 1.4.3 or 1.4.6, it is possible to meet these guidelines using the "Slternate Version" clause in the conformance requirements. A link or control on the page can either change the page so that all aspects conform, or it could take the viewer to a new version of the page that does conform at the desired level. Placing the link or control prominently on the page will assist users in accessing the conforming content readily.

**Procedure:**

1. Check that a link or control exists on the original page that provides access to the alternate version.
2. Check that the link or control on the original page conforms to all success criteria for the conformance level being tested.
3. Check that the alterante version meets the contrast and all other success criteria for the conformance level being tested.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G174)

</details>

<details>
  <summary>What abjective of providing a multi color selection tool on the page for foreground and background colors?</summary>

The objective of this technique is to include a control on a Web page or set of Web pages that allows users to specify preferred foreground and background colors for the content. This technique can be implemented using any technology that allows users to store preferences that can be used across pages. Using this technique, and author includes a color picker control on the site which allows users to select and save foreground and background color preferences for use on other pages in a site pages are designed to look for these preferences and adapt accordingly when saved settins are found.

**Procedure:**

1. Check that there is a control on the page that is identified as a color selection tool.
2. Check that the color selection tool provides a variety of colors choices for the text and background.
3. Select new colors for the text and background using the tool.
4. Check that the content is updated to use the selected color combinations.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G175)

</details>

<details>
  <summary>What abjective of keeping the flashing area small enough?</summary>

The purpose of this technique is to provide and easy way to pass the success criterion for things that flash, but are small.

**Procedure:**

1. The small safe area is calculated.
2. Check taht only one area of the screen is flashing at any time.
3. Check that the floshing content would fit inot a contiguous container whose are is less than the small safe area.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G176)

</details>

<details>
  <summary>What abjective of providing suggested correction text?</summary>

The objective of this technique is to suggest correct text where the information supplied by the user is not accepted and possible correct text is known. The suggestions may include correct spelling or similar text from a known pool of possible text.

**Procedure:**

1. Identify form fields where correct text could be inferred from incorrect text.
2. Fill out the form, deliberately filling in the identified form fields with incorrect text.
3. Check that the user is presented with suggestions for the correct text.
4. Check that teh suggestion s are provided next to the form field or a link to the suggestions is provided close to the form field.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G177)

</details>

<details>
  <summary>What abjective of providing controls on the Web page that allow users to incrementally change the size of all text on the page up to 200 percent?</summary>

The purpose of this technique is to provide a mechanism on the Web page to incrementally increase the size of text. Many people with low vision do not use magnifying software, and they may not be familiar with their browser's text size adjustments. This may be particularly true of older people who are learning about computers later in life and who may be experiencing age related vision loss. It may also be true of some people with cognitive disabilities who require increased font size.

**Procedure:**

1. Set the viewport size to 1024px by 768px or lrger.
2. Increase the text size and check to see if the text size incresed.
3. Check that the text size can be increased to 200% of the original size.
4. Check that after increaseing the text size to 200% of the original size, there is no loss of content or functionality.
5. Decrease the text size to its defautl value and check to see if it in fact returned to the default size.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G178)

</details>

<details>
  <summary>What abjective of ensuring that there is no loss of content or functionality when the text resizes and text containers do not chante their width?</summary>

Some user agent support changing the size of text without changing other dimensions of the text container. Loss of content or functionality can occur when the text overflows the space that was allocated for it. However, the layout properties may provide a way to continue to display the content effectively. The block sizes may be defined wide enough that the text does not overflow when resized by 200%. Thext amy wrap when it no longer fits within the block, and the block may be tall enough that all the text continues to fit in the block. The block may provide scrollbars when the resized text no longer fits.

**Procedure:**

1. Increase text size to 200%.
2. Check whetehr all content and functionality is available.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G179)

</details>

<details>
  <summary>What abjective of providing the user with a means to set the time limit to 10 times the defautl time limit?</summary>

The objective of this technique is to give people with disabilities enough time to complete tasks which may take them longer than someone without those challenges. Some mechanism such as a preference setting or a control on the page lets the user change the time limits to at least 10 times the default time limit. Preferably the mechanism would have a vairable adjustment that lets the user change the time limit to any value in its range but could also provide ways to change time limit by discrete increments. The user chagne s the time limit at the beginning of their session, before any activity that has time limit.

**Procedure:**

1. Check to see if there is a mechanism to set the time limit to 10 times the default time limit.
2. Change the time limit to a new value that is 10 times the default time limit.
3. Perform an action that has a time limit has passed.
4. Wait unitl the default time limit has passed.
5. Check that the time limit does not expire until the limit specified in step 2 has passed.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G180)

</details>

<details>
  <summary>What abjective of encoding user data as hidden or encrypted data in a re-authorization page?</summary>

Web servers that require user quthentication often terminate the session after a set period of time if there is no activity from the user. If the user is unable to input the data quickly enough and the session times out before they submit, the server will require re-authentication before proceeding. When this happens, the server passes (as hidden data) the information from the form into the page that is used for re-authentication. Then, when the user re-authenticates, the server can use the infromation passed on from the re-authentication. Then, when the user re-authenticates, the server can use the information passed on from the re-authentication page to submit the form directly or to present a page that includes the data that is to be submitted for review. In this technique, the server does not have to store any user-submitted data on server. This is an important technique for those cases where it is either illegal or a security risk for the server to store information temporarily. It also is useful in that it frees the server from having to maintain the stored infroamtion and reconnect it with the newly authenticated session.

**Procedure:**

1. Log in and begin the timed activity.
2. Allow the session to time out.
3. Submit the data.
4. Re-authenticate.
5. Check that the process can continue and be completed without loss of data, including the original data and any changes made after re-authentication.
6. Check that the process used to save the information submitted in step 3 is not stored on the server.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G181)

</details>

<details>
  <summary>What abjective of ensuring that additional visual cues are available when text color differences are used to convey information?</summary>

The intent of this technique is to provide a redundatn visual cue for users who may not be able to discern a difference in text color. Color is commonly used to indicate the different status of words that are part of a paragraph or other block of text or where special characters or graphics cannot be used to indicate which words have special status. For example, scattered words in text may be hypertext links that are marked as such by being printed in a different color. This technique describes a way to provide cues in addition to color so that users who may have difficulty perceiving color differences or have low vision can identify them.

**Procedure:**

1. Locate all instances where the color of text is used to convey information.
2. Check that any text where color is used to convey information is also styled or uses a font that makes it visually distinct from other text around it.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G182)

</details>

<details>
  <summary>What abjective of using a contrast ratio of 3:1 with surrounding text and providing additional visuzl cues on hover for links or controls where color alone is used to identify them?</summary>

The intent of this technique is to provide a redundatn visual cue for users who may not be able to discern a difference in text color. Color is commonly used to indicate words that are links within a paragraph or ohter block of text. For example, scattered words in text may be hypertext links that are identified only by a difference in color with surrounding text. This technique describes a way to provide a difference in contrast rather than relying on hue.

**Procedure:**

1. Check that the relative luminance of the color of the text differs from the relative luminance of the surrounding text by a contrast ratio of at least 3:1.
2. Check that hovering over the link causes a visual enhancement.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G183)

</details>

<details>
  <summary>What abjective of providing text instructions at the beginning of a form or set of fields that describes the necessary input?</summary>

The objective of this technique is to help the user avoid input errors by informing them ahead of thime about restrictions of the format of data that they must enter. Instructions on such restictions are provided at the top of forms. This technique works best for forms that have a small number of fields or those where many form fields require data in the same format. In these cases, it is more efficient to describe the format once in instructions at the top of the form rather than repeating the same information for each field that has the same resticted format requirement.

**Procedure:**

1. Identify form controls that will only accept user input data in a given format.
2. Determine if instructions are provided at the top of the form about the expected format of each of the form controls identified in 1.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G184)

</details>

<details>
  <summary>What abjective of linking to all of the pages on the site from the home page?</summary>

The objective of this technique is to make it possible for users to locate all the information in a small Web site by providing links to all Web pages from the home page. When the number of pages in the site is small enough, the home page can contain site map infromation directly. The other pages in the Web site contain links to the home page.

**Procedure:**

1. Check that the home page contains links to all other pages in the Web site.
2. Check taht all other pages in the Web site contain links to the home page.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G185)

</details>

<details>
  <summary>What abjective of using a control in the Web page that stops moving, blinking, or auto-updating content?</summary>

The objective of this technique is to provide the user a control the allows him to stop moving or blinking content. Since the control is in the web page, the control itself meets the appropriate level of WCAG conformance e.g., it has appropriate contrast, it has a name that identifies it , it is keyboard accessible. The control is either at the top of the page or adjacent to the moving content. A single control may stop all moving or blinkign content on the page, or there may be separate controls for separate parts of the content.

**Procedure:**

1. Check that there is a control on the Web page to stop the motion.
2. Activate the control.
3. Check that the motion, blinking or auto updating has stopped.

[More >>](https://www.w3.org/WAI/WCAG22/Techniques/css/G186)

</details>
