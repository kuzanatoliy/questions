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
