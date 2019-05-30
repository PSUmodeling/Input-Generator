# Input-Generator
C code to generate multiple input files from template by replacing keywords.

The program requires two input files: a template file and a configuration file.
1. In the template file, keywords that need to be marked using a **"$"** sign.
   Multiple keywords can be used.
   For example, in the sample template file, `test.operation`, keywords **$CROP** and **$DOY** are used.
2. The header line of the configuration file should start with **DEST_FILE**, followed by keywords that appear in the template file.
   The following lines of configuration file should specify the destination file name, and the replace words for each keywords.

To start replacing, run
```shell
./input_gen <template file> <configuration file> <path_to_generated_files>
```

**NOTE:** Currently, only one keyword is allowed in each line of the template file.
Replacing multiple keywords in one line is not supported.
