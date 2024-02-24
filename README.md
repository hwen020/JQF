# From https://github.com/rohanpadhye/JQF 
This is just an implementation of JQF. Please read the README.doc. 

**Implementation Documentation:**

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
