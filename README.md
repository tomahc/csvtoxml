### What it does

Create XML Documents from CSV files with jinjas template engine and zip them.

### Arguments

```
usage: csvtoxml [-h] [-i CSV] [-o XML] [-s Selector] [-e num_of_elements]

optional arguments:
  -h, --help            show this help message and exit
  -i CSV, --infile CSV
  -o XML, --outfile XML
  -s Selector, --selector selector
  -e elements, --elements num_of_elements		Elements per file
```

```csvtoxml -s selector```

_selector_ can be either a file, or a template name. In any case: Template name is mandatory.

If _selector_ is a file, CSV headers can be selected by using:
```
::template_name
csv_header1
csv_header2
csv_header3
```

If _selector_ is a template name, the whole CSV file will be parsed.

```csvtoxml -e num_of_elements```

Every XML will be created with _num_of_elements_ in it.

```csvtoxml -o XML```

XML filename will be incremented from None to n.
