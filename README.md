# meta-npmignore

A zero dependency cli tool to generate .npmignore file dynamically, based on local and global gitignore config.

## Motivation

To avoid accidentally publishing {unnecessary,credential} files, such as `yarn.error`, `.envrc` or others, 
we have to manage DUPLICATE declarations, both of .gitignore and .npmignore.

`meta-npmignore` solves DUPLICATE declarations. 

## Usage

### Init

Rename `.npmignore` into `.npmignorerc` and add `.npmignore` into `.gitignore`

```bash
$ meta-npmignore --init
```

### Run

Adding `meta-npmignore` into `prepare` npm scripts is recommended.

```bash
$ meta-npmignore
```

## LICENCE

MIT
