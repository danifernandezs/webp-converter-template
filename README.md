# Image Conversion Template

This repository serves as a template for image conversion projects. It includes a GitHub Action that automatically processes WebP images found in the `webp` directory, converting them to PNG and JPG formats, and organizing them into the appropriate directories.

## Features

- **Automatic Image Conversion:** Converts WebP images to PNG and JPG formats.
- **Directory Management:** Automatically creates necessary directories if they do not exist.
- **File Renaming:** Renames WebP files based on their modification date.
- **File Organization:** Moves original WebP files to `webp-originals` and cleaned up processed files.

## Directory Structure

- `webp/`: Directory where WebP images should be placed.
- `webp-originals/`: Directory where original WebP images are moved after processing.
- `png/`: Directory where converted PNG images are stored.
- `jpg/`: Directory where converted JPG images are stored.

## GitHub Action Workflow

The GitHub Action defined in this repository will:

1. **Install Dependencies:** Install necessary tools such as ImageMagick.
2. **Create Directories:** Ensure that `webp`, `webp-originals`, `png`, and `jpg` directories exist.
3. **Check for WebP Files:** If WebP files are found, proceed with processing.
4. **Rename Files:** Rename WebP files based on their modification date.
5. **Convert Images:** Convert WebP files to PNG and JPG formats.
6. **Move and Clean Up:** Move processed WebP files to `webp-originals` and clean up.

## Usage

1. **Add WebP Images:**
   - Place WebP images into the `webp/` directory.

2. **Push Changes:**
   - Push changes to the `main` branch of your repository.

3. **Automatic Processing:**
   - The GitHub Action will automatically process the images, convert them, and organize the files according to the workflow described.

4. **Check Results:**
   - The processed images will be available in the `png/` and `jpg/` directories, and the original WebP images will be moved to `webp-originals/`.

## Customization

Feel free to modify the GitHub Action workflow or directory structure as needed to fit the specific requirements of your project.

## License

This work is under [Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/).

Please read the [LICENSE](LICENSE) file for more details.
