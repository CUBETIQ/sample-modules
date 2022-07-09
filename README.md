# Sample Modules

- Spring Boot with Kotlin
- Spring Dependency Management
- Gradle with Kotlin DSL

# Development

- Clone the modules

```shell
git clone https://git.cubetiqs.com/CUBETIQ/sample-modules.git --recurse-submodules --remote-submodules
```

### Add Submodule by using git submodule (Example)

```shell
git submodule add https://git.cubetiqs.com/CUBETIQ/gradle-sample-module-example.git
```

### Register module in ```settings.gradle.kts``` or ```settings.gradle```

```gradle
rootProject.name = "sample-modules"
include("gradle-sample-module-example")
```

### Implementation module in ```build.gradle.kts```

```gradle
implementation(project(":gradle-sample-module-example"))
```