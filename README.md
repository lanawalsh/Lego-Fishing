# Lego-Fishing
Project Aim: The aim of our project is to create a program that sorts lego pieces based on shape and colour using image processing. We chose this project because it offers a fun and visually engaging way to apply key image processing principles in a practical, real-world context. As a team of big Lego fans, we wanted to combine our love of building and creativity with technical problem-solving.

## Individual Work
<h4>Segmentation</h4>
<h5>Loredana Bura</h5>
<p>Segmentation is the first step </p>
<h4>Colour Classification</h4>
<h5>Alannah Walsh</h5>
<p>This section focuses on analysing each segmented LEGO block to determine its dominant colour.The process begins by converting the image from RGB to HSV (Hue, Saturation, Value) color space, which is more robust to lighting variations than RGB since similar colors have comparable hue values regardless of brightness changes. </p>
<p>For each isolated brick, the program creates a bounding box and applies a precise mask to analyse only the pixels belonging to that specific piece, ignoring the background. The system then compares the HSV values of each pixel against predefined color ranges (such as red, blue, yellow, green) and counts how many pixels fall within each range. The color with the highest pixel count above a minimum threshold is designated as the brick's dominant color, while colors below the threshold are ignored to prevent misclassification from shadows or reflections.</p> 
<p>Finally, the results are displayed visually through bar charts showing the distribution of detected colors, allowing for easy verification of the classification accuracy.</p>
<h4>Feature Extraction</h4>
<h5>Gráinne Bannister</h5>
<p>...</p>



## Output
