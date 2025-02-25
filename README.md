# 👗 Fashion Sales Dashboard

An **interactive Power BI dashboard** to analyze and visualize fashion sales data across multiple channels. Gain insights into sales performance, customer preferences, and regional distribution.

## 📊 Dashboard Features

- **Total Sales & Average Order Value**
- **Order Status Breakdown (Delivered vs. Refunded)**
- **Sales by Channel (Myntra, Amazon, Flipkart, Nykaa)**
- **Top Categories & Best-Selling Sizes**
- **Geographic Sales Distribution (City & State-wise)**
- **B2B vs. B2C Sales Comparison**

## 📁 Dataset Overview

| Column Name         | Description                        |
|---------------------|------------------------------------|
| **Status**          | Delivery status (Delivered/Refunded) |
| **Channel**         | Sales channel (Myntra, Amazon, etc.) |
| **SKU**             | Stock Keeping Unit (Product ID)     |
| **Category**        | Fashion category (e.g., Kurta, Top) |
| **Size**            | Product size (e.g., XL, M, 3XL)     |
| **Qty**             | Quantity of items sold              |
| **Amount**          | Sale amount for each transaction    |
| **Ship-City**       | Customer's shipping city            |
| **Ship-State**      | Customer's shipping state           |
| **Ship-Postal-Code**| Postal code of the shipping address |
| **B2B**             | Whether the order is B2B (Yes/No)  |

## 📐 Key Metrics

1. **Total Sales**: Sum of all transaction amounts.  
2. **Average Order Value (AOV)**: Defined as:
   ```DAX
   AOV = DIVIDE(SUM('Orders'[Amount]), DISTINCTCOUNT('Orders'[Order ID]))
   ```
3. **Order Count by Status**: Visualization of Delivered vs. Refunded.

## 📊 Visuals Included

- **Bar Chart**: Sales by Channel
- **Pie Chart**: Order Status Distribution
- **Map Visualization**: Sales by State/City
- **Card Visual**: Total Sales & AOV
- **Stacked Column Chart**: Category-wise Performance

## 🚀 How to Run the Dashboard

1. Ensure **Power BI Desktop** is installed. [Download here](https://powerbi.microsoft.com/)
2. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/fashion-sales-dashboard.git
    ```

3. Open `fashion_sales_dashboard.pbix` in Power BI Desktop.
4. Explore interactive insights and export reports.

## 📌 Customization
- Modify the `AOV` calculation to a fixed value if required:

    ```DAX
    AOV = 753
    ```

- Add more visuals or adjust filters as needed.

## 📊 Sample Insights
- **Flipkart** leads in sales volume.
- **Kurta** is the top-performing category.
- High return rates for **larger sizes (3XL & 6XL)**.

## 🛠️ Tools Used
- **Power BI Desktop**: Data modeling & visualization
- **Excel/CSV**: Data source
- **DAX (Data Analysis Expressions)**: Custom measures

## 📞 Contact
For inquiries or collaboration, reach out via [your email/LinkedIn].

---

**⭐ Star this repo if you find it useful!**

