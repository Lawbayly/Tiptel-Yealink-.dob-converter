# Tiptel and Yealink image converter

This tool converts images to .dob files to use as logo in Tiptel and Yealink phones. All images will be converted
to 16 level grayscale. The output is tested on a Tiptel IP 286. The display in these phones support 4 levels of grayscale (white, 2 levels of gray, black).


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
- Yealink T42
- Yealink T41
- Yealink T27
- Yealink T23
- Yealink T21
- Yealink CP860
- Yealink T19
- Yealink T53
- Yealink CP920
- Yealink T40

(Variations of the same handset e.g. T42G and T42S should have the same screen dimensions as T42 and therefore can use the same setting as T42)

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
