# all-logging
Informative Repo explaining everything about logging

# SLF4J
* SLF4J is not a logging framework. It acts as an abstraction for other types of Java Logging frameworks.
* SLF4J lets us use the logging framework of our choice. We only have to provide the config which defines the log level, log format, log output etc., and our framework dependency. 
* By being framework-agnostic, SLF4J enables applications to switch to any Java framework interchangeably without impacting its implementations or doing any changes. 
* Because of this convenience, SLF4J is currently the most popular Java logging framework. 

# Logback
Logback is the successor of Log4J and it holds many improvements over Log4j in terms of its performance and native support to SLF4J. Some of the major improvements over Log4J are auto-reloading config files, filtering capabilities and automatic removal of old log archival. 

Logback comes with three core modules.
* logback-core
    - This is the base module that lays the foundation required by the below two modules. 
* logback-classic
    - This module contains an improved version of Log4j and also natively implements the SLF4J API
* logback-access
    - This module integrates with servlet containers such as tomcat and jetty allowing HTTP-access log function. 

# Log4j2
Log4j2 is the success of logback and in addition to logback features, it offers advanced features like lazy evaluation of log messages based on lambda expressions, asynchronous loggers and an option to disable garbage collector operations. 

# Comparison Summary

| Framework / Criteria                         | Log4j                                    | Logback                            | Log4j2                               |
|----------------------------------------------|------------------------------------------|------------------------------------|--------------------------------------|
| Flexibility                                  | Less Flexible                            | Less Flexible                      | Less Flexbile                        |
| Ease of use                                  | Easy to use                              | Easy to use when paired with SLF4J | Easy to use when paired with SLF4J   |
| Portability                                  | Less Portable                            | Less Portable                      | High Portability compared with Log4J |
| Maintainability                              | Not maintainable - Support discountinued | Highly Maintainable                | Highly Maintainable                  |
| Maintainability                              | Not maintainable - Support discountinued | Highly Maintainable                | Highly Maintainable                  |
| Popularity                                   | Less Popular                             | Not popular than LOG4J2            | Highly Popular                       |
| Supports Java Exceptions                     | Yes                                      | Yes                                | Yes                                  |
| Thread Safe                                  | Yes                                      | Yes                                | Yes                                  |
| Supports multiple log destinations           | Yes                                      | Yes                                | Yes                                  |
| Supports setting logging behavior at runtime | Yes                                      | Yes                                | Yes                                  |
| Supports multiple severity levels            | Yes                                      | Yes                                | Yes                                  |
| Native support for SLF4J                     | No                                       | Yes                                | Yes                                  |
| Automatic Log Rotation                       | No                                       | Yes                                | Yes                                  |
| Automatic Config File Reload                 | No                                       | Yes                                | Yes                                  |
| Advanced Filtering                           | No                                       | Yes                                | Yes                                  |
| Support for Lambda Expression evaluation     | No                                       | No                                 | Yes                                  |
| Support for low latency systems              | No                                       | No                                 | Yes                                  |
| Option to disable garbage collector          | No                                       | No                                 | Yes                                  |
