# Filey diff

A Ruby library for comparing file-like objects from various data sources.

## Central concepts

### Filey

A file-like object. Can be, for example, a *file system file* or an *AWS S3
object*.

### Data source

Provides Fileys.

The current built-in data sources support Amazon Web Services S3 and file
system.

## Operations

### List outdated files

Given two data sources A and B, list the changed files that A has but B doesn't.

### List missing files

Given two data sources A and B, list the files that A has but B doesn't.

## Example use cases

Arnie has a blog on AWS S3. He has just finished a new post and wants to upload
only the new post into S3. With the help of Filey diff Arnie can write a Ruby
program that uploads only the new post and nothing else.

## License

Copyright (C) 2012 Lauri Lehmijoki

Distributed under the Apache-2.0 license http://www.apache.org/licenses/LICENSE-2.0.html
