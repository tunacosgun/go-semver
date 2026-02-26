<div align="center">

# 🛠 Go Semantic Versioning (go-semver)

<br/>

[![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)](https://go.dev/)
[![SemVer](https://img.shields.io/badge/Semantic_Versioning-2.0.0-F25C78?style=for-the-badge)](https://semver.org/)

<br/>

A lightweight, robust, and highly performant **Semantic Versioning** parser and evaluator written in purely native **Go**. Designed meticulously to parse, sort, and compare versions aligning precisely with Semantic Versioning standards.

<br/>

[Overview](#-overview) · [Features](#-features) · [Installation](#-installation)

</div>

<br/>

---

<br/>

## 🎯 Overview

Parsing version strings accurately during CI/CD pipelines or dependency resolutons is complex. `go-semver` handles the heavy lifting safely and extremely fast without utilizing heavyweight Regex implementations, enforcing strict Semantic Version rules directly via strong type comparisons in Go.

<br/>

---

<br/>

## ✨ Key Features

- **Strict Parsing**: Reads structured version tags (e.g. `v1.2.4-alpha.2+build.104`) accurately.
- **Pre-Release Identifiers**: Full logic support comparing `alpha`, `beta`, `rc` structures.
- **Native Implementation**: Zero external module dependencies. Pure standard library utilizing Go's speed.
- **Easy Sorting**: Implementation bridging Go's native `sort.Interface` to rapidly array version lists.

<br/>

---

<br/>

## 🚀 Installation & Usage

Using standard `go get` implementations:

```go
go get github.com/tunacosgun/go-semver
```

Integrate into your codebase:

```go
import "github.com/tunacosgun/go-semver/semver"

// Example Usage
v, err := semver.NewVersion("v1.2.3-beta.1")
if err != nil {
    // Handle error
}

// Check comparisons natively
isValid := v.GreaterThan(v2)
```

<br/>

---

<div align="center">
<b>Secure robust version handling inside Go.</b>
</div>