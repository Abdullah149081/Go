# Go

This repository demonstrates basic concepts of Go programming

## Table of Contents

- [Introduction](#introduction)
- [Code Examples](#code-examples)
  - [Using `var` with explicit type](#using-var-with-explicit-type)
  - [Using `var` without explicit type](#using-var-without-explicit-type)
  - [Using shorthand `:=`](#using-shorthand-)
  - [Using `const`](#using-const)

## Variables Introduction

In Go, variables can be declared in multiple ways, including using `var`, shorthand `:=`, and `const`. This repository includes different examples to help you understand how to declare variables in Go.

## Code Examples

### Using `var` with explicit type

When declaring variables with `var`, you can specify the type explicitly.

```go
package main

import "fmt"

func main() {
	var firstName string = "Abdullah"
	var secondName string = "Al"
	var lastName string = "Masud"

	fmt.Println(firstName, secondName, lastName)
}
```

### Using `var` without explicit type

Go supports type inference, which allows you to omit the type when using var. Go automatically infers the type based on the assigned value.

```go
package main

import "fmt"

func main() {
	var firstName = "Abdullah"
	var secondName = "Al"
	var lastName = "Masud"

	fmt.Println(firstName, secondName, lastName)
}
```

### Using shorthand `:=`

Shorthand := is used to declare and initialize variables in a single statement, but it can only be used within a function (not at the package level).

```go
package main

import "fmt"

func main() {
	firstName, secondName, lastName := "Abdullah", "Al", "Masud"

	fmt.Println(firstName, secondName, lastName)
}
```

### Using `const`

Constants are used when you have fixed values that shouldn't change. Constants must be assigned a value at the time of declaration.

```go
package main

import "fmt"

func main() {
	const firstName = "Abdullah"
	const secondName = "Al"
	const lastName = "Masud"

	fmt.Println(firstName, secondName, lastName)
}
```
