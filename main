import os
import shutil

# Source and destination folders
download_folder = r"C:\Users\RAZER\Downloads"
destination_folder = r"C:\Users\RAZER\Downloads\images test"

# Get a list of all files in the download folder
files = os.listdir(download_folder)

# Filter out only image files (you can adjust this condition as needed)
image_files = [file for file in files if file.lower().endswith(('.png', '.jpg', '.jpeg', '.gif'))]

# Move each image file to the destination folder
for image_file in image_files:
    source_path = os.path.join(download_folder, image_file)
    destination_path = os.path.join(destination_folder, image_file)
    
    try:
        shutil.move(source_path, destination_path)
        print(f"Moved: {image_file}")
    except Exception as e:
        print(f"Error moving {image_file}: {e}")
