# Peugeot 2008
This repository contains signal set configurations for the Peugeot 2008, organized by model year and version. The files are structured to allow for easy differentiation between model phases and other vehicle parameters, ensuring accurate signal mapping for each version of the Peugeot 2008.

## About Peugeot 2008 Phases
The Peugeot 2008 has undergone two main design phases:

- **Phase I (2013-2019)**: The original Peugeot 2008 was launched in 2013 as a subcompact crossover, based on the Peugeot 208 platform. It featured a sleek design, compact size, and came with various engine options including petrol and diesel. This phase set the groundwork for Peugeot's crossover SUV lineup.

- **Phase II (2020-present)**: In 2019, Peugeot introduced a redesigned 2008, marking the beginning of Phase II. This model brought a more rugged, angular look, aligning with Peugeot's modern design language. It also introduced an electric variant, the e-2008, making it one of Peugeot’s first electrified crossovers. This phase continues to support various internal combustion engines as well as the fully electric option.

## Repository Structure
The directory is organized as follows:

```plaintext
signalsets/
  └── v3/
      ├── default.json        # Default configuration (applies to Phase 2 and future models)
      └── 2013-2019.json      # Override configuration for Phase 1 (2013-2019)
```
- **default.json**: Acts as the primary configuration file, covering models from 2020 onwards (Phase II). This file will serve as the default fallback for any years not specified by an override file.

- **2013-2019.json**: A specific configuration override for Phase I models (2013-2019), differentiating these years from the baseline configuration in `default.json`.

If a new configuration is required in the future (e.g., for model years 2028 and beyond), a new JSON file (e.g., `2020-2027.json`) can be created to lock in the 2020-2027 model configuration, allowing `default.json` to reflect the latest specifications.

## Usage
Each JSON file in the `v3/` directory corresponds to a specific model year range. This structure enables compatibility with various vehicle parameters and model phases. If new versions of the Peugeot 2008 are released, they can be easily integrated by adding new JSON files, e.g., `2025+.json`.

## Contributing

Contributions are welcome! If you would like to add support for additional model years or other configurations, please open an issue or submit a pull request.

1. Fork the repository
2. Create a new branch for your changes
3. Commit your changes and open a pull request with a detailed description

## Issues

If you encounter any issues or would like to discuss improvements, please feel free to open an issue. We encourage collaboration and appreciate feedback to make the repository as accurate and useful as possible.