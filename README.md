# Tiptel and Yealink image converter

This tool converts images to .dob files to use as logo in Tiptel and Yealink phones. All images will be converted
to 16 level grayscale (The phones support more than the 2 level grayscale mentioned in the manual)

## Supported phones

- Tiptel IP 286
- Tiptel IP 284
- Tiptel IP 282
- Yealink T10T
- Yealink T12
- Yealink T22
- Yealink T26
- Yealink T28
- Yealink T80

## Dependencies

- python3
- pillow

## Usage

```bash
# Convert logo to .dob without resizing
$ ./convert.py logo.png logo.dob

# Convert logo to .dob for a Tiptel IP 286
$ ./convert.py -p ip286 logo.png logo.dob

# Convert .dob back to a .png
$ ./convert.py -r logo.dob logo.png
```