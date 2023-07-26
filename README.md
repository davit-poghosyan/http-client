# http-client

This is a simple cross-platform HTTP client implemented in C. 
It allows you to send HTTP GET requests to web servers and receive their responses.
The client supports both Windows and UNIX-based systems.

## Usage

  Clone the repository or download the source code.
  Compile the program using a C compiler (e.g., GCC on UNIX-based systems or Visual Studio on Windows).
  Run the executable with the URL as a command-line argument.

### Example

$ ./http http://www.example.com:80/res/page1.php?user=bob#account

## How it Works

The HTTP client consists of three main functions:

    parse_url: Parses the provided URL to extract the hostname, port, and path components.

    connect_to_host: Configures and establishes a TCP connection to the web server using the extracted hostname and port.

    send_request: Constructs an HTTP GET request and sends it to the server over the established connection.


  The program then waits for the server's response and displays the received HTTP headers and body on the console.
## Cross-Platform Support

  The HTTP client is designed to work on both Windows and UNIX-based systems. 
  It utilizes preprocessor directives to include the appropriate platform-specific header files and define macros for platform-specific functions.

## Limitations

This is a simplified implementation of an HTTP client and may not handle all HTTP response types or edge cases.
It does not support HTTPS, redirects, or other advanced features. 
The client is intended for educational purposes and as a starting point for more complex HTTP client implementations.
