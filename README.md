# find_files_for_deletion

Identify files which can be deleted or which need some action (like being gzipped).

[![Build Status](https://travis-ci.org/sanger-pathogens/find_files_for_deletion.svg?branch=master)](https://travis-ci.org/sanger-pathogens/find_files_for_deletion)  
[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-brightgreen.svg)](https://github.com/sanger-pathogens/find_files_for_deletion/blob/master/LICENSE)  

## Contents
  * [Introduction](#introduction)
  * [Installation](#installation)
    * [Required dependencies](#required-dependencies)
  * [Usage](#usage)
  * [License](#license)
  * [Feedback/Issues](#feedbackissues)

## Introduction
This is a script for identifying files that can be deleted or compressed to save space.
 
## Installation
### Required dependencies
* Test::Most  
* Moose  
* File::Slurp  
* YAML::XS  

Details for installing find_files_for_deletion are provided below. If you encounter an issue when installing find_files_for_deletion please contact your local system administrator. If you encounter a bug please log it [here](https://github.com/sanger-pathogens/find_files_for_deletion/issues) email us at path-help@sanger.ac.uk.

Clone the GitHub repository:
```
git clone https://github.com/sanger-pathogens/find_files_for_deletion.git
```
Move into the directory and run the tests:
```
cd find_files_for_deletion
make test
```
## Usage
```
Usage: ./find_files_to_delete.pl [options]
This will look for files which can usually be deleted

./find_files_to_delete.pl -e test --directory /path_to/directory -o my_output_file
 Options:
     --environment     Production or Test
     --directory       The root directory to use
     --output_file     The filename for the raw list of found files
     --quiet           Do not send emails to users or admin
```
## License
find_files_for_deletion is free software, licensed under [GPLv3](https://github.com/sanger-pathogens/find_files_for_deletion/blob/master/LICENSE).

## Feedback/Issues
Please report any issues to the [issues page](https://github.com/sanger-pathogens/find_files_for_deletion/issues) or email path-help@sanger.ac.uk.

