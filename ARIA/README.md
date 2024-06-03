# Aria

<details>
  <summary>What is aria?</summary>

The ARIA modifies the accessibility tree, modifying how assistive technology presents the content to your users. ARIA doesn't change anything about an element's function or behavior. When not using semantic HTML elements for their intended purpose and default functionality, you must use JavaScript to manage behavior, focus, and ARIA states.

</details>

<details>
  <summary>ARIA is for what?</summary>

It especially helps with dynamic content and advanced user interface controls developed with HTML, JavaScript, and related technologies. Without WAI-ARIA certain functionality used in Web-sites is not available to some users with disabilities, especially people who rely on screen readers and people who cannot use a mouse.

</details>

<details>
  <summary>Where ARIA is used?</summary>

There are three main components used in ARIA:

- Roles;
- States;
- Properties.

</details>

<details>
  <summary>When shouldn’t we use ARIA?</summary>

W3C actually created the Rules of ARIA Use to help to guide us in this question. There are five of them, starting with:

- Use native HTML at all times;
- Do not change native HTML semantics unless you absolutely have to;
- All interactive ARIA controls must be keyboard accessible;
- For all elements that are focusable, do not ever add role="presentation" or aria-hidden="true";
- All interactive elements must have an accessible name.

</details>

[Aria attributes](ARIA_ATTRIBUTES.md)

[Aria roles](ARIA_ROLES.md)
