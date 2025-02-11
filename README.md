
# **🖥️ AWK Command Guide 📜** #

AWK is a powerful text-processing tool used for pattern scanning and data manipulation. It is widely used for analyzing structured text, extracting information, and automating reports.

## **📌 What is AWK?** ##

AWK is a programming language designed for text processing and is used mainly in Unix/Linux environments. It allows users to:

✔️ Search and filter text 📑

✔️ Process and manipulate structured data 📊

✔️ Generate reports automatically 📜

## **🚀 Getting Started with AWK
AWK processes text line by line and operates on fields within each line. The default delimiter is whitespace, but you can specify custom delimiters.

awk 'pattern { action }' file.txt
👉 pattern: Defines when the action should execute.
👉 action: Specifies what AWK should do with the matched text.

## 🔥 Common AWK Examples ##

**📌 Print Specific Columns **

        awk '{print $1, $3}' file.txt
        
📝 Prints the first and third columns of each line in file.txt.


📌 Filter Data Based on a Condition

        awk '$3 > 50 {print $1, $2}' data.csv
        
🔍 Prints the first and second columns only if the third column is greater than 50.

📌 Use a Custom Delimiter (CSV Processing)
bash
Copy
Edit
awk -F "," '{print $1, $2}' data.csv
📌 Sets comma (,) as the field separator and prints the first two columns of a CSV file.

🎯 Why Use AWK?
✅ Lightweight and built-in on most Linux/Unix systems
✅ Powerful for data extraction and formatting
✅ Ideal for log file analysis, reports, and data transformation

📚 Advanced AWK Features
🔥 Using Variables:

bash
Copy
Edit
awk '{ sum += $3 } END { print "Total:", sum }' data.txt
✔️ Computes the sum of the third column in data.txt.

🔥 Using Regular Expressions:

bash
Copy
Edit
awk '/error/ {print $0}' logfile.txt
✔️ Prints lines containing the word "error" in a log file.

🔥 Formatted Output:

bash
Copy
Edit
awk '{printf "User: %s, Age: %d\n", $1, $2}' users.txt
✔️ Formats output in a structured way.

🌟 Conclusion
AWK is an essential tool for text processing, data manipulation, and automation. It’s widely used by system administrators, data analysts, and developers.

📌 Master AWK and unlock the full potential of your command-line workflows! 🚀



