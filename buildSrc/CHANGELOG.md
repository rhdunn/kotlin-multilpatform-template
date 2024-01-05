# Change Log
> Release notes for the Kotlin multiplatform project template.

This format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [1.3.1] - 2024-01-05

This release supports Kotlin 1.7.

### Fixed

- Added missing imports from the template `build.gradle.kts` file.

## [2.1.0] - 2023-05-29

This release supports Kotlin 1.8.

### Added

- Support for the Maven snapshot repository if enabled by the build
  configuration.

### Changed

- Make the use of Maven Local determined by the build configuration.

### Fixed

- Fix the name of the "publish to maven central" targets in GitHub Actions.
- Fix building for Kotlin/JVM when the Java version is different.

## [1.3.0] - 2023-05-29

This release supports Kotlin 1.7.

### Added

- Support for the Maven snapshot repository if enabled by the build
  configuration.

### Changed

- Make the use of Maven Local determined by the build configuration.

### Fixed

- Fix the name of the "publish to maven central" targets in GitHub Actions.
- Fix building for Kotlin/JVM when the Java version is different.

## [2.0.0] - 2023-05-22

### Removed

- Remove support for the deprecated Kotlin/JS legacy target.
- Remove support for the deprecated Kotlin/Native targets.

### Changed

- Default to building with gradle 8.1.1.

### Dependency Upgrades

- Upgrade to Gradle 8.0 and later.
- Upgrade to Kotlin 1.8.21.
- Upgrade to Dokka 1.8.10.
- Upgrade to JUnit 5.9.3.

## [1.2.1] - 2023-05-20

### Fixed

- Don't run the workflows when pushing tags to the repository.
- Set `jvm.variants` and `konan.variants` to `target-only` when importing the
  project in IntelliJ IDEA.
- Fix running the build action for the `watchos_x86` Kotlin/native target on
  GitHub Actions.

## [1.2.0] - 2023-05-16

### Added

- A `SupportedVariants` enumeration type.
- `jvm.variants` and `konan.variants` build configuration properties.
- `jvmMain` and `jvmTest` DSL helper methods taking a `Named` target.
- The readme file now includes:
    - table of contents
    - documentation links
    - information for adding the library as a Maven dependency
    - maven central and license badges

### Fixed

- Use `jvm` for the Kotlin/JVM documentation.
- Use `native` for the Kotlin/Native documentation.

## [1.1.0] - 2023-05-14

### Added

- A `jvmName` DSL helper method.
- `jvmMain`, `jvmTest`, and `jvmArtifactId` DSL helper methods taking a `JavaVersion`.
- A `KonanTarget.publicationName` DSL helper property.
- `nativeMain` and `nativeTest` DSL helper methods taking a `Named` target.

### Fixed

- Resolve dependency variants locally for e.g. `kotlin-test`.
- Include all the supported JVM target variants in the `kotlinMultiplatform` module metadata.
- Include all the supported native target variants in the `kotlinMultiplatform` module metadata.

## [1.0.0] - 2023-05-10

### Added

- `.gitignore` rules for IntelliJ IDE and gradle.
- Kotlin Multiplatform configuration for JS, Native, and JVM.
- Publication artifact signing.
- Configuring and deploying to Maven Local and Maven Central.
- Build and publish the Dokka documentation to GitHub Pages.
- Build and optionally deploy the various targets to Maven Central.

[Unreleased]: https://github.com/rhdunn/kotlin-multilpatform-template/compare/2.1.0...HEAD
[2.1.0]: https://github.com/rhdunn/kotlin-multilpatform-template/compare/2.0.0...2.1.0
[2.0.0]: https://github.com/rhdunn/kotlin-multilpatform-template/compare/1.2.1...2.0.0
[1.3.1]: https://github.com/rhdunn/kotlin-multilpatform-template/compare/1.3.0...1.3.1
[1.3.0]: https://github.com/rhdunn/kotlin-multilpatform-template/compare/1.2.1...1.3.0
[1.2.1]: https://github.com/rhdunn/kotlin-multilpatform-template/compare/1.2.0...1.2.1
[1.2.0]: https://github.com/rhdunn/kotlin-multilpatform-template/compare/1.1.0...1.2.0
[1.1.0]: https://github.com/rhdunn/kotlin-multilpatform-template/compare/1.0.0...1.1.0
[1.0.0]: https://github.com/rhdunn/kotlin-multilpatform-template/releases/tag/1.0.0
