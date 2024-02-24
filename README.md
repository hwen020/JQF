# JQF | Testing | Fuzz Testing | Test Input Generation | Coverage Information Analysis | Parallel Testing 
From https://github.com/rohanpadhye/JQF 
This is just an implementation of JQF. Please read the README.pdf. 

## 1. **Implementation Documentation:**

**Step 1: Download and set up JQF**
- **Substep 1.1:** Cloned the JQF repository from GitHub.
- **Substep 1.2:** Checked and ensured the installation of dependencies (JDK and Maven).
- **Substep 1.3:** Created a test file (`SimpleTest.java`) and inserted code.

**Step 2: Fuzz the PUT using JQF**
- **Substep 2.1:** Compiled the test file with essential dependencies.
- **Substep 2.2:** Ran `jqf-random` on the compiled bytecode for 10 iterations.

**Step 3: Print out coverages**
- **Substep 3.1:** Modified JQF source code to print branch decisions.
- **Substep 3.2:** Rebuilt JQF.
- **Substep 3.3:** Ran `jqf-random` on the compiled bytecode for 10 iterations.

**Step 4: Change test inputs and print coverages**
- **Substep 4.1:** Modified JQF source code to generate integer 200 for every iteration.
- **Substep 4.2:** Modified JQF source code to print trace events.
- **Substep 4.3:** Rebuilt JQF.
- **Substep 4.4:** Ran `jqf-random` on the compiled bytecode for 10 iterations.

**Result Documentation:**

**Step 2: Fuzz the PUT using JQF**
- **Substep 2.2:** Obtained generated inputs, execution time, and program process status.

**Step 3: Run jqf-random on the PUT bytecode for 10 iterations and print branch decisions**
- **Substep 3.3:** Printed out branch decisions for each event.

**Step 4: Run jqf-random on the PUT bytecode for 10 iterations and print branch decisions**
- **Substep 4.4:** Printed out branch decisions for each event.

**Potential Optimizations:**
1. **Parallel Fuzzing:**
   - Explore strategies for parallel fuzzing to enhance test coverage.
   - Utilize multiple instances of JQF running concurrently to expedite the fuzzing process.

2. **Customized Guidance Strategies:**
   - Experiment with various guidance strategies provided by JQF.
   - Develop or tailor guidance strategies specific to the program under test for more effective coverage.


## 2. The main functionalities of the program under test (PUT) using the JQF tool in the field of computer science are as follows:

1. **Fuzz Testing:**
   - JQF provides the capability of fuzz testing, which is a method to detect vulnerabilities and errors in a program by supplying random or semi-random input data. In this context, the PUT is the target of the fuzz testing.

2. **Test Input Generation:**
   - JQF generates test input data for running the PUT by executing the `jqf-random` command. This helps in testing the behavior of the program under different input conditions.

3. **Coverage Information Analysis:**
   - JQF is modified to print the branch decision information of the program, i.e., the decision points during execution. This aids in understanding the program's execution paths and coverage.

4. **Optimization Exploration:**
   - JQF is modified to experiment with different optimization strategies, such as altering the generation of test inputs or printing additional debugging information. This helps in evaluating the impact of different strategies on the program's performance and behavior.

5. **Parallel Testing:**
   - The potential optimization strategies include exploring parallel fuzz testing to enhance test coverage. This involves utilizing multiple instances of JQF running concurrently to expedite the fuzz testing process.

In summary, JQF's functionalities in the field of computer science primarily revolve around testing and optimizing programs. It employs fuzz testing techniques to discover potential issues and enhances testing depth and efficiency through coverage analysis and experimentation with various optimization strategies.
