# Scheme Interpreter

This project is a minimalistic interpreter for a subset of the Scheme programming language. The specific portion of Scheme handled is outlined in the [functional programming section of Composing Programs](#), with reference to our [language specification](#) and [built-in procedure documentation](#).

## Features

- **Read-Eval-Print Loop (REPL)**: Enter Scheme expressions and see them evaluated.
- **File Loading**: Load Scheme files with `(load 'filename)`.
- **Case-Insensitive**: Scheme identifiers in this interpreter are case-insensitive.

## Getting Started

### Prerequisites

- Python 3.x

### Running the Interpreter

To start the REPL, run:

```shell
python3 scheme.py
```

To exit, press Ctrl-d (Mac/Linux) or Ctrl-z Enter (Windows), or evaluate (exit) as follows:

```shell
scm> (exit)
```

To evaluate expressions from a file:

```shell
python3 scheme.py tests.scm
```

The tests.scm file contains a long list of sample Scheme expressions and their expected values. 

## Files

- `scheme_eval_apply.py`: The recursive evaluator for Scheme expressions.
- `scheme_forms.py`: Handles evaluation for special forms.
- `scheme_classes.py`: Contains classes that describe Scheme expressions.
- `questions.scm`: Scheme procedures that you need to implement.
- `scheme.py`: The interpreter's Read-Eval-Print Loop (REPL).
- `pair.py`: Defines the Pair class and the nil object, which is the empty list in Scheme.
- `scheme_builtins.py`: Built-in Scheme procedures are defined here.
- `scheme_reader.py`: Reads Scheme input.
- `scheme_tokens.py`: Tokenizer for Scheme input.
- `scheme_utils.py`: Utility functions for inspecting Scheme expressions.
- `ucb.py`: Utility functions for use in CS61A projects.
- `tests.scm`: A collection of test cases written in Scheme.
- `ok`: The autograder for the project.
- `tests`: A directory containing additional tests used by `ok`.
- `mytests.rst`: A file where you can add your own tests.

## Acknowledgments

This project is available thanks to:
- **The Scheme language and its community**
- **Structure and Interpretation of Computer Programs (CS61A) at UC Berkeley**
