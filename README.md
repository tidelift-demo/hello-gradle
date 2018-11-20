# hello-gradle

The dependency graph for gradle projects needs to be created by gradle itself to be complete. For example, you can run
```bash
gradle dependencies -q > gradle-dependencies-q.txt
```

Or

```bash
./gradlew dependencies -q > gradle-dependencies-q.txt
```

And Tidelift will be able to analyze the dependencies.


## Project w/ subproject

You may need to target specific desired subprojects to generate the dependency graph depending on the project structure. For example,

```bash
./gradlew server:dependencies -q > gradle-dependencies-q.txt
```
