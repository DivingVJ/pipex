### pipex
Summary: The purpose of this project is to code the shell pipe | in C

The function is to be executed:
> pipex file1 cmd1 cmd2 file2

to emulate:

> < file1 cmd1 | cmd2 > file2

| Functions | Prototype | Description |
|---|---|---|
| access   | int access(const char *pathname, int mode) | checks if the calling process can access the pathname |
| open     | int open(const char *pathname, int flags) | opens file returns fd |
| unlink   | int unlink(const char *pathname) | deletes name from the filesystem |
| close    | int close(int fd) | closes a fie descriptor |
| read     | ssize_t read(int fd, void *buf, size_t count) | read from file descriptor into buf |
| write    | ssize_t write(int fd, const void *buf, size_t count) | writes to file from buf |
| malloc   | void *malloc(size_t size) | allcates memory in the heap for usage |
| waitpid  | pid_t waitpid(pid_t pid, int *stat_loc, int options) | suspends execution of the calling process until a child process has changed state |
| wait     | pid_t wait(int *status) | suspends execution of the calling process until one of its children terminates |
| free     | void free(void *ptr) |  frees the memory space pointed to by ptr |
| pipe     | int pipe(int pipefd[2]) | creates a pipe, a unidirectional data channel |
| dup      | int dup(int fildes) | duplicate an open file descriptor |
| dup2     | int dup2(int fildes, int fildes2) | duplicate an open file descriptor  fildes to fildes2 |
| execve   | int execve(const char *filename, char *const argv[], char *const envp[]) | executes the program pointed to by filename |
| fork     | pid_t fork(void) | creates a new process by duplicating the calling process |
| perror    | void perror(const char *s) | produces a message on the standard error output |
| strerror | char *strerror(int errnum) | returns a pointer to a string that describes the error code passed in the argument |
| exit     | void exit(int status) | terminates the calling process "immediately" |

## The Plan (for now)
- [ ] Research definitions of functions allowed
- [ ] Research pipe usage (aka how to use a pipe)
