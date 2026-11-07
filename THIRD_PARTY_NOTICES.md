# Third-party notices

QEntry is proprietary software (see [LICENSE](LICENSE)). It includes the open-source components below, each under its own license. Nothing in the QEntry license limits your rights under these licenses.

The license and NOTICE files that come with each Java library stay inside the library's own jar, unchanged, in `app.jar` (`BOOT-INF/lib/`).

## Backend (`app.jar` in the `qentry-app` image)

| Component | License |
|---|---|
| Spring Framework, Spring Boot, Spring Data, Spring Security | Apache-2.0 |
| Hibernate ORM, Hibernate Models, Hibernate Validator, JBoss Logging, Classmate | Apache-2.0 |
| Apache Tomcat (embedded), Apache Commons Lang, Apache Commons Logging, Apache Log4j API | Apache-2.0 |
| Jackson, SnakeYAML, Byte Buddy, HikariCP, Micrometer, JSpecify | Apache-2.0 |
| Flyway (community edition, PostgreSQL support) | Apache-2.0 |
| JJWT | Apache-2.0 |
| springdoc-openapi, Swagger Core, Swagger UI | Apache-2.0 |
| PostgreSQL JDBC driver | BSD-2-Clause |
| HdrHistogram | BSD-2-Clause (or CC0-1.0) |
| ANTLR 4 runtime | BSD-3-Clause |
| SLF4J, jul-to-slf4j, Checker Framework qualifiers, webjars-locator-lite | MIT |
| Logback | EPL-1.0 / LGPL-2.1 (dual; used under EPL) |
| AspectJ weaver | EPL-2.0 (with BSD-3-Clause and Apache-1.1 parts) |
| Jakarta Annotation API, Jakarta Transaction API | EPL-2.0 or GPL-2.0 with Classpath Exception |
| Jakarta Persistence API | EPL-2.0 / EDL-1.0 |
| Jakarta Activation, Jakarta XML Binding (API and runtime), Angus Activation, istack, TXW2 | EDL-1.0 (BSD-3-Clause) |

## Web apps (dashboard, caller, display, counter display, kiosk, resto in the `qentry-web` image)

Bundled, minified, into the apps' JavaScript files:

| Component | License |
|---|---|
| React, React DOM, scheduler | MIT |
| lucide-react | ISC |
| @noble/hashes | MIT |
| qrcode, with dijkstrajs, pngjs and its yargs helpers (camelcase, cliui, decamelize, find-up, locate-path, p-limit, p-locate, p-try, path-exists, require-directory, require-main-filename, set-blocking, string-width, strip-ansi, ansi-regex, ansi-styles, color-convert, color-name, emoji-regex, is-fullwidth-code-point, which-module, wrap-ansi, y18n, yargs, yargs-parser, get-caller-file) | MIT / ISC |
| write-excel-file, fflate | MIT |

Fonts:

| Font | License |
|---|---|
| Barlow Condensed, Copyright 2017 The Barlow Project Authors | SIL Open Font License 1.1 |
| Plus Jakarta Sans, Copyright 2020 The Plus Jakarta Sans Project Authors | SIL Open Font License 1.1 |

The full font licenses are in `display/src/assets/fonts/OFL-*.txt`, in the repository and in the release zip.

## Docker images

The release zip's `qentry-images.tar.gz` holds two images built on these open-source bases:

| Image | Built on | Includes |
|---|---|---|
| `qentry-app` | `eclipse-temurin:21-jre-alpine` | Eclipse Temurin Java runtime (OpenJDK, GPL-2.0 with Classpath Exception) and Alpine Linux packages (among others BusyBox, GPL-2.0; musl libc, MIT) |
| `qentry-web` | `nginx:1.27-alpine` | nginx (BSD-2-Clause) and Alpine Linux packages (as above) |

The database and the HTTPS proxy are not in the zip. The installer downloads the official `postgres:15` (PostgreSQL License) and `caddy:2-alpine` (Apache-2.0) images from Docker Hub.

### Source code of GPL and LGPL components

The source code of the GPL- and LGPL-licensed components above is published by their projects:
- Eclipse Temurin: https://github.com/adoptium
- Alpine Linux packages: https://gitlab.alpinelinux.org/alpine/aports
- nginx: https://nginx.org

For three years from the date you received QEntry, the Licensor will also provide, on request, a copy of the corresponding source code of those components, for no more than the cost of making and sending it. Ask your QEntry supplier, who passes the request to the Licensor.
