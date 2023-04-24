# LAB REPORT 2
## PART I

## PART II
A failure-inducing input for the method `reversed` would be
`@Test
  public void testReversed() {
    // test 1
    int[] input2 = {2,1,4};
    assertArrayEquals(new int[]{4,1,2}, ArrayExamples.reversed(input2));
  }`
### PART III
In the week 3 lab, I learned a lot about debugging and utilizing JUnit tests. Debugging is the process of finding errors in your code, and 
removing said errors by editing the code. JUnit is a java library that is used run tests. In the lab, we used tests such as `assertArrayEquals` to test
our methods. I learn best by practicing, so fixing the code/writing tests for the methods `reverseInPlace` and `reversed` helped me understand
the process of debugging. I also feel more comfortable with writing JUnit tests. Before this lab, I didn't know that JUnit tests are written in
a different class from the methods being tested, and that an `@Test` annotation is required before a void test method.
