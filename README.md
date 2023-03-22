# Webhook Validator

This program checks if a given Discord webhook URL is valid or not by making a GET request to it and checking the response code.

## Prerequisites

This program requires `libcurl` to be installed on your system. If you're using a Debian-based Linux distribution, you can install it by running:

```
sudo apt-get install libcurl4-openssl-dev
```

## Usage

1. Clone this repository or download the source code.
2. Compile the code using your preferred C++ compiler. For example, if you're using `g++`, you can run:
```
g++ -o webhook-validator webhook-validator.cpp -lcurl
```

3. Run the compiled binary and enter the webhook URL when prompted:

```
./webhook-validator
webhook url >: https://discord.com/api/webhooks/123456789012345678/abcdefghijklmnopqrstuvwxyz
Valid webhook FR
```

If the webhook URL is invalid, the program will print an error message and exit with a non-zero status code.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

