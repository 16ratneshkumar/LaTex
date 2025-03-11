# **Tables in LaTeX: Formatting and Usage**
> *🚀📊 Tables in LaTeX: Where rows align, columns shine, and data dines in style! ✨🔥*  

## **Introduction**  
The `tabular` environment in LaTeX is used to **typeset tables**. By default, LaTeX does not draw **horizontal** or **vertical** lines; you must specify them explicitly. LaTeX automatically determines the width of the columns unless otherwise specified.  

## **Basic Syntax**  
A LaTeX table begins with the following command:  
```latex
\begin{tabular}{...}
```
Where the `{...}` inside the curly brackets defines the table's **column structure**. The table is closed using:  
```latex
\end{tabular}
```

---

## **Column Definitions**  
Inside the `{...}`, different symbols define the alignment and formatting of table columns:  

| **Symbol** | **Meaning** |
|-----------|------------|
| `l`  | Left-aligned column (`l` for **left**) |
| `r`  | Right-aligned column (`r` for **right**) |
| `c`  | Center-aligned column (`c` for **center**) |
| `|`  | Adds a **vertical line** between columns |

---

## **Table Row and Column Separators**  
- **Column Separator (`&`)** → Used to separate columns in a row.  
- **New Row (`\\`)** → Placed at the **end of a row** to move to the next row.  

### **Example Table Without Borders**  
```latex
\begin{tabular}{l c r}
Apple & Banana & Cherry \\  
Dog & Elephant & Fox \\  
Guitar & Harmonica & Violin \\  
\end{tabular}
```

🔹 **Output:**  
![Output](<Output/Table 1.png>)

---

## **Adding Lines in Tables**  
To enhance readability, **horizontal** and **partial lines** can be added:  

### **1. Full Horizontal Line (`\hline`)**  
- Draws a **full-width** line across the table.  

### **2. Partial Horizontal Line (`\cline{X-Y}`)**  
- Draws a horizontal line **only from column `X` to column `Y`**.  

### **Example Table with Lines**  
```latex
\begin{tabular}{|l|c|r|}
\hline
Apple  & Banana    & Cherry  \\  
\hline
Dog    & Elephant  & Fox     \\  
\cline{2-3}
Guitar & Harmonica & Violin  \\  
\hline
\end{tabular}
```

🔹 **Output:**  
![Output](<Output/Table 2.png>)

---

## **Conclusion**  
The `tabular` environment is a **powerful tool** for creating well-structured tables in LaTeX. By combining **column alignments**, **lines**, and **row separators**, you can format tables as per your needs.  


[← Previous Page](<List,Comments & Spacing, Special Characters.md>) | **7** | [Next Page →](<Mathematical Expression.md>)
