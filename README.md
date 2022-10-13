# COURSE: RUST

My course on Rust programming.

## REFERENCES

* [Website - Rust Lanaguage Project](https://www.rust-lang.org/)
* [Website - Rust Playground](https://play.rust-lang.org/)
* [Website - Rustup](https://rustup.rs/)
* [Ebook - Rust in Action](https://www.manning.com/books/rust-in-action)

---

## GETTING STARTED

Try Rust online in the [Rust Playground](https://play.rust-lang.org/).

---

## DEVELOPER'S GUIDE

Not available yet.

### Installation

Try Rust online in the [Rust Playground](https://play.rust-lang.org/) without installing.

To install Rust, use [the official installers](https://rustup.rs/).

``` shell
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

#### RUST IN ACTION

### C1 - Introducing Rust

Rust’s <b>cargo</b> tool provides both a build system and a package manager. That means cargo knows how to convert your Rust code into executable binaries and also can manage the process of downloading and compiling the project’s dependencies.

For a hello-world project:

``` shell
$ cd $TMP
$ cargo new hello # cargo creates a default project structure
$ cd hello
$ cargo run # cargo runs the project, added new files, compiles the code in debug mode, and results in an executable binary file
```

<b>Cargo</b> creates a standard template project:

``` shell
$ sudo apt-get -y update && sudo apt -y install tree
$ tree --dirsfirst hello
hello
├── src
│ └── main.rs
├── target
│ └── debug
│ ├── build
│ ├── deps
│ ├── examples
│ ├── native
│ └── hello
├── Cargo.lock
└── Cargo.toml
```

* Rust source (<b>.rs</b> extension) code appears in the src directory.
* Cargo.toml describes the project’s metadata, such as the project’s name, its version, and its dependencies
* Cargo.lock file and a target/ directory are managed by cargo

New hello-project:

# main.rs
fn greet_world() {
    println!("Hello, world!"); 
    let southern_germany = "Grüß Gott!"; 
    let japan = "ハロー・ワールド"; 
    let regions = [southern_germany, japan]; 
    for region in regions.iter() { 
        println!("{}", &region); 
    }
}

fn main() {
    greet_world()
}

Rust features:
* The exclamation mark indicates the use of a macro, which we’ll discuss shortly.
* Assignment in Rust, more properly called variable binding, uses the let keyword.
* Unicode support is provided out of the box. Strings are guaranteed to be encoded as UTF-8.
* Array literals use square brackets.
* Many types can have an iter()  method to return an iterator.
* The ampersand “borrows”  region for read-only access.
* Calls a function. Note  that parentheses follow  the function name.
* Executable projects require a main() function.
* Escapes the trailing newline character (\)
* Skips header row and lines with  only whitespace
* cfg! checks configuration  at compile time.
* eprintln! prints to standard error (stderr).
* println! prints to standard out (stdout).

Rust comes close to the high-level, expressive feel of dynamic languages, achieving low-level, bare-metal performance.

* Common control flow mechanisms: This includes for loops and the continue keyword.
* Method syntax: Although Rust is not object-oriented as it does not support inheritance, it carries over this feature of object-oriented languages.
* Higher-order programming: Functions can both accept and return functions.
* Type annotations—Although relatively rare, these are occasionally required as a hint to the compiler.
* Conditional compilation—In the listing, lines 21–24 (if cfg!(…);) are not included in release builds of the program.
* Implicit return—Rust provides a return keyword, but it’s usually omitted. Rust is an expression-based language.

Macros are similar to functions except that instead of returning data, these return code. Macros are often used to simplify common patterns.


### What is Rust?

Rust’s distinguishing feature as a programming language is its ability to prevent invalid data access at compile time. Rust eliminates that class of bug (approximately 70% of serious security bugs). It guarantees that your program is memory-safe without imposing any run-time costs.

Other languages can provide this level of safety, but these require adding checks that execute while your program is running, thus slowing it down. Rust’s distinguishing feature as a professional community is its willingness to explicitly include values into its decision-making process. Even the Rust compiler’s error messages are ridiculously helpful.

Rust is labelled as a systems programming language, which tends to be seen as quite a specialized, almost esoteric branch of programming. However, many Rust programmers
have discovered that the language is applicable to many other domains. Safety, productivity, and control are useful in all software engineering projects. Moreover, the
Rust community’s inclusiveness means that the language benefits from a steady stream
of new voices with diverse interests




### Rust’s big features

The three principles features of the language:
* Performance
* Concurrency
* Memory efficiency
* A positive and welcoming community




###  Downsides of Rust

...


### Where does Rust fit best?

Although it was designed as a systems programming language, Rust is a general-purpose language.
* Command-line utilities
* Data processing
* Extending applications
* Resource-constrained environments
* Server-side applications
* Desktop applications
* Desktop
* Mobile
* Web
* Systems programming

### SUMMARY
* Many companies have successfully built large software projects in Rust.
* Software written in Rust can be compiled for the PC, the browser, and the server, as well as mobile and IoT devices.
* The Rust language is well loved by software developers. It has repeatedly won Stack Overflow’s “most loved programming language” title.
* Rust allows you to experiment without fear. It provides correctness guarantees that other tools are unable to provide without imposing runtime costs.
* With Rust, there are three main command_line tools to learn:
– cargo, which manages a whole crate
– rustup, which manages Rust installations
– rustc, which manages compilation of Rust source code
* Rust projects are not immune from all bugs.
* Rust code is stable, fast, and light on resources.

---

## USER'S GUIDE

Not available yet.

---

## CONTRIBUTOR'S GUIDE

Not available yet.

---

## RUST PROGRAMMING

Not available yet.

---

## ADDITIONAL SOURCES

Not available yet.

---