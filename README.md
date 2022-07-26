# MASI Lab Programming Baseline
Programming exercise for prospective and/or new MASI Lab members

## Guidelines
- Use either Matlab or Python 3 to complete the following tasks. A Matlab Live Editor, Jupyter Notebook, or normal script are all acceptable; a starter program of each type is provided for you. 
- Remember to commit your code often (with descriptive commit messages) to keep a record of your problem solving process. Push your code to your repo fork and send us an email with a link to the forked repository when you're happy with your solution.
- There is no time limit to this assessment, but you should be able to comfortably complete it in 2-3 hours; we will be looking at your commit history to gauge how long it took you to complete each task.
- You may use the internet and/or reference books, but you may not ask for help from other people in creating your solution. 
- The purpose of this  assessment is not to challenge your programming prowess or trick you; it is simply to assess whether you have the basic programming experience necessary to be a productive member of the MASI lab.
- Good luck! :)

## Exercise Instructions
This exercise was designed to simulate a first-pass quality check of a new imaging dataset. This process generally includes 1) scanning image files to gather image meta data, 2) looking at the meta data to assess differences between images, and 3) looking at the image data itself to assess quality. 

You will be running a quality check on a dataset of pet pictures from the MASI lab! The only input to your code should be a file path to the directory containing an arbitrary number of pet pictures. Each image file follows the format "Pet name_Owner Initials.jpg" (note: not all images are JPEGs); if a file includes more than one pet name (example: 'Morris and Jackson_YT.jpg'), treat the entire string prior to the '_' as just a single pet name. **Do not hardcode the file paths to the individual images.**

### Task 1: Scan the image files to gather image meta data. 
1. Make a table that includes the following meta data for each image:
	- image name
	- image dimensions
	- image size (expressed via number of pixels)
	- image aspect ratio (expressed as a single floating point number)
	- pet name
	- owner initials
2. Sort the table largest to smallest by image size, breaking ties by alphabetical pet names (A - Z).
	- if using a notebook: print this table
	- if using a script: save this table to a file

### Task 2: Look at the meta data to assess differences in the dataset.
*For the following, label all plot axes (including units) and give all plots a descriptive title. If using a notebook, display all plots; if using a script, save all plots to files.*

1. Visualize the relationship between image size and aspect ratio by making a scatterplot of these two features across all images.
2. Pick the image with the smallest size. Make histograms of the Red, Green, and Blue color band intensities for this image.

### Task 3: Look at the image data to check quality.
*For the following: if using a notebook, display the figure; if using a script, save the figure to a file.*

1. Make a visualization of all images in the dataset.
	- All images should be displayed in subplots within a single figure. The subplot grid should have 4 columns. 
	- Images should be sorted alphabetically by the owner's initials (A - Z), starting in the top left corner of the grid.
		- again, break ties by pet names, also sorted alphabetically (A - Z).
	- Use the pet name as the title of each image in the grid.
