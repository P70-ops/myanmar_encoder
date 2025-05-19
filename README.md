# myanmar_encoder
Myanmar Name Encoding System (Professional Edition)


# Key Improvements

## ✅ Professional Architecture
- Object-oriented design with proper encapsulation  
- Comprehensive error handling  
- Configurable output formats  

## 📊 Enhanced Data Management
- Rich syllable database with metadata (frequency, category, alternatives)  
- Usage statistics tracking  
- Complete encoding history with timestamps  

## 🚀 Advanced Features
- Input validation with Myanmar-specific rules  
- Multiple output formats (short, long, academic, initials)  
- Statistical analysis of encoding results  
- Data export capabilities (JSON, Pandas DataFrame)  

## 🖥️ Improved User Interface
- Interactive menu system  
- Detailed output with warnings and statistics  
- History viewing and export  

## 📈 Analytical Capabilities
- Compression ratio calculation  
- Syllable frequency tracking  
- Performance metrics  

## 🧩 Extensibility
- Easy to add new syllable mappings  
- Support for external resource loading  
- Modular design for future enhancements  


### **1. Installation**
First, ensure you have Python installed (version 3.6 or later). Then, install the required dependency (Pandas for data analysis):

```bash
pip install pandas
```

---

### **2. Running the Encoder**
Copy the full code into a Python file (e.g., `myanmar_encoder.py`) and run it:

```bash
python myanmar_encoder.py
```

---

### **3. Interactive Menu Options**
When you run the program, you'll see a menu with these options:

```
============================================================
Myanmar Name Encoding System (Professional Edition)
============================================================

Options:
1. Encode a name
2. View statistics
3. Export history
4. Exit
```

---

### **4. How to Encode a Name**
1. **Select Option 1** (Encode a name).
2. **Enter a Myanmar name** (e.g., `မောင်ကျော်ထွန်း`).
3. **Choose an output format**:
   - `short` (e.g., `MgKyawT`)  
   - `long` (e.g., `MaungKyawHtun`)  
   - `academic` (similar to long)  
   - `initial` (e.g., `MKT`)  

**Example Output:**
```
Original: မောင်ကျော်ထွန်း
Encoded (short): MgKyawT

Statistics:
  Syllables: 3
  Mapped: 3
  Compression: 42.9%
```

---

### **5. Viewing Statistics (Option 2)**
- Shows system usage data:
  - Total encodings processed
  - Most frequently used syllables
  - Top 5 mapped syllables

**Example Output:**
```
System Statistics:
Total encodings: 5
Most used syllable: မောင် (3 uses)
Top 5 syllables:
  1. မောင် (3 uses)
  2. ကျော် (2 uses)
  3. ထွန်း (2 uses)
```

---

### **6. Exporting History (Option 3)**
- Saves all past encodings to `encoding_history.json`.
- Displays the last 3 encodings in a table format.

**Example Output:**
```
History saved to encoding_history.json

Recent encodings:
timestamp                     original          encoded    format  stats
2024-05-20T12:30:45.123 မောင်ကျော်ထွန်း    MgKyawT    short   {...}
2024-05-20T12:31:10.456 အောင်ဇော်            AZ         short   {...}
```

---

### **7. Exiting (Option 4)**
- Type `4` to quit the program.

---

### **Advanced Usage**
- **Custom Syllable Mappings**:  
  Modify the `syllable_map` dictionary in `_initialize_syllable_database()` to add new mappings.
  
- **Data Analysis**:  
  Use `encoder.generate_dataframe()` to analyze encoding trends with Pandas.

- **Error Handling**:  
  Invalid inputs (e.g., non-Myanmar characters) will trigger warnings.

---

### **Example Workflow**
1. Run the program.
2. Select `1` and enter `ကျော်စန်းဝင်း`.
3. Choose `short` format → Output: `KyawSW`.
4. Check statistics (Option 2) to see usage trends.
5. Export history (Option 3) for records.
6. Exit (Option 4).

