# Mall Customer Segmentation – K-Means Clustering  

This project applies **K-Means Clustering** to segment mall customers based on **Annual Income** and **Spending Score**.  
The goal is to understand customer groups for better marketing and business strategies.  

---

## Dataset Features  

| Feature | Description |
|---------|-------------|
| `CustomerID` | Unique ID for each customer |
| `Gender` | Male/Female |
| `Age` | Age of the customer |
| `Annual Income (k$)` | Annual income in thousands of dollars |
| `Spending Score (1-100)` | Mall-assigned score based on purchase behavior |

---

## Steps Performed  

1. **Load and explore** the dataset  
2. **Fit K-Means** and assign cluster labels  
3. **Find optimal K** using the Elbow Method  
4. **Visualize clusters** with business interpretation  
5. **Evaluate** using Silhouette Score  

---

## Elbow Method – Finding Optimal K  

The **Elbow Method** identifies the best K by looking for the point where adding more clusters doesn’t reduce inertia significantly.  

<img width="571" height="455" alt="image" src="https://github.com/user-attachments/assets/1a954848-0e27-4569-b13a-77e1db2c4b30" />


From the plot, **K = 5** was chosen.  

---

## Cluster Descriptions  

| Cluster Name | Business Meaning |
|--------------|------------------|
| **Cluster 0 – Average Spenders**  | Moderate income and spending |
| **Cluster 1 – High Income, High Spending**  | Premium loyal customers |
| **Cluster 2 – Low Income, High Spending**  | Impulsive shoppers |
| **Cluster 3 – Low Income, Low Spending**  | Budget-conscious customers |
| **Cluster 4 – High Income, Low Spending**  | Wealthy but cautious spenders |

---

## Final Visualization  

<img width="1020" height="470" alt="image" src="https://github.com/user-attachments/assets/beb38555-942e-43b6-9d2a-3f252043f596" />


- **X-axis:** Annual Income (k$)  
- **Y-axis:** Spending Score (1–100)  
- **Colors:** Represent distinct customer segments with business meaning  

---

## Model Evaluation  

- **Silhouette Score:** `0.408` → Moderate separation between clusters  
- Some clusters (e.g., high spenders vs low spenders) are well separated,  
  while others (middle income/spending) slightly overlap.

---

## Business Insights  

- **High spenders**: Target with loyalty programs & premium offers  
- **High income, low spenders**: Personalized marketing to increase spending  
- **Low income, high spenders**: Offer discounts & seasonal deals  
- **Average customers**: Encourage more spending with promotions  
- **Budget-conscious**: Low marketing priority  

---


