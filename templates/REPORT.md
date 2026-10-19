# REPORT.md

Group: <name>   Members: <names>

## Part A -- Test types
For smoke, regression, and slow: define it, say when it runs, give two
bookstore-relevant examples.

1. Smoke Testing

**Definition:** Smoke testing is a quick test that checks whether the main features of an application work at a basic level.

**When it should run:** It should run after a new build or code change, especially after every push to the repository, to quickly identify major problems.
**Examples:**
1. Register a new bookstore customer.
2. Add a product to the shopping cart and complete a basic checkout.

2.Regression Testing

**Definition:** Regression testing checks whether existing functionality still works after code changes or bug fixes.

**When it should run:** It should run after fixing a bug and before releasing changes. A fast subset can run frequently, while the full regression suite can run before a release or in scheduled CI runs.

**Examples:**
1. Check that a previously fixed cart-total calculation bug has not returned.
2. Check that login still rejects an incorrect password after changing the user-registration code.

3. Slow Testing

**Definition:** Slow testing checks behaviour that requires substantial processing, large datasets, or many operations.

**When it should run:** It should run during scheduled test runs, before major releases, or when changes affect performance-sensitive features.

**Examples:**
1. Import tens of thousands of bookstore products and check that the import completes correctly.
2. Perform many cart operations and verify that the final cart contents and totals are correct.

## Part B -- Scenario classification
For each of the six scenarios: smoke / regression / slow (may be more than one)
with a 2-3 sentence justification.


## Part F -- Team reflection
1. Why is running only regression tests before every commit inefficient?
2. Why do smoke tests usually run first in a CI/CD pipeline?
3. What risks arise if slow tests are never run?
4. Can one test belong to two categories? Give an example.
5. Bug-finders and bug-fixers are often different people in a real QA team.
   What does that separation change about how a bug report must be written?
