# Apple's Font Tools for Xcode

What's available for download in summer 2024 (8 to 9 were "re-released" after introduction of SIP and signed):

| Name | Release Date | File | Size |
| ---  | --- | --- | --- |
| Font Tools for Xcode 16 beta     | June 10, 2024      | Font Tools for Xcode 16 beta.dmg      | 9.37 MB |
| Font Tools for Xcode 15.1        | December 11, 2023  | Font Tools for Xcode 15.1.dmg         | 9.37 MB |
| Font Tools for Xcode 15.1 beta 3 | November 14, 2023  | Fonts Tools For Xcode 15.1 beta 3.dmg | 9.36 MB |
| Font Tools for Xcode 15          | September 18, 2023 | Font Tools for Xcode 15.dmg           | 9.37 MB |
| Font Tools for Xcode 15 Release Candidate | September 12, 2023 | Font Tools for Xcode 15 Release Candidate.dmg | 9.37 MB |
| Font Tools for Xcode 15 beta     | June 5, 2023       | Font_Tools_for_Xcode_15_beta.dmg      | 9.39 MB |
| Font Tools for Xcode 14          | September 12, 2022 | Font Tools for Xcode 14.dmg           | 9.44 MB |
| Font Tools for Xcode 14 Release Candidate | September 7, 2022  | Font Tools for Xcode 14 Release Candidate.dmg | 9.44 MB |
| Font Tools for Xcode 13          | September 20, 2021 | Font Tools for Xcode 13.dmg           | 9.44 MB |
| Font Tools for Xcode 13 beta     | June 7, 2021       | Font Tools for Xcode 13 beta.dmg      | 9.43 MB |
| Font Tools for Xcode 12          | September 16, 2020 | Font Tools for Xcode 12.dmg           | 9.23 MB |
| Font Tools for Xcode 12 beta     | June 22, 2020      | Font Tools for Xcode 12.dmg           | 7.84 MB |
| ---  | --- | --- | --- |
| Font Tools for Xcode 8           | November 8, 2019   | Font Tools for Xcode 8.dmg            | 10.36 MB |
| Font Tools for Xcode 8.1         | November 8, 2019   | Font Tools for Xcode 8.1.dmg          | 10.45 MB |
| Font Tools for Xcode 8.2         | November 8, 2019   | Font Tools for Xcode 8.2.dmg          | 10.36 MB |
| Font Tools for Xcode 9           | November 1, 2019   | Font Tools for Xcode 9.dmg            | 10.41 MB |
| ---  | --- | --- | --- |
| Font Tools for Xcode 11          | October 1, 2019    | Font Tools for Xcode 11.dmg           | 10.46 MB |
| Font Tools for Xcode 11 GM Seed  | September 10, 2019 | Font Tools for Xcode 11 GM Seed.dmg   | 10.45 MB |
| OS X Font Tools Release 4, beta 1 | October 11, 2011  |                                       | 10.36 MB |

(pre-SIP) versions no longer available for download:

| Date | Name |
| ---  |  --- |
| 2017-09-19 | Font_Tools_for_Xcode_9.dmg        |
| 2016-12-08 | Font_Tools_for_Xcode_8.2.dmg      |
| 2016-10-21 | Font_Tools_for_Xcode_8.1.dmg      |
| 2016-09-21 | Font_Tools_for_Xcode_8.1_beta.dmg |
| 2016-09-13 | Font_Tools_for_Xcode_8.dmg        |
| 2016-06-10 | Font_Tools_for_Xcode_8_beta.dmg   |


Self-reported versions:

| Xcode version | ftxvalidator build | FontToolbox.framework build |
| ---  | --- | --- |
| 16 Beta | 208 | 354 |
| 15.1 | 208 | 354 |
| 15 | 208 | 353 |
| 14 | 208 | 353 |
| 13 | 208 | 353 |
| 12 | 207 | 340 |
| 11 | 207 | 335 |
| --- | --- | --- |
| 9 | 207 | 257 |
| 8 | 207 | 239 |
| 4 beta 1 | -- | 55 |

8, 9 does not install on Mac OS 12; but manually unpacking then running works.
4 beta 1 fails on recent Mac OS with "Objective-C garbage collection is no longer supported.".
Some of the other tools report FontToolbox.framework version as "55".

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
