# **Manufacturing Downtime Analysis**

## **Overview**

This project analyzes **downtime factors** and **operator performance** for a soda bottling production line. The analysis identifies:

1. **Line efficiency**.  
2. **Underperforming operators**.  
3. **Leading factors contributing to downtime**.  
4. **Specific operator errors causing delays**.  

The results can be used to improve overall production efficiency.

---

## **Data Sources**

The analysis is based on the following datasets:

1. **Line Productivity**: Contains batch details, products, operators, start times, and end times.  
2. **Products**: Contains information about different types of products produced at the factory.  
3. **Line Downtime**: Records downtime minutes for each batch caused by various downtime factors.  
4. **Downtime Factors**: Provides descriptions for downtime codes and indicates whether they are operator errors.

---

## **Steps of Analysis**

### **1. Line Efficiency**
- **Calculation**:  
  **Efficiency** = Total Minimum Time / Total Actual Time
- The total actual time was derived from batch durations, and the total minimum time was taken from product requirements.

---

### **2. Underperforming Operators**
- Grouped productivity data by operators to calculate the **total time spent on batches**.  
- Compared performance against the **average line efficiency** to identify underperforming operators.

---

### **3. Leading Downtime Factors**
- Summed downtime minutes across all batches for each **downtime factor**.  
- Identified the **top contributing factors** to downtime.

---

### **4. Operator Errors**
- Filtered the **downtime data** for factors marked as **"Operator Error"**.  
- Merged the filtered data with the **Line Productivity** dataset to associate downtime factors with specific operators.  
- Grouped the results by **operators** and **error types** to analyze patterns of inefficiency.

---

## **Results**

### **1. Current Line Efficiency**
- The current line efficiency is **63.62%**.

---

### **2. Underperforming Operator**
- **Mac** appears to be underperforming with an efficiency of **58.33%**, compared to the average line efficiency.

---

### **3. Top 5 Leading Downtime Factors**
| **Downtime Factor**       | **Total Hours Wasted** |
|---------------------------|------------------------|
| Machine adjustment        | 332.0                 |
| Machine failure           | 254.0                 |
| Inventory shortage        | 225.0                 |
| Batch change              | 160.0                 |
| Batch coding error        | 145.0                 |

---

### **4. Top 5 Operators with Specific Downtime Factors**
| **Operator**   | **Downtime Factor**      | **Downtime (mins)** |
|----------------|--------------------------|---------------------|
| **Mac**        | Batch change             | 130.0               |
| **Dennis**     | Machine adjustment       | 120.0               |
| **Charlie**    | Machine adjustment       | 118.0               |
| **Dee**        | Machine adjustment       | 79.0                |
| **Charlie**    | Batch coding error       | 44.0                |

---

## **Conclusion**

The analysis provides actionable insights into:
1. **Downtime factors** that significantly impact productivity (e.g., Machine adjustment, Machine failure).  
2. **Operator performance**, with particular focus on underperformers like **Mac**.  
3. Areas for improvement by addressing operator errors and top downtime causes.

By addressing these areas, the soda bottling production line can reduce delays and improve overall efficiency.

