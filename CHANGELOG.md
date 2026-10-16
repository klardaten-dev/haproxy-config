# Changelog

## 1.0.2
- Target HAProxy version (*Settings | Languages & Frameworks | HAProxy*, 2.6 – 3.5): warnings for sections, keywords,
  actions, bind/server options, sample fetches and converters that are newer than the version your servers run;
  completion leaves them out.
- Version data now covers HAProxy 2.6, 2.8, 3.0, 3.1, 3.2, 3.3, 3.4 and 3.5-dev.

## 1.0.1
- Reformat Code for HAProxy files: section header lines at column 0, section bodies indented by one level
  (uses the IDE's indent settings), trailing whitespace removed. Spacing between arguments and `.if`/`.endif` lines are
  left as they are.
- Quick fix "Create backend/cache/… section" for references to sections that don't exist yet.

## 1.0.0
First release: highlighting, completion, navigation/rename, inspections, quick documentation, structure view and
folding for HAProxy configuration files; keyword data from HAProxy 2.8 – 3.x manuals.
