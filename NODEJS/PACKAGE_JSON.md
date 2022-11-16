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

<details>
  <summary>What are an author and a contributors properties?</summary>

The "author" is one person. "contributors" is an array of people. A "person" is an object with a "name" field and optionally "url" and "email", like this:

    {
      "name" : "Barney Rubble",
      "email" : "b@rubble.com",
      "url" : "http://barnyrubble.tumblr.com/"
    }

Or you can shorten that all into a single string, and npm will parse it for you:

    {
      "author": "Barney Rubble <b@rubble.com> (http://barnyrubble.tumblr.com/)"
    }

[More >>](https://docs.npmjs.com/cli/v9/configuring-npm/package-json#people-fields-author-contributors)

</details>

<details>
  <summary>What is a funding property?</summary>

It is possible to specify an object containing a URL that provides up-to-date information about ways to help fund development of your package, or a string URL, or an array of these:

    "funding": [
      {
        "type" : "individual",
        "url" : "http://example.com/donate"
      },
      "http://example.com/donateAlso",
      {
        "type" : "patreon",
        "url" : "https://www.patreon.com/my-account"
      }
    ]

[More >>](https://docs.npmjs.com/cli/v9/configuring-npm/package-json#funding)

</details>

<details>
  <summary>What is a files property?</summary>

The optional files field is an array of file patterns that describes the entries to be included when your package is installed as a dependency. File patterns follow a similar syntax to .gitignore, but reversed: including a file, directory, or glob pattern (*, **/*, and such) will make it so that file is included in the tarball when it's packed. Omitting the field will make it default to ["*"], which means it will include all files.

[More >>](https://docs.npmjs.com/cli/v9/configuring-npm/package-json#files)

</details>

<details>
  <summary>What is a main property?</summary>

The main field is a module ID that is the primary entry point to your program. If main is not set it defaults to index.js in the package's root folder.

[More >>](https://docs.npmjs.com/cli/v9/configuring-npm/package-json#main)

</details>

<details>
  <summary>What is a browser property?</summary>

If a module is meant to be used client-side the browser field should be used instead of the main field. This is helpful to hint users that it might rely on primitives that aren't available in Node.js modules.

[More >>](https://docs.npmjs.com/cli/v9/configuring-npm/package-json#browser)

</details>

<details>
  <summary>What is a bin property?</summary>

To use this, supply a bin field in your package.json which is a map of command name to local file name. When this package is installed globally, that file will be either linked inside the global bins directory or a cmd (Windows Command File) will be created which executes the specified file in the bin field, so it is available to run by name or name.cmd (on Windows PowerShell). When this package is installed as a dependency in another package, the file will be linked where it will be available to that package either directly by npm exec or by name in other scripts when invoking them via npm run-script.

For example, myapp could have this:

    {
      "bin": {
        "myapp": "./cli.js"
      }
    }

[More >>](https://docs.npmjs.com/cli/v9/configuring-npm/package-json#bin)

</details>

<details>
  <summary>What is a man property?</summary>

Specify either a single file or an array of filenames to put in place for the man program to find.

If only a single file is provided, then it's installed such that it is the result from man pkgname, regardless of its actual filename. For example:

    {
      "name": "foo",
      "version": "1.2.3",
      "description": "A packaged foo fooer for fooing foos",
      "main": "foo.js",
      "man": "./man/doc.1"
    }

[More >>](https://docs.npmjs.com/cli/v9/configuring-npm/package-json#man)

</details>

<details>
  <summary>What is a directories property?</summary>

The CommonJS Packages spec details a few ways that you can indicate the structure of your package using a directories object. If you look at npm's package.json, you'll see that it has directories for doc, lib, and man.

[More >>](https://docs.npmjs.com/cli/v9/configuring-npm/package-json#directories)

</details>

<details>
  <summary>What is a repository property?</summary>

Specify the place where your code lives. This is helpful for people who want to contribute. If the git repo is on GitHub, then the npm docs command will be able to find you.

Do it like this:

    {
      "repository": {
        "type": "git",
        "url": "https://github.com/npm/cli.git"
      }
    }

[More >>](https://docs.npmjs.com/cli/v9/configuring-npm/package-json#repository)

</details>

<details>
  <summary>What is a scripts property?</summary>

The "scripts" property is a dictionary containing script commands that are run at various times in the lifecycle of your package. The key is the lifecycle event, and the value is the command to run at that point.

[More >>](https://docs.npmjs.com/cli/v9/configuring-npm/package-json#scripts)

</details>

<details>
  <summary>What is a config property?</summary>

A "config" object can be used to set configuration parameters used in package scripts that persist across upgrades. For instance, if a package had the following:

    {
      "name": "foo",
      "config": {
        "port": "8080"
      }
    }

It could also have a "start" command that referenced the npm_package_config_port environment variable.

[More >>](https://docs.npmjs.com/cli/v9/configuring-npm/package-json#config)

</details>

<details>
  <summary>What is a dependencies property?</summary>

Dependencies are specified in a simple object that maps a package name to a version range. The version range is a string which has one or more space-separated descriptors. Dependencies can also be identified with a tarball or git URL.

[More >>](https://docs.npmjs.com/cli/v9/configuring-npm/package-json#dependencies)

</details>

<details>
  <summary>What is a devDependencies property?</summary>

If someone is planning on downloading and using a module in their program, then they probably don't want or need to download and build the external test or documentation framework that you use. In this case, it's best to map these additional items in a devDependencies object.

[More >>](https://docs.npmjs.com/cli/v9/configuring-npm/package-json#devdependencies)

</details>
