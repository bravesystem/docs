# BRaVe Documentation

The Documentation portal for the BRaVe - an open-source tool for humanitarian registration, deduplication, assistance, and referral.

> [!NOTE]  
> Currently the documentation requires Quarto to be installed locally and to be rendered locally before pushing changes. An upcoming release will render through CI, whic will failitate content updates through the web interface without requiring a local rendering.


## Prerequisites

Before edit or rendering the docs, ensure you have the Quarto tool installed; a package manager for your code along with the packages you need installed; and a text editor or IDE that supports Quarto.

To set up your development environment using the Pixi tool, run the following:

Install Pixi on Windows:
```powershell
powershell -ExecutionPolicy ByPass -c "irm -useb https://pixi.sh/install.ps1 | iex"
```

Install Pixi on MacOS:
```bash
curl -fsSL https://pixi.sh/install.sh | bash
```

Install Quarto:
```bash
pixi global install quarto
```


## Contributing

To update the documentation, edit the *.qmd* files. 
To preview your edits run 
```bash
quarto preview
```
To render the documentation to the *docs/* folder run
```bash
quarto render
```
Once rendered, commit and push your changes to the repository.

The documentation follows the [diátaxis](https://diataxis.fr/) model, which includes four types of content: tutorials, how-to guides, reference, and explanations. When contributing, please ensure that your additions or modifications align with these categories.

## Troubleshooting
If you encounter any issues while working with the documentation, please refer to the [Quarto Documentation](https://quarto.org/docs/) for guidance or open an issue in the repository for assistance.

If you add pages, make sure they are included in the ```_quarto.yml``` file under *render*.
