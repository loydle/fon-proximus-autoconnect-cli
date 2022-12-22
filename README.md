# Proximus Fon Autoconnect
This script automates the process of connecting to a Proximus Fon hotspot.

## Requirements

`curl` or `wget` must be installed on your system

## Usage

```
Usage: proximusfon [-u username] [-p password]

Options:
  -u, --username   The Fon username (default: your_username@proximus.be)
  -p, --password   The Fon password (default: your_password)
```

## Configuration

You can specify the Fon username and password either by using the `-u` and `-p` options when running the script, or by creating a configuration file called `.proximusfon.conf` in the same directory as the script, and adding the following lines to the file:

```
USERNAME='your_username@proximus.be'
PASSWORD='your_password'
```

The script will use the login credentials specified in the configuration file, if it exists, or it will use the default credentials specified in the script if the configuration file does not exist. If the `-u` and `-p` options are specified when running the script, they will override the credentials specified in the configuration file.

### Examples

To connect to a Proximus Fon hotspot using the default login credentials:

```
./proximusfon
```

To connect to a Proximus Fon hotspot using a different username and password:

```
./proximusfon -u my_username@proximus.be -p my_password
```
