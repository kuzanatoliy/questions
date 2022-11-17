# JavaScript patterns

<details>
  <summary>What is an Immediately Invoked Function Expression (IIFE)?</summary>

An IIFE is a JavaScript function that runs as soon as it is defined. The name IIFE is promoted by Ben Alman in his blog.

The use cases:

1. *Avoid polluting the global namespace* - Because our application could include many functions and global variables from different source files, it's important to limit the number of global variables. If we have some initiation code that we don't need to use again, we could use the IIFE pattern. As we will not reuse the code again, using IIFE in this case is better than using a function declaration or a function expression.

        (() => {
          // some initiation code
          let firstVariable;
          let secondVariable;
        })();

2. *Execute an async function* - An async IIFE allows you to use await and for-await even in older browsers and JavaScript runtimes that have no top-level await:

        const getFileStream = async (url) => {
          // implementation
        };

        (async () => {
          const stream = await getFileStream("https://domain.name/path/file.ext");
          for await (const chunk of stream) {
            console.log({ chunk });
          }
        })();

3. *The module pattern* - We would also use IIFE to create private and public variables and methods. For a more sophisticated use of the module pattern and other use of IIFE, you could see the book Learning JavaScript Design Patterns by Addy Osmani.

        const makeWithdraw = (balance) =>
          ((copyBalance) => {
            let balance = copyBalance; // This variable is private
            const doBadThings = () => {
              console.log("I will do bad things with your money");
            };
            doBadThings();
            return {
              withdraw(amount) {
                if (balance >= amount) {
                  balance -= amount;
                  return balance;
                }
                return "Insufficient money";
              },
            };
          })(balance);

[More >>](https://developer.mozilla.org/en-US/docs/Glossary/IIFE)

</details>
