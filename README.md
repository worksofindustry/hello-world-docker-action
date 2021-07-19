# Hello world docker action

This action prints "Hello World" or "Hello" + the name of a person to greet to the log.

## Inputs

## `who-to-greet`

**Required** The name of the person to greet. Default `"World"`.

## Outputs

## `time`

The time we greeted you.

## Example usage

uses: actions/hello-world-docker-action@v1
with:
  who-to-greet: 'Mona the Octocat'
  
####
action.yml file serves as an action metadata file. It defines the inputs and outputs and main
entrypoint for your action. 

workflow files use action files, workflow files that use an action, uses the "with" keyword to set an input values. 
Inputs specified in a workflow file, get created as an environment variable by GitHub, with the name ''INPUT_<VARIABLE_NAME>''.

