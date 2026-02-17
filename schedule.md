
## Schedule

This course is structured into 6 parts, each approximately 1 hour long.

### Part 1: Why R Packages and Getting Started

- Why write an R package?
  - R packages as portable code containers
  - The "laundry basket" analogy
  - Sharing code beyond copy-paste and email
  - Packages for personal use vs public sharing
- Installation and setup
  - Verify R, RStudio, and required packages
  - Installing {usethis}, {devtools}, {roxygen2}, {testthat}
  - Understanding the RStudio IDE for package development
  - Setting up your development environment
- Introduction to the {praiseme} package
  - Our teaching package modeled on {praise}
  - What we'll build together
  - Overview of the package development workflow

### Part 2: Creating Your First Package

- Creating the package structure
  - Using `usethis::create_package()`
  - Understanding DESCRIPTION, NAMESPACE, and R/ folder
  - What files are essential vs optional
- Building your first function
  - Writing a simple function in R/
  - Loading with `devtools::load_all()`
  - Testing your function interactively
- Package metadata
  - Editing the DESCRIPTION file
  - Title, Description, Author fields
  - Choosing a license with `usethis::use_*_license()`
  - Version numbering basics

### Part 3: Documentation with roxygen2

- Exporting and documenting functions
  - Using roxygen2 comments above functions
  - `@param`, `@return`, `@examples`, `@export`
  - Generating documentation with `devtools::document()`
  - Viewing help pages with `?function_name`
- Adding function arguments
  - Making functions more flexible
  - Required vs optional arguments
  - Setting sensible defaults
  - Documenting each argument properly
- Hands-on practice
  - Add arguments to your package functions
  - Write comprehensive documentation
  - Test examples to ensure they work

### Part 4: Package Checking and Dependencies

- Running R CMD check
  - Using `devtools::check()` to validate your package
  - Understanding NOTEs, WARNINGs, and ERRORs
  - Common check problems and solutions
  - Getting to a clean check
- Using functions from other packages
  - Understanding DESCRIPTION: Imports vs Suggests
  - Adding dependencies with `usethis::use_package()`
  - Calling functions with `::`
  - Best practices for managing dependencies
- Hands-on exercise
  - Add a package dependency
  - Use functions from external packages
  - Run `devtools::check()` and fix any issues

### Part 5: Testing and Quality Assurance

- Why test your package?
  - Catching bugs before users do
  - Confidence when refactoring
  - Tests as documentation of expected behavior
- Writing tests with {testthat}
  - Setting up with `usethis::use_testthat()`
  - Creating test files with `usethis::use_test()`
  - Writing expectations: `expect_equal()`, `expect_error()`, etc.
  - Running tests with `devtools::test()`
- Practical testing
  - Write tests for your package functions
  - Test edge cases and error conditions
  - Achieve reasonable test coverage
  - Fix bugs revealed by tests

### Part 6: Sharing Your Package

- Putting your package online
  - Setting up Git for your package
  - Creating a GitHub repository
  - Pushing your package to GitHub
  - Making your package installable with {remotes}
- Creating a README
  - Using `usethis::use_readme_rmd()`
  - What to include: installation, basic usage, examples
  - Rendering README with `devtools::build_readme()`
  - Badges and project status
- Next steps and extensions
  - GitHub Actions for continuous integration
  - Creating package websites with {pkgdown}
  - R Universe for easy installation
  - Submitting to CRAN (overview)
- Open Q&A and individual help
  - Work on your own package ideas
  - Troubleshooting and best practices
  - Resources for continued learning

---

Notes:
- Each part is approximately 1 hour
- Participants create the {praiseme} package step-by-step
- Emphasizes hands-on practice following the book materials
- By the end, you'll have a working, documented, tested package on GitHub
