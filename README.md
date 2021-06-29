# Mixd GitHub Actions Workflow
This GitHub Action Workflow has been created by Mixd as a step towards leveraging the advantages of CI/CD.

It has been designed around our in-house NHS WordPress framework so may not always be appropriate for your use case.

## What does it do?
When you push to the primary branch of your repository it will first run a PSR-12 Compliance check against your WordPress theme and then will also install your Composer and NodeJS dependencies and ensure that your static assets can be built. 

## How do I use it?

To use this GitHub Action Workflow, start of by creating a new folder in the root of your project called `.github`, and inside that folder create another folder called `workflows`.

Download a copy of the `/workflow-templates/build.yml` file from this repository and add it to your `workflows` folder.

It should look like this:

```
<root>
| .github/
|____ workflows/
|________ build.yml
```

Edit the `build.yml` file and replace the `$default-branch` with the name of your default branch. For recently created repos this is typically `main` otherwise it may be `master`.
