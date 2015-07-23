# PyMSN #
PyMSN is a Python script that translates old-fashioned XML MSN Messenger logfiles
to lovely readable HTML files. It's easily customizable, as the basic CSS stylesheet
is ready to customize! If you're familiar with Python, you're also going to find
it very easy to customize.

## Usage ##
PyMSN can translate a single file or all the XML files contained in a directory:

    $ ./pymsn.py /path/to/file.xml

Or:

    $ ./pymsn.py /path/to/directory

Note that you should **NOT** add a slash (/) after the directory name.

There are also two flags available: `--no-style` and `--no-date`. The former will
use the style defined in the CSS stylesheet in the messages, instead of the user-defined
styles that are embedded into the XML files, while the latter will generate an HTML
file without appending the date and time of sent messages next to the sender's name.

Example of use, if you wanted to translate the file 'convo.xml' without custom styling:

    $ ./pymsn.py convo.xml --no-style


(**IMPORTANT NOTE**) The script needs to have permission to read and write the
file(s) that are going to be processed (obviously).
