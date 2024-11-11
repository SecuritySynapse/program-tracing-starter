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
there a several different, often complementary techniques for detecting malware
of a system. This project invites you to explore more about **dynamic malware
analysis** where you will write a `programtracer` that will observe the
execution of a Python program and then record a program trace that a malware
analyst could study so as to better understand its behavior and to perhaps
extract a behavior signature that could be used to detect it in the future.

### Features


### Getting Started

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

### Additional Information

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
