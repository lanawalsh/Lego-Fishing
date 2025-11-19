# Lego-Fishing

## Project Overview

A program that sorts LEGO pieces based on shape and colour using image processing techniques. We chose this project because it offers a fun and visually engaging way to apply key image processing principles in a practical, real-world context. As a team of big Lego fans, we wanted to combine our love of building and creativity with technical problem-solving.

## How It Works

The system processes LEGO blocks through a three-stage pipeline:

1. **Segmentation** - Detects and isolates individual blocks from the background
2. **Color Classification** - Determines the dominant colour of each block
3. **Feature Extraction** - Identifies structural characteristics (e.g., number of studs)

## Pipeline Components

### 1. Segmentation 
**Loredana Bura**

Detects and separates individual LEGO blocks via adaptive thresholding, contour detection, and binary masking.  Adaptive thresholding responds to changing illumination conditions across the image, making detection more reliable.  Produces individual segmented blocks against a white background.

 ### 2. Color Classification 
 **Alannah Walsh**

Analyse each block in the HSV color space to discover the dominant colour. The HSV color system is more resistant to lighting fluctuations than RGB, as identical colours retain comparable hue values regardless of brightness.  Pixel values are compared to predetermined colour ranges and the number of pixels for each colour is counted.  The results are displayed using bar charts.  This component also aids in the separation of different-coloured touching blocks.

 ### 3. Feature Extraction 
 **Gráinne Bannister**

 Uses the Hough Circle Transform to detect and count circular studs on each block.  The Hough Circle Transform recognises circular structures by identifying edges and locating points that form circles with specific radii.  This information is used to categorise blocks by type.

## Limitations

- LEGO blocks cannot be white
- Blocks must be flat (not at an angle or overlapping)
- Blocks cannot be upside down
- Touching blocks must be different colours (same-colour touching blocks cannot be separated)

## Current Status

✅ All three pipeline stages integrated and working

Working on: Enhancing handling of touching blocks and implementing classification system

## Output

- Isolated mask for each block
- Dominant colour classification
- Number of circular studs
- Visual colour distribution charts

