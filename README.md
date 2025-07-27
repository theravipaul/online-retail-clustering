# 🧠 Customer Segmentation Using K-Means Clustering

This project performs customer segmentation on an online retail dataset using RFM (Recency, Frequency, Monetary) analysis and K-Means clustering. It helps businesses identify different customer groups for targeted marketing and retention strategies.

---

## 📂 Dataset

- **Source**: `online_retail_2.xlsx`
- **Features Used**:
  - `InvoiceDate` → for **Recency**
  - `Invoice` → for **Frequency**
  - `Quantity x Price` → for **Monetary Value**

---

## ⚙️ Features & Flow

### ✅ Step-by-step:
1. **Data Cleaning**  
   - Remove cancelled orders, null values, and invalid stock codes

2. **Feature Engineering**  
   - Create `TotalPrice` and compute RFM values

3. **Outlier Removal**  
   - Exclude top 5% of extreme values for RFM features

4. **Standardization**  
   - Scale data using `StandardScaler` for clustering

5. **Elbow & Silhouette Method**  
   - Determine optimal number of clusters (`k`)

6. **K-Means Clustering**  
   - Cluster customers into meaningful segments

7. **Cluster Visualization**  
   - Use `violinplot` to show RFM distribution across clusters

8. **Business Interpretation**  
   - Label clusters (e.g., "Loyal Spenders", "Lost Customers")
   - Suggest retention or marketing strategies

---

## 📈 Technologies Used

- `pandas` for data manipulation  
- `numpy` for numerical operations  
- `matplotlib` & `seaborn` for visualizations  
- `scikit-learn` for clustering and preprocessing

---

## 📊 Example Output

- Cluster 3 → Loyal High Spenders  
- Cluster 0 → Regular Buyers  
- Cluster 2 → Mid-Tier Customers  
- Cluster 1 → Lost/One-Time Customers

---

## 📁 Files

- `online_retail_clustering.ipynb` → Full code notebook
- `requirements.txt` → Install dependencies
- `README.md` → Project documentation

---

## 🚀 How to Run

```bash
# Install dependencies
pip install -r requirements.txt

# Launch Jupyter
jupyter notebook
