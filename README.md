<h1 align="center">Pipex</h1>
<h4>For this project we will have to replicate a mecanism from UNIX, specifically "pipes"</h4>

## 📚 Mandatory Part 📚

- **Name of the program** : `pipex`
- **Files** : [`pipex.c`](./src/pipex.c) [`error.c`](./src/error.c) [`free.c`](./src/free.c) [`process.c`](./src/process.c) [`pipex.h`](./includes/pipex.h) [`extras`](./extra) [`Makefile`](./Makefile)
- **Makefile rules** : `all` `clean` `fclean` `re`
- **Authorized functions** : [`access`](https://linux.die.net/man/2/access) [`open`](https://man7.org/linux/man-pages/man2/open.2.html) [`unlink`](https://man7.org/linux/man-pages/man2/unlink.2.html) [`close`](https://linux.die.net/man/2/close) [`read`](https://man7.org/linux/man-pages/man2/read.2.html) [`write`](https://man7.org/linux/man-pages/man2/write.2.html) [`malloc`](https://www.tutorialspoint.com/c_standard_library/c_function_malloc.htm) [`waitpid`](http://manpages.ubuntu.com/manpages/bionic/es/man2/wait.2.html) [`wait`](http://manpages.ubuntu.com/manpages/bionic/es/man2/wait.2.html) [`free`](https://www.tutorialspoint.com/c_standard_library/c_function_free.htm) [`pipe`](https://www.programacion.com.py/escritorio/c/pipes-en-c-linux) [`dup`](https://baulderasec.wordpress.com/programacion/programacion-con-linux/3-trabajando-con-los-archivos/acceso-de-bajo-nivel-a-archivos/dup-y-dup2/) [`dup2`](https://baulderasec.wordpress.com/programacion/programacion-con-linux/3-trabajando-con-los-archivos/acceso-de-bajo-nivel-a-archivos/dup-y-dup2/) [`execve`](https://man7.org/linux/man-pages/man2/execve.2.html) [`fork`](https://www.geeksforgeeks.org/fork-system-call/) [`perror`](http://www.w3big.com/es/cprogramming/c-function-perror.html) [`strerror`](http://www.w3big.com/es/cprogramming/c-function-strerror.html) [`exit`](https://www.tutorialspoint.com/c_standard_library/c_function_exit.htm)

## 🔥 USAGE 🔥
#### Compiling the `pipex` file should be as easy as run `make` inside the pipex folder. You should execute the `pipex`program like this:
#### `$> ./pipex file1 command1 commmand2 file2`
#### Where:

- `file1` is the input file.
- `command1` is the first command you would like to execute on the `file1`.
- `command2` is the second command you would like to execute on the `command1` output.
- `file2` is where the `command2` output is saved. If `file2` does not exist when you run the command, `pipex`should create it.

### The execution of the pipex program shoul replicate the next shell command:
#### `$> file1 command1 | command2 > file2`

## 💣 EXAMPLES 💣

### The command:
### `./pipex infile "ls -l" "wc -l" outfile`
### Should do the same as:
### `<infile ls -l | wc -l >outfile`

## 💯 Mark 💯

<p align="center">
  <a align="center">
    <img src="./Addings/Mark.png">
  </a>
</p>
