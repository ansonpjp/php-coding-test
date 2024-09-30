# Rave Build PHP Coding Test
Welcome to the Rave Build PHP Coding Test! 

### The brief
A lot of our product at Rave involves managing projects, and the tasks required to complete those projects.
This is reflected in this codebase, which is a few classes that represent some common functionality at Rave.

The supplied code + tests are old, incomplete and no-one has reviewed this code or the test cases. There is nothing 
that currently uses this code, so you are free to refactor it however you see fit without concern of breaking anything.

**Feel free to edit or create any files in this repository** as part of this exercise as you see fit.

Your objectives are:
1. Update/refactor/fix/add/remove/improve any file (including tests) ensuring all the tests pass and the code works as you would expect it to
2. Ensure that the code and tests meets a modern high standard (whatever that means to you)
3. Note down any choices or assumptions you made and why you made them in this README. For example, "I assumed Task names are not unique"
4. Note down what you would do if you had more time in this README. For example, "I would have added more tests to cover xyz... as I found the existing tests didn't cover the scenario when xyz..."
5. Delete the `vendor` directory, then zip this directory and email it to us

We expect this test should take 1-2 hours to complete.

## Installation
PHP installations are quite complicated, so we have Dockerised the 
dependencies for this test in an attempt to simplify getting it running.
You need to:

1. Clone this Git repository
2. Install [Make](https://www.gnu.org/software/make/). For Windows
   [follow one of these instructions](https://stackoverflow.com/a/32127632).
   For MacOS, install with homebrew like `brew install make`. For Linux, use 
   your package manager like `apt install make`.
3. Install Docker. For Windows and MacOS we recommend 
   [installing Docker Desktop](https://docs.docker.com/desktop/install/windows-install/). 
   For Linux distributions we recommend
   [installing the Docker Engine](https://docs.docker.com/engine/install/).
4. Check that Docker is working by running `docker run hello-world`.

## Running the tests
Run `make test` to run the PHPUnit tests in a Docker container.

## Running program.php
Run `make run` to execute `program.php`. It is not required, but we have provided 
it if you would like to just run PHP code to debug things.

## My notes
### Choices or assumptions I made and reasons why
* I assumed that task IDs are unique
* I assumed that getTask function is to return the name of the TASK if its exist, else return NULL

### Things I would do if I had more time
* I would have added code to handle duplicate task names, and to handle tasks with same name
* Handle tasks that needs to do synchronously and asynchronously (with dispatchable jobs)
* Check for existing IDs, and to overwriting existing task with same ID
* I would add more test cases such as test for updating a Task
* I would add validations when adding task such as ID is unique and name is not empty
* I would add proper documentation and comments so that each method and class is more readable
* I would add encapsulation and validations for Task.php and Project.php 
* Type decalarations will be added to each function
