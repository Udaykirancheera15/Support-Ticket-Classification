# Dataset Availability

## Inability to Provide All Datasets Due to Large Size

Due to the large size of the datasets used in this project, we are unable to provide the full datasets for direct download. The datasets are extensive and may not be feasible to host directly on this repository. However, we will outline the data sources and alternative options for obtaining the data.

## Data Source
The datasets used in this project were inspired by real-world support ticket classification data. Specifically, the data is simulated from Stack Overflow posts across various topics, such as:
- **3D Printing**
- **Android**
- **Apple**
- **Database Administration (DBA)**
- **Unix**

These datasets contain various attributes such as post titles, body content, tags, ticket types, and other metadata.

## Alternative Options for Accessing Data
If you need the complete datasets for your own use or to replicate this project, we recommend the following alternatives:

1. **Stack Overflow Dataset**  
   You can access a similar dataset directly from the [Stack Overflow Data Dump](https://archive.org/details/stackexchange).

2. **Custom Dataset Generation**  
   You can generate your own dataset using similar attributes from Stack Overflow or other platforms like GitHub, where issues can be treated as tickets. This can help you create a similar dataset for text mining and classification tasks.

3. **Smaller Sample Data**  
   For development and testing purposes, a smaller sample dataset (`AllTicketsSample`) is included in this repository. This is a subset of the full dataset and is suitable for experimentation and model development.

## Notes on Dataset Size
- The full dataset is large and contains millions of posts, which could be difficult to handle for local environments with limited resources.
- The dataset is stored in a PostgreSQL database in the production setup, and the system is designed to handle it in a distributed environment (AI Hub).

If you have specific requests for data or need guidance on how to generate or access datasets, feel free to open an issue in this repository or contact the project maintainers.

## Conclusion
We apologize for the inconvenience and appreciate your understanding. Please refer to the above-mentioned data sources to replicate or extend the datasets for your own use.

