# Python Parquet Files Tutorial: Complete Guide with Examples

A comprehensive collection of Jupyter notebooks teaching everything you need to know about working with Apache Parquet files in Python using pandas and PyArrow.

## 📚 Tutorial Contents

### 1. [Complete Guide to Apache Parquet Files in Python](01_Parquet_Files_Python_Tutorial_Complete_Guide.ipynb)
Learn the fundamentals of Parquet files and why they're essential for modern data engineering.

**Topics covered:**
- What is Apache Parquet and its benefits
- Parquet vs CSV performance comparison
- Installing required libraries (pandas, pyarrow)
- Understanding Parquet file structure
- Data type preservation
- Compression basics

**Keywords:** parquet files python, apache parquet tutorial, parquet vs csv, python data formats

---

### 2. [How to Read and Write Parquet Files in Python](02_Read_Write_Parquet_Files_Python_Pandas_PyArrow.ipynb)
Master reading and writing Parquet files with various options and optimizations.

**Topics covered:**
- Writing Parquet files with pandas and PyArrow
- Reading Parquet files efficiently
- Column selection and filtering
- Compression methods comparison
- Working with partitioned datasets
- Cloud storage integration (S3, Azure, GCS)

**Keywords:** read parquet python, write parquet pandas, pyarrow parquet, parquet compression

---

### 3. [Advanced Parquet Operations in Python](03_Advanced_Parquet_Operations_Python_Tutorial.ipynb)
Dive deep into advanced features and performance optimizations.

**Topics covered:**
- Schema management and evolution
- Working with metadata
- Advanced filtering with PyArrow
- Memory-efficient batch processing
- Integration with Dask
- Data validation and quality checks

**Keywords:** parquet schema evolution, pyarrow filtering, parquet metadata, batch processing parquet

---

## 🚀 Getting Started

### Prerequisites

```bash
pip install pandas pyarrow
```

Optional packages for advanced features:
```bash
pip install dask[complete]  # For distributed processing
pip install fastparquet     # Alternative Parquet engine
```

### Quick Example

```python
import pandas as pd

# Write a Parquet file
df = pd.DataFrame({'name': ['Alice', 'Bob'], 'age': [25, 30]})
df.to_parquet('example.parquet')

# Read a Parquet file
df_read = pd.read_parquet('example.parquet')
print(df_read)
```

## 💡 Why Use Parquet Files?

1. **Storage Efficiency**: 70-90% smaller than CSV files
2. **Performance**: 5-10x faster read operations
3. **Type Safety**: Preserves data types without parsing
4. **Big Data Ready**: Works with Spark, Dask, and other frameworks
5. **Cloud Optimized**: Efficient with S3, Azure Blob, and GCS

## 🛠️ Common Use Cases

- **Data Warehousing**: Efficient storage for analytical queries
- **ETL Pipelines**: Fast data transformation workflows
- **Machine Learning**: Quick access to training datasets
- **Data Archival**: Long-term storage with compression
- **Real-time Analytics**: Partitioned datasets for time-series data

## 📊 Performance Comparison

| Format | File Size | Read Speed | Type Preservation | Compression |
|--------|-----------|------------|-------------------|-------------|
| CSV    | 100 MB    | 1.0x       | ❌                | ❌          |
| Parquet| 15 MB     | 5-10x      | ✅                | ✅          |

## 🔗 Additional Resources

- [Apache Parquet Documentation](https://parquet.apache.org/)
- [PyArrow Documentation](https://arrow.apache.org/docs/python/)
- [Pandas Parquet Guide](https://pandas.pydata.org/docs/user_guide/io.html#parquet)

## 📝 Contributing

Feel free to submit issues, fork the repository, and create pull requests for any improvements.

## 📄 License

This tutorial collection is available under the MIT License.

---

**Author**: Lorenzo De Tomasi
**Last Updated**: 2025   
**Python Version**: 3.8+
