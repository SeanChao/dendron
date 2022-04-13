---
id: kd3z6mvmw58qj0cmuy6nf9u
title: Logger
desc: ''
updated: 1649773502237
created: 1649773423598
---

## [simple_logger](https://docs.rs/simple_logger/2.1.0/simple_logger/)

`simple_logger = "2.1.0"`

```
// Just initialize logging without any configuration:
simple_logger::init().unwrap();
// Set the log level from the RUST_LOG environment variable:
simple_logger::init_with_env().unwrap();
// Hardcode a default log level:
simple_logger::init_with_level(log::Level::Warn).unwrap();
```
