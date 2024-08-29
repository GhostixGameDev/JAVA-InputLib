---

# ConsoleReader

The `ConsoleReader` class is part of the `ar.com.ghostix.lib.inputLib` package. It provides a convenient way to read various types of input from the console, with optional user confirmation. This class is designed to handle input for several data types, including `String`, `int`, `double`, `float`, `boolean`, `long`, `byte`, `short`, `BigDecimal`, and `BigInteger`.

## Features

- Read input for various data types.
- Optional user confirmation for the input.
- Customizable prompts for user interaction.
- No external dependencies.

## Installation

To use the `ConsoleReader` class in your project, simply copy the source code into your project.

## Usage

Here's an example of how to use the `ConsoleReader` class to read an integer value from the console:

```java
import ar.com.ghostix.lib.inputLib.ConsoleReader;

public class Main {
    public static void main(String[] args) {
        ConsoleReader consoleReader = new ConsoleReader();
        int foo = consoleReader.input("Insert a number: ", 0, true); // Asks the user for an integer value and asks for confirmation.
        System.out.println("You entered: " + foo);
    }
}
```

## Constructors

### `ConsoleReader()`
Creates a `ConsoleReader` object with the default `System.in` input stream.

### `ConsoleReader(Scanner scan)`
Creates a `ConsoleReader` object with a custom `Scanner` object.

- **Parameters:**
  - `scan`: A custom `Scanner` object to use for input.

### `ConsoleReader(InputStream inputStream)`
Creates a `ConsoleReader` object with a custom `InputStream`.

- **Parameters:**
  - `inputStream`: A custom `InputStream` to use for input.

## Methods

### `<T> boolean askConfirmation(T value)`
Asks the user for confirmation on a given input value.

- **Parameters:**
  - `value`: The value to be confirmed.
- **Returns:**
  - `true` if the user confirms (`S`), `false` otherwise.

### `String input(String prompt, boolean askForUserConfirmation)`
Reads a `String` from the console with an optional confirmation.

- **Parameters:**
  - `prompt`: The prompt to display to the user.
  - `askForUserConfirmation`: Whether to ask for user confirmation.
- **Returns:**
  - The inputted `String`.

### `String input(String prompt, boolean askForUserConfirmation, boolean lineJump)`
Reads a `String` from the console with an optional confirmation and handles line jumps.

- **Parameters:**
  - `prompt`: The prompt to display to the user.
  - `askForUserConfirmation`: Whether to ask for user confirmation.
  - `lineJump`: Whether to handle line jumps.
- **Returns:**
  - The inputted `String`.

### `int input(String prompt, int input, boolean askForUserConfirmation)`
Reads an `int` from the console with an optional confirmation.

- **Parameters:**
  - `prompt`: The prompt to display to the user.
  - `input`: The default input value.
  - `askForUserConfirmation`: Whether to ask for user confirmation.
- **Returns:**
  - The inputted `int`.

### `double input(String prompt, double input, boolean askForUserConfirmation)`
Reads a `double` from the console with an optional confirmation.

- **Parameters:**
  - `prompt`: The prompt to display to the user.
  - `input`: The default input value.
  - `askForUserConfirmation`: Whether to ask for user confirmation.
- **Returns:**
  - The inputted `double`.

### `float input(String prompt, float input, boolean askForUserConfirmation)`
Reads a `float` from the console with an optional confirmation.

- **Parameters:**
  - `prompt`: The prompt to display to the user.
  - `input`: The default input value.
  - `askForUserConfirmation`: Whether to ask for user confirmation.
- **Returns:**
  - The inputted `float`.

### `boolean input(String prompt, Boolean input, boolean askForUserConfirmation)`
Reads a `boolean` from the console with an optional confirmation.

- **Parameters:**
  - `prompt`: The prompt to display to the user.
  - `input`: The default input value.
  - `askForUserConfirmation`: Whether to ask for user confirmation.
- **Returns:**
  - The inputted `boolean`.

### `long input(String prompt, long input, boolean askForUserConfirmation)`
Reads a `long` from the console with an optional confirmation.

- **Parameters:**
  - `prompt`: The prompt to display to the user.
  - `input`: The default input value.
  - `askForUserConfirmation`: Whether to ask for user confirmation.
- **Returns:**
  - The inputted `long`.

### `byte input(String prompt, byte input, boolean askForUserConfirmation)`
Reads a `byte` from the console with an optional confirmation.

- **Parameters:**
  - `prompt`: The prompt to display to the user.
  - `input`: The default input value.
  - `askForUserConfirmation`: Whether to ask for user confirmation.
- **Returns:**
  - The inputted `byte`.

### `short input(String prompt, short input, boolean askForUserConfirmation)`
Reads a `short` from the console with an optional confirmation.

- **Parameters:**
  - `prompt`: The prompt to display to the user.
  - `input`: The default input value.
  - `askForUserConfirmation`: Whether to ask for user confirmation.
- **Returns:**
  - The inputted `short`.

### `BigDecimal input(String prompt, BigDecimal input, boolean askForUserConfirmation)`
Reads a `BigDecimal` from the console with an optional confirmation.

- **Parameters:**
  - `prompt`: The prompt to display to the user.
  - `input`: The default input value.
  - `askForUserConfirmation`: Whether to ask for user confirmation.
- **Returns:**
  - The inputted `BigDecimal`.

### `BigInteger input(String prompt, BigInteger input, boolean askForUserConfirmation)`
Reads a `BigInteger` from the console with an optional confirmation.

- **Parameters:**
  - `prompt`: The prompt to display to the user.
  - `input`: The default input value.
  - `askForUserConfirmation`: Whether to ask for user confirmation.
- **Returns:**
  - The inputted `BigInteger`.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---
