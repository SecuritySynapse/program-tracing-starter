# 🔬 Program Tracing

[![build](../../actions/workflows/build.yml/badge.svg)](../../actions/)
![Platforms: Linux, MacOS, Windows](https://img.shields.io/badge/Platform-Linux%20%7C%20MacOS%20%7C%20Windows-blue.svg)
[![Language: Python](https://img.shields.io/badge/Language-Python-blue.svg)](https://www.python.org/)
[![Commits: Conventional](https://img.shields.io/badge/Commits-Conventional-blue.svg)](https://www.conventionalcommits.org/en/v1.0.0/)
[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)

## ✨ Table of Contents

<!---toc start-->

<!---toc end-->

## 🏁 Introduction

If you are a student completing this project as part of a class at Allegheny
College, you can check the schedule on the course web site for the due date or
ask the course instructor for more information about the due date. You can also
find the deadline for the project, as reported by GitHub Classroom, by clicking
the grey box at the top of this file. Please furthermore note that the content
provided in the `README.md` file for this GitHub repository is an overview of
the project and thus may not include the details for every step needed to
successfully complete every project deliverable. This means that you may need to
schedule a meeting during the course instructor's office hours to discuss
aspects of this project.

## 🤝 Seeking Assistance

Even though the course instructor will have covered all of the concepts central
to this project before you start to work on it, please note that not every
detail needed to successfully complete the assignment will have been covered
during prior classroom sessions. This is by design as an important skill that
you must practice as security engineer is to search for and then understand and
ultimately apply the technical content found in additional resources.

## 🛫 Project Overview

This project invites you to implement and use a program called `programtracer`
that can produce a detailed trace of a program's execution in the service of
automated malware analysis. As explained by CrowdStrike in the article entitled
[10 Malware Detection
Techniques](https://www.crowdstrike.com/en-us/cybersecurity-101/malware/malware-detection/),
there a several different, yet often complementary, techniques for detecting
malware of a system. This project invites you to explore more about **dynamic
malware analysis** where you will write a `programtracer` that will observe the
execution of a Python program and then record a program trace that a malware
analyst could study so as to better understand its behavior and to perhaps
extract a behavior signature that could be used to detect it in the future. The
`programtracer` should be able to perform a rudimentary analysis of a save trace
and compare two different traces that it previously produced.

## 🏁 Getting Started

After cloning this repository to your computer, please take the following steps
to get started on the project:

- Make sure that you are using a recent version of Python 3.12 to complete this
assignment by typing `python --version` in your terminal; if you are not using a
recent version of Python please upgrade before proceeding.
- Make sure that you are using a recent version of Poetry 1.8 to complete this
assignment by typing `poetry --version` in your terminal; if you are not using a
recent version of Poetry please upgrade before proceeding.
- Before moving to the next step, you may need to again type `poetry install`
one or more times in order to avoid the appearance of warnings when you next run
the `programtracer` program.

Please note that you are invited to complete all of the background research,
implementation, and experimentation needed to implement and use the
`programtracer`, as outlined further in the following subsections.

## 📚 Background Research

Your `programtracer` will take as input a Python program and/or a Python
program's test suite, and then produce a detailed trace of the program's
behavior. The trace should record all of the details about the specific
instructions that were run during the execution of the Python program. To learn
more about program tracing, please consult the following references organized
into the following technical categories:

- **Concepts**: Introduction to the technical concepts of program analysis and dynamic
malware analysis.
    - [10 Malware Detection
Techniques](https://www.crowdstrike.com/en-us/cybersecurity-101/malware/malware-detection/)
    - [What is a Malware Signature and How Does it Work?](https://www.sentinelone.com/blog/what-is-a-malware-file-signature-and-how-does-it-work/)
    - [Tracing Executions](https://www.debuggingbook.org/beta/html/Tracer.html)
    - [Tracking Failure Origins](https://www.debuggingbook.org/beta/html/Slicer.html)
- **Packages**: Built-in packages for program tracing in Python
    - [Python `sys`](https://docs.python.org/3/library/sys.html)
    - [Python `settrace`](https://docs.python.org/3/library/sys.html#sys.settrace)
    - [Python `monitoring`](https://docs.python.org/3/library/sys.monitoring.html)
    - [Python `trace`](https://docs.python.org/3/library/trace.html)
    - [Python `inspect`](https://docs.python.org/3/library/inspect.html)
    - [Python `dis`](https://docs.python.org/3/library/dis.html)
    - [Python `ast`](https://docs.python.org/3/library/ast.html)
- **Tools**: Tools for program tracing in Python
    - [`coverage.py`](https://github.com/nedbat/coveragepy)
    - [`line_profiler`](https://github.com/pyutils/line_profiler)
    - [`python-hunter`](https://github.com/ionelmc/python-hunter)
    - [`slipcover`](https://github.com/plasma-umass/slipcover)
    - [`scalene`](https://github.com/plasma-umass/scalene)

## 🚀 Implementation Details

After reading all of the background research and exploring the references that
the prior section provides, you should pick a small Python program and Pytest
test suite (perhaps even one that you wrote yourself) and attempt run it and
then produce a trace of each line of source code that the test suite ran in the
Python program. The trace that your tool produces should include all of the
executed instructions at the level of the abstract syntax tree (AST), the Python
source code, and/or the native code produced by the Python interpreter. Whenever
possible, the trace should also include the values of variables that were
accessed by each of the detected instructions. Finally, the trace should be
stored in a file in either a plaintext, comma-separated value (CSV), or
JavaScript object notation (JSON) format.

Once you have an implementation that is working for a small Python project, you
should create a complete implementation of the `programtracer` project, using
the `main.py` file to implement the command-line interface (CLI) for the
program. As you add features to your tool you should confirm that it works for
progressively larger Python programs and test suites. You should then implement
the following features into your `programtracer` tool:

- **Command-Line Interface**: The `programtracer` should have a command-line
that accepts the name of a Python program and/or a Python program's test suite
and then performs the program tracing when the tests run on the program.
- **Program Tracing**: The `programtracer` should trace the execution of a
Python program and save the trace in a suitable format in a specified directory
and file.
- **Variable Tracking**: The `programtracer` should track the values of
variables as they are referenced by the specific instructions in the program's
source code.
- **Trace Analysis**: The `programtracer` should be able to analyze the trace by
reporting information about, for instance, the number of instructions in the
trace, the number of times each instruction was executed, the number of times a
variable is accessed by instructions, and the number of unique values stored in
the variables accessed by the instructions.
- **Trace Comparison**: The `programtracer` should be able to compare two traces
and surface the similarities and differences between the them. This feature
would be useful in the context of malware analysis to compare the behavior of
a new program to a well-known malware program.

You should aim to implement all of these features as a part of your
`programtracer` tool. If you are not able to implement a specific feature, then
you must both document the steps that you took and explain why it was not possible to
implement a featured in `writing/reflection.md` file.

## 🎉 Experiment Details

## ✨ Additional Information

- If you have already installed the
[GatorGrade](https://github.com/GatorEducator/gatorgrade) program that runs the
automated grading checks provided by
[GatorGrader](https://github.com/GatorEducator/gatorgrader) you can, from the
repository's base directory, run the automated grading checks by typing
`gatorgrade --config config/gatorgrade.yml`.
- You may also review the output from running GatorGrader in GitHub Actions.
- Don't forget to provide all of the required responses to the technical writing
prompts in the `writing/reflection.md` file.
- Please make sure that you completely delete the `TODO` markers and their
labels from all of the provided source code. This means that instead of only
deleting the `TODO` marker from the code you should delete the `TODO` marker and
the entire prompt and then add your own comments to demonstrate that you
understand all of the source code in this project.
- Please make sure that you also completely delete the `TODO` markers and their
labels from every line of the `writing/reflection.md` file. This means that you
should not simply delete the `TODO` marker but instead delete the entire prompt
so that your reflection is a document that contains polished technical writing
that is suitable for publication on your professional web site.
