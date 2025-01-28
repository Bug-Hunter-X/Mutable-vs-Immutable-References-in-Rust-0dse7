This repository contains a simple Rust program that showcases a common error involving mutable and immutable references.  The `bug.rs` file demonstrates the error, while `bugSolution.rs` provides a corrected version.

The core issue revolves around trying to create both a mutable reference (`&mut x`) and an immutable reference (`&x`) to the same variable (`x`) simultaneously.  Rust's borrow checker prevents this to ensure data consistency and avoid race conditions.  The solution involves careful management of borrowing scopes.