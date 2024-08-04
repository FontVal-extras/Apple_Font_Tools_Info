# Apple's Font Tools for Xcode

| Name | Release Date | File | Size |
| ---  | --- | --- | --- |
| Font Tools for Xcode 16 beta     | June 10, 2024      | Font Tools for Xcode 16 beta.dmg      | 9.37 MB |
| Font Tools for Xcode 15.1        | December 11, 2023  | Font Tools for Xcode 15.1.dmg         | 9.37 MB |
| Font Tools for Xcode 15.1 beta 3 | November 14, 2023  | Fonts Tools For Xcode 15.1 beta 3.dmg | 9.36 MB |
| Font Tools for Xcode 15          | September 18, 2023 | Font Tools for Xcode 15.dmg           | 9.37 MB |

```
ftxvalidator build 208, FontToolbox.framework build 354
Usage:  ftxvalidator [-hlrRSTvV] [-t testList] [-o outputfile] fontfile
Options:
	-e (--exclude) An optional list of tests to exclude
	-h (--help) Output this message
	-K (--check-build-number) Check that the tool is at least the given version
		`ftxvalidator-K 200` returns -1 if the build number is not 200 or higher
	-l (--list) List available tests
	-o (--output) An optional output file for test results; stdout is used if this parameter is not specified
	-r (--full-report) Generate a full report
	-R (--return-value-results) Use return value to indicate overall results
	-S (--summary-report) Generate a summary report
	-t (--test-list) The tests to execute.  Valid inputs are:
		"all", execute all tests,
		"core", execute the core test set,
		"default", execute the default test set,
		or a list of font test types, separated by commas,
		or a list of test identifiers, separated by commas`	
	-T (--table-report) Generate a tabular report
	-v (--verbose) Verbose operation, additional data is output to stderr
	-V (--version) Output the tool's version to stdout
	-W (--suppress-warnings) Suppress warning messages

Return values:
	0 No results
	1 Execution errors
	2 No execution errors, validator fatal errors found
	3 No execution errors, validator major errors found
	4 No execution errors, validator minor errors found
	5 No execution errors, spec violations found
The return value, if greater than 1, is the lowest value possible.
Return values greater than 1 are only used if --return-value-results is set.
```
