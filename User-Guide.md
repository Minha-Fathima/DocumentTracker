# 📖 User Guide for Data Analytics of a Document Tracker

## 1. Getting Started
Navigate to the executable folder and run the `CW2.exe` executable file to launch the application.

Once the application is launched, you will be able to view the interface as shown in figure 1.

<img width="395" alt="image" src="https://github.com/user-attachments/assets/23f1fef6-3e62-4faf-84b5-92ef17a4ade9" />



---

## 2. Loading Data
To begin your data analysis process, you can load your JSON data using the **"Load File"** button as shown in figure 2.

The button will open a file dialog menu allowing you to navigate and upload your desired JSON data file.

<img width="468" alt="image" src="https://github.com/user-attachments/assets/b6f75dd7-5ca1-4222-8f7e-fbada1c50b7e" />

---

## 3. Data Analysis Tasks
To view the available data analysis processes, you can click on the **"Analysis Task"** dropdown menu as shown in figure 3.

Based on the selected task, you will be asked to provide the **Document UUID** and (optionally) **Visitor UUID**, as shown in Figure 4.

If no new fields open up, then no UUIDs are required.

<img width="468" alt="image" src="https://github.com/user-attachments/assets/1bc3fe07-1529-42d3-9768-5fb602d2e857" />

<img width="468" alt="image" src="https://github.com/user-attachments/assets/8c7f931f-9b9a-4d5c-8519-99aa980e048c" />



---

## 4. Interactive Visualizations
Once you have selected your desired data analysis task, click on the **"Analyze"** button as shown in Figure 5.

The visualizations will be displayed in the **Visualization Area**, as shown in Figure 5.

You can hover over the visualizations to get more detailed information.

<img width="395" alt="image" src="https://github.com/user-attachments/assets/65bd9f00-cd76-438c-bad2-b36c300fd046" />



---

## 5. Generating Graphs
To generate the graph for **"Also Likes"**, provide the required UUIDs and click on **"Analyze"**. Once the graph has been generated, a PDF of the graph will automatically launch in your default PDF viewer.

If the PDF does not launch, you can alternatively find the PDF in the same folder as the `CW2.exe` executable file.

<img width="395" alt="image" src="https://github.com/user-attachments/assets/bb603f7e-e4a8-4f5f-8524-47e1f9bd9f79" />


---

## 6. Viewing the Admin Dashboard
To view the Admin Dashboard, click on the **"View Admin Dashboard"** button on the top left corner of the application, as shown in Figure 7.

<img width="468" alt="image" src="https://github.com/user-attachments/assets/c62cd1d9-0d4b-47e5-b058-30f3dce59672" />

---

## 7. Navigating the Admin Dashboard
To view insights in the Admin Dashboard:

1. Load a JSON data file by clicking on the **"Load Data"** button in the navigation panel (Figure 8).
2. Once data is loaded, navigate to different insights using the navigation panel.

<img width="395" alt="image" src="https://github.com/user-attachments/assets/7c0fc8a8-93cb-4b7b-8d53-f9f96e44c38c" />


---

## 8. Viewing Visualizations in the Admin Dashboard
- Click on the **"Overview"** button in the navigation panel to see a general overview of the loaded data (Figure 9).
- Use the **"Next"** and **"Previous"** buttons at the bottom of the visualizations to browse through the visualizations (Figure 10).
- Click on the **"Table"** button in the navigation panel to view a sorted table of all documents, showing the number of readers and the average time spent reading each document. The table is scrollable for large datasets (Figure 11).

<img width="395" alt="image" src="https://github.com/user-attachments/assets/31e108ca-064a-40d6-a767-bac5704ada2d" />
<img width="395" alt="image" src="https://github.com/user-attachments/assets/0985fa2d-c8b9-4c77-ae79-18f4c46ebe5a" />
<img width="395" alt="image" src="https://github.com/user-attachments/assets/1036e40e-c06b-47ba-b0d4-abf9a07cd91d" />


---

## 9. Command-Line Interface Usage
You can run all the data analysis tasks using the command-line interface (CLI).

1. Navigate to the directory containing the executable file (`cw2`) using a terminal or command prompt.
2. Run the script using the following command format:

   ```bash
   ./cw2 -u user_uuid -d doc_uuid -t task_id -f file_name
   ```

### Command-Line Arguments
| Argument          | Description                                         | Example           |
|-------------------|-----------------------------------------------------|-------------------|
| `-t` or `--task_id` | Specifies the task to perform. Options: 2a, 2b, 3a, 3b, 4, 5d, 6, 7. | `-t 2a`          |
| `-d` or `--doc_uuid` | The Document UUID to analyze. Required for certain tasks like 2a, 2b, 5d, and 6. | `-d 12345`       |
| `-u` or `--visitor_uuid` | The Visitor UUID (optional for task 6).           | `-u 67890`       |
| `-f` or `--file_name` | The JSON file containing the data for analysis.    | `-f data/sample.json` |

---

### Additional Notes
- Ensure the JSON file format is correct and contains the necessary fields for analysis.
- Follow the error messages and guidance provided by the application for troubleshooting.

---

For further assistance, please refer to the repository's [README.md](./README.md) or contact the project maintainers.
