### Multimodule-starter

<details><summary><h3> Steps to manage gradle files </h3></summary>

1. Change view of your project from Android to Project
2. Right click on top, then new -> Directory and create a Directory named as buildSrc
3. Create a new file "build.gardle.kts" under buildSrc
4. Write these lines under this file and click on sync now

```
   plugins{
    `kotlin-dsl`
    }

repositories{
    mavenCentral()
}

```

5. buildSrc will be changed in the form of a module. This is present at root level and hence accessible from every build.gradle of each module.

6. Again, create new -> directory : src\main\java under buildSrc
7. Create a new kotlin file in java folder named as : Dependencies.kt
8. Switch view from Project to Android and go on `build.gradle(Module:app)`
9. Do the necessary operations for conversion of gradle files.
</details>
