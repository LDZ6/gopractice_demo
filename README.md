# Go Practice Examples Collection

[![Go Version](https://img.shields.io/badge/Go-1.15+-blue.svg)](https://golang.org)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

This repository is a comprehensive collection of Go language practice examples, covering commonly used frameworks, tools, and best practices in Go development. Suitable for Go developers to learn and reference.

## 📚 Table of Contents

- [Introduction](#introduction)
- [Project Structure](#project-structure)
- [Quick Start](#quick-start)
- [Example Modules](#example-modules)
- [Requirements](#requirements)
- [Usage](#usage)
- [Contributing](#contributing)

## Introduction

This is a carefully organized Go language learning and practice project that includes the following core content:

- 🚀 Web Framework Practice (Gin)
- 📝 Logging Libraries (glog, logrus, zap, custom logging)
- 🔧 CLI Tool Development (Cobra, pflag)
- 📊 API Design & Documentation (Swagger, gRPC)
- 🧪 Testing & Debugging (GoMock, Fuzzing, Delve, pprof)
- 🗄️ Database Operations (GORM)
- ⚙️ Configuration Management (Viper)
- 🔐 Access Control (Ladon)
- ⏰ Scheduled Tasks (Cron)
- 🎯 Design Patterns & SOLID Principles
- ❌ Error Handling Best Practices
- 🔄 Distributed Locks (Redsync)

## Project Structure

```
gopractise-demo/
├── apistyle/           # API design style examples
│   ├── greeter/        # gRPC Greeter service example
│   └── ping/           # Simple ping service
├── cobra/              # Cobra CLI framework examples
│   ├── demoapp/        # Demo application
│   └── newApp2/        # Second demo application
├── cron/               # Cron scheduled task examples
├── delve/              # Delve debugger examples
├── errors/             # Error handling best practices
├── fuzz/               # Fuzzing test examples
├── gin/                # Gin web framework examples
│   ├── cookie/         # Cookie handling
│   ├── custom_log_format/  # Custom log format
│   ├── graceful/       # Graceful shutdown
│   ├── http-configuration/ # HTTP configuration
│   ├── log/            # Logging integration
│   ├── middleware/     # Middleware examples
│   ├── multiple-service/   # Multiple service examples
│   ├── parse/          # Parameter parsing
│   ├── redirect/       # Redirect handling
│   └── webfeature/     # Web feature examples
├── gomock/             # GoMock testing framework examples
├── gorm/               # GORM ORM framework examples
├── graceful/           # Graceful service shutdown examples
├── interface/          # Interface usage examples
├── ladon/              # Ladon access control framework
│   ├── condition/      # Conditional policies
│   └── policy/         # Policy management
├── log/                # Logging library examples collection
│   ├── cuslog/         # Custom logging library
│   ├── glog/           # glog usage examples
│   ├── logrus/         # Logrus usage examples
│   ├── std/            # Standard library logging
│   └── zap/            # Zap high-performance logging
├── makefile/           # Makefile usage examples
├── modules/            # Go Modules examples
├── oop/                # Object-oriented programming examples
├── pflag/              # pflag command-line argument parsing
├── pprof/              # Performance profiling examples
├── protobuf/           # Protocol Buffers examples
├── redsync/            # Redis distributed lock examples
├── SOLID/              # SOLID design principles examples
│   ├── lsp/            # Liskov Substitution Principle
│   └── srp/            # Single Responsibility Principle
├── swagger/            # Swagger API documentation examples
├── test/               # Unit testing examples
├── testable/           # Testable code design examples
└── viper/              # Viper configuration management examples
```

## Requirements

- Go 1.15 or higher
- Git
- (Optional) Docker - for running certain dependency services

## Quick Start

### 1. Clone the Repository

```bash
git clone https://github.com/marmotedu/gopractise-demo.git
cd gopractise-demo
```

### 2. Install Dependencies

```bash
go mod download
```

### 3. Run Examples

Each subdirectory contains independent example programs that can be run separately:

```bash
# Run Gin web example
cd gin
go run example.go

# Run Viper configuration management example
cd viper
go run main.go

# Run Cobra CLI example
cd cobra/demoapp
go run main.go
```

## Example Modules

### 🌐 Web Development

#### Gin Framework
- **Basic Example**: [gin/example.go](gin/example.go) - Gin framework basics
- **Middleware**: [gin/middleware/](gin/middleware/) - Custom and built-in middleware
- **Graceful Shutdown**: [gin/graceful/](gin/graceful/) - Graceful service shutdown
- **Logging Integration**: [gin/log/](gin/log/) - Logging middleware integration
- **Multiple Services**: [gin/multiple-service/](gin/multiple-service/) - Running multiple services simultaneously

### 📝 Logging

Provides usage examples for various logging libraries:

- **Standard Library Logging**: [log/std/](log/std/)
- **glog**: [log/glog/](log/glog/) - Google's logging library
- **Logrus**: [log/logrus/](log/logrus/) - Structured logging
- **Zap**: [log/zap/](log/zap/) - Uber's high-performance logging library
- **Custom Logging**: [log/cuslog/](log/cuslog/) - Custom logging implementation

### 🔧 CLI Tool Development

- **Cobra**: [cobra/](cobra/) - Powerful CLI application framework
- **pflag**: [pflag/](pflag/) - POSIX/GNU-style command-line argument parsing

### 🗄️ Database

- **GORM**: [gorm/](gorm/) - Go ORM library usage examples

### ⚙️ Configuration Management

- **Viper**: [viper/](viper/) - Complete configuration solution
  - Supports multiple configuration formats (JSON, YAML, TOML, etc.)
  - Environment variable reading
  - Configuration hot-reloading

### 🧪 Testing & Debugging

- **Unit Testing**: [test/](test/) - Unit testing best practices
- **GoMock**: [gomock/](gomock/) - Mock testing framework
- **Fuzzing**: [fuzz/](fuzz/) - Fuzzing test examples
- **Performance Profiling**: [pprof/](pprof/) - CPU and memory profiling
- **Debugging Tools**: [delve/](delve/) - Delve debugger usage

### 📊 API Design

- **Swagger**: [swagger/](swagger/) - Automatic API documentation generation
- **gRPC**: [apistyle/greeter/](apistyle/greeter/) - gRPC service examples
- **Protocol Buffers**: [protobuf/](protobuf/) - Protobuf usage examples

### ❌ Error Handling

The [errors/](errors/) directory contains best practices for Go error handling:

- Error creation and wrapping
- Error chain tracking
- Custom error types
- Error logging

### 🎯 Design Patterns & Principles

- **SOLID Principles**: [SOLID/](SOLID/)
  - Single Responsibility Principle (SRP)
  - Liskov Substitution Principle (LSP)
- **Object-Oriented Programming**: [oop/](oop/) - OOP practices in Go
- **Interface Design**: [interface/](interface/) - Interface usage examples
- **Testable Code**: [testable/](testable/) - Writing testable code

### 🔄 Distributed & Concurrency

- **Distributed Locks**: [redsync/](redsync/) - Redis-based distributed locks
- **Scheduled Tasks**: [cron/](cron/) - Cron job scheduling

### 🔐 Access Control

- **Ladon**: [ladon/](ladon/) - Access control policy engine
  - Policy management
  - Conditional evaluation

## Usage

### Running Specific Examples

Most examples can be run independently. Here are some common ways to run them:

```bash
# Gin web service
cd gin/graceful
go run main.go

# Viper configuration management
cd viper
go run main.go

# Cobra CLI tool
cd cobra/demoapp
go build -o demoapp
./demoapp --help

# Run tests
cd test
go test -v

# Performance profiling
cd pprof
go run pprof.go
```

### Exploring Examples

Each module directory contains corresponding code examples. We recommend learning in the following order:

1. Basic syntax and features (modules/, interface/, oop/)
2. Error handling (errors/)
3. Logging (log/)
4. Web development (gin/)
5. CLI tools (cobra/, pflag/)
6. Testing (test/, gomock/, testable/)
7. Database and configuration (gorm/, viper/)
8. API design (swagger/, apistyle/)
9. Distributed and advanced features (redsync/, ladon/)

## Contributing

Contributions are welcome! If you have good examples or improvement suggestions:

1. Fork this repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details

## Related Resources

- [Official Go Documentation](https://golang.org/doc/)
- [Effective Go](https://golang.org/doc/effective_go)
- [Go Design Patterns](https://github.com/tmrts/go-patterns)
- [Awesome Go](https://github.com/avelino/awesome-go)

## Contact

For questions or suggestions, feel free to submit an Issue or Pull Request.

---

⭐ If this project helps you, please give it a Star!
