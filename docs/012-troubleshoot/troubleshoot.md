---
// filepath: kubernetes/docs/012-troubleshoot/README.md
sidebar_label: "Troubleshooting Kubernetes Exit Codes"
sidebar_id: "troubleshooting-kubernetes-exit-codes"
sidebar_position: 1
---

# Troubleshooting Kubernetes Exit Codes

In Kubernetes, understanding exit codes is essential for diagnosing and resolving issues that arise within containers. Exit codes are returned by processes to indicate their success or failure. Each exit code has a specific meaning that helps developers troubleshoot problems efficiently.

## What are Exit Codes?
Exit codes are numerical values returned by a process when it terminates. They indicate whether the process executed successfully or encountered an error. A zero exit code typically means success, while any non-zero exit code indicates a failure, with specific codes signifying different types of errors.

## Why Do We Get Exit Codes?
Exit codes are generated by the underlying operating system and are often the result of various factors, such as:
- Command syntax errors
- Resource limitations (e.g., memory or CPU)
- Signal termination
- Application-specific errors

By understanding the exit codes, you can identify the root cause of issues and take corrective action.

## Exit Code Reference Table
Below is a list of common exit codes, their meanings, and links to hands-on examples available in this repository:

| Exit Code | Meaning                                      | Reference                                         |
|-----------|----------------------------------------------|--------------------------------------------------|
| 0         | Success                                      | [Exit Code 0](./exit-code-0/exit-code-0.md)         |
| 1         | Generic error                                | [Exit Code 1](./exit-code-1/exit-code-1.md)         |
| 2         | Misuse of shell builtins                     | [Exit Code 2](./exit-code-2/exit-code-2.md)         |
| 125       | Command invoked cannot execute               | [Exit Code 125](./exit-code-125/exit-code-125.md)     |
| 126       | Command invoked cannot execute (permission)  | [Exit Code 126](./exit-code-126/exit-code-126.md)     |
| 127       | Command not found                            | [Exit Code 127](./exit-code-127/exit-code-127.md)     |
| 128       | Invalid exit argument                        | [Exit Code 128](./exit-code-128/exit-code-128.md)     |
| 130       | Script terminated by Control-C              | [Exit Code 130](./exit-code-130/exit-code-130.md)     |
| 134       | Abnormal termination (SIGABRT)              | [Exit Code 134](./exit-code-134/exit-code-134.md)     |
| 137       | Container killed by OOM (Out of Memory)     | [Exit Code 137](./exit-code-137/exit-code-137.md)     |
| 139       | Segmentation fault (SIGSEGV)                | [Exit Code 139](./exit-code-139/exit-code-139.md)     |
| 141       | Broken pipe (SIGPIPE)                       | [Exit Code 141](./exit-code-141/exit-code-141.md)     |
| 143       | Graceful termination (SIGTERM)              | [Exit Code 143](./exit-code-143/exit-code-143.md)     |
| 255       | Exit status out of range                    | [Exit Code 255](./exit-code-255/exit-code-255.md)     |

## Detailed Information on Each Exit Code
For detailed hands-on examples and simulations for each exit code, please refer to the individual README files linked above. Each of these files provides:
- An explanation of the exit code
- Sample Kubernetes manifests for simulating the exit code
- Suggested fixes for resolving issues associated with the exit code
- Prevention strategies for avoiding similar issues in the future

By utilizing these resources, you can enhance your understanding of Kubernetes troubleshooting and improve your ability to manage containerized applications effectively.
