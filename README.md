# argv-fortran

A better `get_command_argument` for Fortran that returns the argument in an allocatable character string.

### Usage

To use `argv-fortran` within your fpm project, add the following to your `fpm.toml` file:
```toml
[dependencies]
argv-fortran = { git="https://github.com/jacobwilliams/argv-fortran.git" }
```

### Example

```fortran
program test

  use argv_module

  implicit none

  character(len=:),allocatable :: arg

  arg = argv(1) ! get the first argument

end program test
```

