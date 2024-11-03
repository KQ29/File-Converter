# File Converter

A Python-based tool for converting various file formats, such as Word documents, text files, images, PDFs, and more. This tool simplifies file conversions, allowing users to input a file path and automatically get the converted output in the desired format.

## Features

- Convert `.docx` (Word) to `.pdf`
- Convert `.txt` (Text) to `.pdf`
- Convert `.png` (Image) to `.jpeg`
- Convert `.jpeg` to `.png`
- Convert `.pdf` to `.pptx`
- Convert `.xlsx` (Excel) to `.pdf`
- Convert `.html` to `.pdf`

## Prerequisites

- Python 3.6 or higher
- Virtual environment (`venv`) is recommended for managing dependencies

## Installation

1. **Clone the Repository**:

    ```bash
    git clone https://github.com/KQ29/File-Converter.git
    cd File-Converter
    ```

2. **Set Up Virtual Environment**:

    ```bash
    python3 -m venv env
    source env/bin/activate  # On Windows, use `env\Scripts\activate`
    ```

3. **Install Dependencies**:

    Install the required libraries using the `requirements.txt` file:

    ```bash
    pip install -r requirements.txt
    ```

4. **Additional Requirements**:

    - Install `wkhtmltopdf` for HTML to PDF conversion:

        - On macOS:

            ```bash
            brew install wkhtmltopdf
            ```

        - On other systems, download and install from [wkhtmltopdf website](https://wkhtmltopdf.org/downloads.html).

## Usage

1. **Run the Script**:

    ```bash
    python File_converter.py
    ```

2. **Enter the Path of the File You Want to Convert**:

    When prompted, input the path to the file you want to convert. The script will detect the file type and perform the appropriate conversion.

    Example:

    ```plaintext
    Enter the path of the file you want to convert: /path/to/your/file.docx
    ```

## Supported Conversions

| Input Format | Output Format | Library Used    |
|--------------|---------------|-----------------|
| `.docx`      | `.pdf`        | `docx2pdf`      |
| `.txt`       | `.pdf`        | `fpdf`          |
| `.png`       | `.jpeg`       | `Pillow`        |
| `.jpeg`      | `.png`        | `Pillow`        |
| `.pdf`       | `.pptx`       | `pdf2image`, `python-pptx` |
| `.xlsx`      | `.pdf`        | `pandas`, `pdfkit` |
| `.html`      | `.pdf`        | `pdfkit`        |

## Example Code Structure

- **File_converter.py** - Main script that contains all conversion functions and handles file input.
- **requirements.txt** - Lists all dependencies required for the project.

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests with improvements or new features.

1. Fork the repository
2. Create a new branch (`git checkout -b feature-branch`)
3. Commit your changes (`git commit -m 'Add new feature'`)
4. Push to the branch (`git push origin feature-branch`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Thanks to the creators of `docx2pdf`, `pdfkit`, `Pillow`, `fpdf`, `pdf2image`, and `python-pptx` libraries for making this project possible.
- [wkhtmltopdf](https://wkhtmltopdf.org/) for HTML to PDF conversion support.