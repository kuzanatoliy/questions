# Package json

<details>
  <summary>What is a name property?</summary>

It is name of your package. The property is optional for private projects, but it is required for public projects.

Rules:

- The name must be less than or equal to 214 characters. This includes the scope for scoped packages.
- The names of scoped packages can begin with a dot or an underscore.
- New packages must not have uppercase letters in the name.
- The name ends up being part of a URL, an argument on the command line, and a folder name. Therefore, the name can't contain any non-URL-safe characters.

[More >>](https://docs.npmjs.com/cli/v9/configuring-npm/package-json#name)

</details>

<details>
  <summary>What is a version property?</summary>

The version property contains version of a package. It is option for private projects, but it is required for public projects. Version must be parseable by node-semver, which is bundled with npm as a dependency.

[More >>](https://docs.npmjs.com/cli/v9/configuring-npm/package-json#version)

</details>

<details>
  <summary>What is a description property?</summary>

Put a description in it. It's a string. This helps people discover your package, as it's listed in npm search.

[More >>](https://docs.npmjs.com/cli/v9/configuring-npm/package-json#description)

</details>

<details>
  <summary>What is a keywords property?</summary>

Put keywords in it. It's an array of strings. This helps people discover your package as it's listed in npm search.

[More >>](https://docs.npmjs.com/cli/v9/configuring-npm/package-json#keywords)

</details>

<details>
  <summary>What is a homepage property?</summary>

The url to the project homepage.

Example:

    "homepage": "https://github.com/owner/project#readme"

[More >>](https://docs.npmjs.com/cli/v9/configuring-npm/package-json#homepage)

</details>

<details>
  <summary>What is a bugs property?</summary>

The url to your project's issue tracker and / or the email address to which issues should be reported.

Example:

    {
      "url" : "https://github.com/owner/project/issues",
      "email" : "project@hostname.com"
    }

[More >>](https://docs.npmjs.com/cli/v9/configuring-npm/package-json#bugs)

</details>

<details>
  <summary>What is a license property?</summary>

You should specify a license for your package so that people know how they are permitted to use it, and any restrictions you're placing on it.

Examples:

    {
      "license" : "BSD-3-Clause"
    }

    {
      "license" : {
        "type" : "ISC",
        "url" : "https://opensource.org/licenses/ISC"
      }
    }

[More >>](https://docs.npmjs.com/cli/v9/configuring-npm/package-json#license)

</details>
