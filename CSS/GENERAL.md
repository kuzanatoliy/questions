# CSS

### Links

[Scrollbar](https://developer.mozilla.org/en-US/docs/Web/CSS/::-webkit-scrollbar)

### Questions

<details>
  <summary>Is it possible to use non-blocking CSS?</summary>

Yes, styles that are not critical on the loading step could be moved on a separate file and involved by print media. The loading of the CSS styles is non-blocked. So, it is possible to change the media type to all after loading.

</details>

<details>
  <summary>Is it possible to customize scrollbar?</summary>

Yes, it is possible to use the follow scrollbar selectors:

| Selector                        | Description                                                                                                                                         |
| ------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| ::-webkit-scrollbar             | the entire scrollbar                                                                                                                                |
| ::-webkit-scrollbar-button      | the buttons on the scrollbar (arrows pointing upwards and downwards that scroll one line at a time)                                                 |
| ::-webkit-scrollbar-thumb       | the draggable scrolling handle                                                                                                                      |
| ::-webkit-scrollbar-track       | the track (progress bar) of the scrollbar, where there is a gray bar on top of a white bar                                                          |
| ::-webkit-scrollbar-track-piece | the part of the track (progress bar) not covered by the handle                                                                                      |
| ::-webkit-scrollbar-corner      | the bottom corner of the scrollbar, where both horizontal and vertical scrollbars meet. This is often the bottom-right corner of the browser window |
| ::-webkit-resizer               | the draggable resizing handle that appears at the bottom corner of some elements                                                                    |

</details>
