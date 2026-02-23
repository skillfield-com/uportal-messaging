
# Upgrade Java Project

## 🖥️ Project Information
- **Project path**: /Users/subodhchettri/repo/uportal-messaging
- **Java version**: 21
- **Build tool type**: Maven
- **Build tool path**: /opt/homebrew/Cellar/maven/3.9.11/bin

## 🎯 Goals

- Upgrade Java to 21
- Upgrade Spring Boot to 2.7.x

## 🔀 Changes

### Test Changes
|     | Total | Passed | Failed | Skipped | Errors |
|-----|-------|--------|--------|---------|--------|
| Before | 96 | 96 | 0 | 0 | 0 |
| After | 0 | 0 | 0 | 0 | 0 |
### Dependency Changes


#### Upgraded Dependencies
| Dependency | Original Version | Current Version | Module |
|------------|------------------|-----------------|--------|
| org.springframework.boot:spring-boot-starter-web | 1.5.9.RELEASE | 2.7.18 | uportal-messaging |
| org.springframework.boot:spring-boot-starter-data-rest | 1.5.9.RELEASE | 2.7.18 | uportal-messaging |
| org.springframework.boot:spring-boot-starter-tomcat | 1.5.9.RELEASE | 2.7.18 | uportal-messaging |
| org.springframework.boot:spring-boot-devtools | 1.5.9.RELEASE | 2.7.18 | uportal-messaging |
| org.springframework.boot:spring-boot-starter-test | 1.5.9.RELEASE | 2.7.18 | uportal-messaging |
| Java | 8 | 21 | Root Module |

#### Added Dependencies
|   Dependency   | Version | Module |
|----------------|---------|--------|
| junit:junit | 4.13.2 | uportal-messaging |
| jakarta.validation:jakarta.validation-api | 3.0.2 | uportal-messaging |
| org.mockito:mockito-core | 5.2.0 | uportal-messaging |
| org.mockito:mockito-inline | 5.2.0 | uportal-messaging |
| cglib:cglib | 3.3.0 | uportal-messaging |

### Code commits

All code changes have been committed to branch `appmod/java-upgrade-20260223003839`, here are the details:
7 files changed, 49 insertions(+), 12 deletions(-)

- cf8f611 -- Upgrade to Java 21 and Spring Boot 2.7.x

- fea59e9 -- Validate build after vulnerability check
### Potential Issues

#### CVEs
- commons-io:commons-io:2.6:
  - [**MEDIUM**][CVE-2021-29425](https://github.com/advisories/GHSA-gwrp-pvrq-jmwv): Path Traversal and Improper Input Validation in Apache Commons IO
  - [**HIGH**][CVE-2024-47554](https://github.com/advisories/GHSA-78wr-2p64-hpwj): Apache Commons IO: Possible denial of service attack on untrusted input to XmlStreamReader

- org.json:json:compile:
  - [**HIGH**][CVE-2022-45688](https://github.com/advisories/GHSA-3vqj-43w4-2q58): json stack overflow vulnerability
  - [**HIGH**][CVE-2023-5072](https://github.com/advisories/GHSA-4jq9-2xhw-jpx7): Java: DoS Vulnerability in JSON-JAVA

- org.apache.commons:commons-lang3:3.7:
  - [**MEDIUM**][CVE-2025-48924](https://github.com/advisories/GHSA-j288-q9x7-2f5v): Apache Commons Lang is vulnerable to Uncontrolled Recursion when processing long inputs
