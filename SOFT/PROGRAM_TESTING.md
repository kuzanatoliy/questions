# Program testing

### Links

### Questions

<details>
  <summary>What are whitebox and blackbox testing?</summary>

The sense of the type of testing is in knowledge about implementation. So if we write tests without knowledge about implementation it is black box testing and whitebox is opposite case.

</details>

<details>
  <summary>How fixing errors?</summary>

1. Determine the real class of tests on which the error manifests itself. You may have found a bug while checking the corner case, but it actually affects a wider class of tests.
2. Understand why the error occurs, and eliminate its cause.
3. Verify that the problem has indeed been fixed. To do this, you need to carefully check the test on which the previous version of the solution broke.
4. Make sure other cases don't break. Check invariants, figure out which tests potentially affect code changes, and look only at them.

</details>
