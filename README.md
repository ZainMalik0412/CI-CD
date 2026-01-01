# CI-CD
Learning for CI/CD

name: CI push learning workflow # Name can be anything

on: [push] # When we push it will be picked up

jobs: 
    build:
        runs-on: ubuntu-latest
        steps: # Steps that actions that will run in the build, steps contains a list called name 
        - name: checkout code 
          uses: actions/checkout@v2 #reusable action
        - name: We are testing this workflow
          run: echo Hello everyone!