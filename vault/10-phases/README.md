# Phases
One note per course module (template: `course-module`). Progress dashboard:

```dataview
TABLE course, phase, status, started, finished
FROM "10-phases"
WHERE type = "module"
SORT phase ASC, started ASC
```
