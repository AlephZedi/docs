# Track configuration

```text
./config.json
```

This file has the following keys:

* **language** \(string\) the official name of the programming language.
* **blurb** \(string\) a short, friendly intro to be used in the header of the landing page on the site.
* **active** \(boolean\) whether the track is active on the site.
* **test\_pattern** \(string\) _\(optional\)_ a regex pattern that test filenames will match. It is used to determine which files will be visible on a problem's test-suite page on the exercism.io site. The default value used if this key is not present is `/test/i`.
* **ignore\_pattern** \(string\) _\(optional\)_ a regex pattern that will cause files matching it to not be served by the `exercism fetch` command. The default value used if this key is not present is `/example/i`.
* **solution\_pattern** \(string\) _\(optional\)_ a regex pattern that matches solution files in the track repository. If not present, it defaults to `/[Ee]xample/`
* **foregone** \(array of strings\) a list of problem specification slugs that the track maintainers have decided not to implement.
* **exercises** \(array of objects\) the metadata for implemented exercises.

The format of the `exercises` array is described in detail [here](exercises.md).

