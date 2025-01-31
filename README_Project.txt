
# Entry-Level Luxury Cars Analysis Project

## **Overview**
This project analyzes consumer discussions on entry-level luxury cars, scraped from Edmunds.com forums, to uncover insights about brand mentions, attribute associations, co-occurrence lift values, and consumer aspirations. The analysis was performed using Python and various libraries for text processing, data analysis, and visualization.

---

## **Dataset**
- **Source**: The data for this project was scraped from the [Edmunds Forums: Entry-Level Luxury Performance Sedans](https://forums.edmunds.com/discussion/2864/general/x/entry-level-luxury-performance-sedans).
- **Files Included**:
  - `check_data.csv`: Contains the scraped posts.
  - `Word_Frequency.csv`: Word frequency analysis output.
  - `brand_pair.csv`: Brand co-occurrence pairs.
  - `attributes_pair.csv`: Brand-attribute pairs.
  - `aspiration_pair.csv`: Brand-aspiration pairs.

---

## **Project Files**
- **Python Notebook**: A Jupyter Notebook file (`Project.ipynb`) containing the code for analysis.
- **Outputs**:
  - MDS plots and heatmaps for visualization.
  - CSV files with processed data and calculated lift values.
- **Documentation**:
  - Detailed project explanation and insights (provided in this README and accompanying files).

---

## **Environment Setup**

### **1. Install Required Libraries**
Run the following command to install the required Python packages:
```bash
pip install pandas numpy matplotlib seaborn nltk scikit-learn
```

### **2. File Structure**
Ensure the following folder structure:

```
project-folder/
    |-- Input Files/
        |-- check_data.csv
        |-- Word_Frequency_Rank.csv
        |-- car_models_and_brands.csv
    |-- Output Files/
        |-- Word_Frequency.csv
        |-- brand_pair.csv
        |-- attributes_pair.csv
        |-- aspiration_pair.csv
        |-- Top_Brands_Lift_Values.csv
        |-- Top_Brands_Lift_Matrix.csv
        |-- Attributes_Lift_Matrix.csv
        |-- Aspiration_Lift_Matrix.csv
    |-- Project.ipynb
    |-- README.md
```

### **3. Downloading and Running the Project**
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/entry-level-luxury-cars-analysis.git
   ```
2. Navigate to the project directory:
   ```bash
   cd entry-level-luxury-cars-analysis
   ```
3. Open the Jupyter Notebook:
   ```bash
   jupyter notebook Project.ipynb
   ```
4. Run the notebook cells sequentially to reproduce the analysis and visualizations.

---

## **Methodology**
1. **Scraping Data**:
   - Data was scraped from [Edmunds.com](https://www.edmunds.com/) forums, focusing on discussions about entry-level luxury cars.
2. **Data Preprocessing**:
   - Removed punctuation, converted text to lowercase, and tokenized the posts.
   - Replaced car model names with their respective brands.
3. **Analysis Steps**:
   - Word frequency analysis to identify popular brands and attributes.
   - Lift value calculation for brand and attribute co-occurrence.
   - Multi-Dimensional Scaling (MDS) for brand visualization.

---

## **Results and Insights**
- **MDS and Lift Analysis**:
  - Acura and Subaru had unexpected high co-mentions, likely due to overlapping discussions.
  - Volkswagen and Audi showed strong co-mentions, reflecting their shared parentage.
  - Infiniti was positioned between Acura and Audi, highlighting its upper-middle-class appeal.
- **Brand-Attribute Analysis**:
  - Honda and Subaru outperformed luxury brands like BMW in tech-related discussions.
  - BMW's performance-related mentions were lower than expected, indicating a gap in consumer perception.
- **Aspirational Mentions**:
  - Discussions were not heavily aspirational, though Hyundai showed notable co-mentions with aspiration-related terms.

---

## **Dependencies**
- **Python Version**: 3.8+
- **Libraries Used**:
  - `pandas`: Data manipulation and analysis.
  - `numpy`: Numerical computations.
  - `matplotlib` and `seaborn`: Data visualization.
  - `nltk`: Natural language processing.
  - `scikit-learn`: MDS plot generation.

---

## **How to Use the Project**
1. Place the required input files in the `Input Files/` folder.
2. Run the notebook to reproduce the analysis, which includes:
   - Generating word frequencies.
   - Calculating and visualizing lift values.
   - Producing MDS plots and heatmaps for insights.
3. Use the output CSV files and visualizations for further analysis or reporting.

---

## **Contact**
If you encounter any issues or have questions, feel free to open an issue or contact me at [prrohilla@utexas.edu].
