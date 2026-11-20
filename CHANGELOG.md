# Changelog

## 1.0.3
Fixes found by testing on ~170 more real configs (HAProxy Data Plane API, config-parser and client-native test configs,
Kubernetes ingress controllers, Patroni and others):
- `acl` is accepted in `fcgi-app` sections.
- `track-sc3` and higher are accepted. When the file's `global` section sets `tune.stick-counters` too low, you get a
  warning; without that setting, a weak hint (the default is 3).
- Server option `resolve-opts` is known.
- HAProxy 3.5-dev: `http-hardening` sections (all checks, `from`, profile references on `bind`/`server` lines, built-in
  `trusted`/`untrusted` profiles), plus the other new keywords up to 3.5-dev13 (`tr()`, `h2_enabled`, `tune.h2.fe.enabled`…).
- Documentation links for keywords added in 3.4/3.5 open the development manual.

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
