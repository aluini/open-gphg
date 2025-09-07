# Open GPHG

This project contains results data for the Grand Prix d'Horlogerie de Genève (GPHG).

## Project Structure
- `results.json`: Contains the results data for each GPHG edition in JSON format. The structure is as follows:
   - An array of objects, each representing a GPHG edition (e.g., `"edition": "2001"`).
   - Each edition has a list of `categories` (e.g., Complicated Watch, Jewelry Watch).
   - Each category includes:
      - `name`: The category name in English.
      - `original_name`: The original name of the category.
      - `watches`: An array of watches nominated in that category.
         - Each watch entry includes:
            - `name`: The watch model.
            - `brand`: The manufacturer.
            - `brand_group`: The group the brand belongs to.
            - `brands`: An array with brand details (`name`, `role`, `group`).
            - `is_collaboration`: Boolean indicating if the watch is a collaboration.
            - `winner`: (optional) Boolean indicating if the watch won the category.

This structure allows for detailed analysis of GPHG results by year, category, brand, and watch.

## Getting Started
1. Clone the repository:
   ```zsh
   git clone https://github.com/aluini/open-gphg.git
   ```
2. Navigate to the project directory:
   ```zsh
   cd open-gphg
   ```

## Usage
- The `results.json` file can be used for data analysis, visualization, or integration into other projects.

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License
Specify your license here (e.g., MIT, GPL, etc.).
