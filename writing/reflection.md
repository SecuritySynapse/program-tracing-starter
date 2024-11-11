# Program Tracing

## Add Your Name Here

## Re-type the sentence "I adhered to the Allegheny College Honor Code while completing this project."

TODO: You must retype the sentence here in order to digitally sign your pledge.

**IMPORTANT:** If you do not type the required sentence then the course
instructor will not know that you adhered to the Allegheny College Honor Code
while completing the project.

## Program Selection

TODO: Please provide a list of the **names** and **GitHub repositories** for the
five projects that you used as subjects to conduct your program tracing
experiment. Importantly, please note that these subjects need to be executed
either through your interactive use of the program (i.e., through its web
interface, command-line interface, or text-based interface) or through its test
suite. You cannot use projects that you created for a class at Allegheny College;
you must use real-world projects created by external software developers.

_Reminder: Select diverse programs to ensure a comprehensive evaluation._

## Run the `programtracer` Tool

TODO: Execute the `programtracer` tool on each of the selected Python programs
and its test suite. Ensure that the tool generates a trace file in the specified
format (i.e., plaintext, CSV, or JSON). Create a directory called `traces` and
save all of your trace files in this directory. Make sure that it is clear which
of the five projects you used as subjects to conduct your program tracing
resulted in each of the trace files.

_Reminder: Verify that the trace files are generated correctly for each program._

## Verify the Trace Output

TODO: For each selected program and its test suite, manually inspect the
majority of the trace file in the `traces` directory to verify that it
accurately records the program's execution. Check that the trace includes
details such as executed instructions, variable values, and any other relevant
runtime information. Provide a checklist of the steps that you followed to
verify the trace output, indicating whether or not you were able to verify the
trace output at each step.

_Reminder: Ensure the trace files are accurate and complete._

## Analyze the Traces

TODO: Using Markdown tables, for each selected program and its test suite,
use the `programtracer` tool's analysis features to gather information about the
trace. This includes:
    - The number of instructions in the trace.
    - The number of times each instruction was executed.
    - The number of times variables were accessed by instructions.
    - The number of unique values stored in the variables accessed by the instructions.

_Reminder: Document the analysis results for each program._

## Compare Traces

TODO: After making a change to the source code of each Python program, run the
`programtracer` tool on it. Manually compare the traces that arise from this
modified program and the original to identify the similarities and differences
in their execution behavior. Provide excerpts of the program traces and an
analysis of them to confirm whether or nor your `programtracer` tool can
surface enough information that would help you to characterize the differences
in program behavior.

_Reminder: Highlight key differences and similarities in the traces._

## Efficiency Analysis

TODO: For each selected program and its test suite, time the execution of the
`programtracer` tool when it is completing tasks such as creating the trace,
saving the trace, and analyzing the trace. Using Markdown tables, record the
size of the trace files when stored in memory and on disk.

_Reminder: Record performance metrics and trace file sizes._

## Analyze Results

Summarize the findings from the experiments in this report. The report should include:
    - An overview of the selected Python program and test suite.
    - A description of the trace output and its verification.
    - Results from the trace analysis, including any notable patterns or insights.
    - A comparison of different traces, highlighting key differences.
    - Efficiency analysis results, including performance metrics and trace file sizes.
    - Any challenges encountered during the experiment and how they were addressed.
    - The lessons learned from conducting this experiment with the `programtracer` tool.

_Reminder: Provide a comprehensive summary of your findings and insights._

### Take Home Points

TODO: Provide a two to three sentence statement about the key takeaways from
conducting this experiment. Please note that the course instructor will display
some student takeaways on the course web site and use them to facilitate
follow-on discussions during the class and laboratory sessions.

_Reminder: Clearly summarize the key takeaways from this security survey project._
