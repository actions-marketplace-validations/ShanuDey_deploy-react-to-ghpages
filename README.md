## Deploy React app to gh-pages 

This Action will automate the process of building and deploying react app to gh-pages.

## Action 
Add this action inside your Repository's Actions

```
name: React app deployment

on:
  push:
    branches: [ master ]

jobs:
  build:
    runs-on: ubuntu-latest
    
    steps:
    - uses: actions/checkout@v2

    - name: Deploy react application to github pages with gh-pages
      uses: ShanuDey/deploy-react-to-ghpages@v1.0

```
