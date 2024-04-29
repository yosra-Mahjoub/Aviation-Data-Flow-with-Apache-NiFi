# Aviation Data Flow with Apache NiFi

> ## Overview

This project demonstrates the power of Apache NiFi in managing the data flow essential for efficient aviation operations. Data flow is the lifeblood of modern aviation, where timely and accurate information can make all the difference in ensuring safe and smooth operations. From flight schedules and weather conditions to passenger manifests and maintenance logs, aviation generates vast amounts of data that need to be collected, processed, and analyzed in real-time.

Apache NiFi serves as the backbone of this data flow, providing the infrastructure to seamlessly integrate, transform, and route data from diverse sources to various destinations. With its intuitive graphical interface and extensive library of processors, NiFi simplifies the creation of complex data pipelines, allowing aviation professionals to focus on insights and actions rather than the intricacies of data management.

For more details read [Why data flow is the fuel for aviation operations](https://www.linkedin.com/pulse/why-data-flow-fuel-aviation-operations-zivan-gvozdenovic-ssm/)


> ## Features

- **Data Collection**: Apache NiFi is configured to collect streaming data from the [AviationStack API](https://aviationstack.com/) using the *InvokeHTTP processor*. This allows for real-time retrieval of aviation data, including flight information, airline details, and more.

- **Data Processing**: The collected JSON data is split into individual records based on days using the *SplitJSON processor*. Additionally, *JoltTransformJSON processor* is employed to apply transformations to the JSON payload as per specified Jolt specifications. This ensures efficient handling and processing of the data flow.

- **Data Storage**: Processed data is stored in MongoDB for persistence. MongoDB offers flexibility and scalability, making it suitable for storing unstructured or semi-structured data like JSON documents. Furthermore, the JSON data is converted into SQL format for insertion into a MySQL table..


## Getting Started

To get started with this project:

1. Install Apache NiFi on your server or local machine.
2. Clone this repository.
3. Import the XML file included in this repository.
4. Add Template to Nifi Canvas.

