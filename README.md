# Open GPHG

This project contains structured results data for the Grand Prix d'Horlogerie de Genève (GPHG).

## Project Structure

- `results.json`: Contains the results data for each GPHG edition in JSON format.  
  **Recent Update:**  
  The file now includes detailed structured data for the 2001 and 2002 editions, with categories and nominated watches, including winner flags and brand group information.

  **Data model:**
  - An array of objects, each representing a GPHG edition (e.g., `"edition": "2001"`).
  - Each edition has a list of `categories` (e.g., Complicated Watch, Jewellery, Men's, Ladies', Mechanical Clock, Geneva Seal, Aiguille d'Or Grand Prix, Design Watch, Ultra-Thin, Technical Innovation and Complication, etc.).
  - Each category includes:
    - `name`: The category name in English.
    - `original_name`: The original name of the category (in French).
    - `watches`: An array of watches nominated in that category.
      - Each watch entry includes:
        - `name`: The watch model.
        - `by`: The manufacturer.
        - `brands`: Array of brand details (`name`, `role`, `group`).
        - `is_collaboration`: Boolean indicating if the watch is a collaboration.
        - `winner`: (optional) Boolean indicating if the watch won the category.
        - `image`: (optional) URL to watch image.

This structure allows for detailed analysis of GPHG results by year, category, brand, and watch, including winner identification and brand group analysis.

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
- Example analyses:
  - Identify category winners for each year.
  - Visualize brand participation and group affiliation.
  - Extract images of nominated/winning watches.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License

Specify your license here (e.g., MIT, GPL, etc.).
