# CIM RDF Validator

This project contains a Jupyter Notebook (`cim_rdf_validator.ipynb`) for validating CIM instance XML files against one or more RDFS profile files.

## Prerequisites

- **Python 3.7+**
- **Jupyter Notebook** or **JupyterLab**
- The following Python packages:
  - `ipywidgets`
  - `tkinter` (usually included with Python)
  - `lxml` (optional, for better XML parsing and line numbers)

Install required packages with:
```sh
pip install ipywidgets lxml
```

## How to Run

1. **Open the Notebook**
   - Launch Jupyter Notebook or JupyterLab:
     ```sh
     jupyter notebook
     ```
   - Navigate to the `RDF Validator` folder and open `cim_rdf_validator.ipynb`.

2. **Run the Notebook**
   - Execute the first code cell to initialize the UI.
   - Use the buttons to:
     - **Select CIM Instance**: Choose your CIM XML file.
     - **Add RDFS Profile(s)**: Select one or more RDFS profile files (XML or RDFS).
     - **Clear All Profiles**: Remove all selected profiles.
     - **Parse & Validate**: Run validation.

3. **View Results**
   - Validation status and detailed output will appear in the notebook output area.

## Notes

- The notebook uses `tkinter` dialogs for file selection. These will open native file dialogs.
- If `lxml` is not installed, validation will still work but line numbers for errors/warnings will not be shown.
- The notebook checks for schema compliance, multiplicities, datatypes, and enumerations.

## Troubleshooting

- If you see errors about missing modules, install them using `pip`.
- For issues with file dialogs on some platforms, ensure `tkinter` is properly installed.

## License

This project is for internal use and demonstration purposes.