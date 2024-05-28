# Dusty

Dusty is a reference chat application designed specifically for soil scientists. It leverages the TinyLlama model to provide accurate and insightful responses to queries related to soil science. The application offers a REST API and an interactive Vaadin-based user interface for seamless interaction. Built using Spring Boot, Dusty can also be compiled as a native application using GraalVM for enhanced performance.

## Features

- **Soil Science Reference**: Get accurate answers and references for soil science-related queries.
- **Interactive Chat Interface**: Use the Vaadin-based UI for intuitive and user-friendly interactions.
- **REST API**: Access Dusty's features programmatically via the REST API.
- **Native Compilation**: Compile the application as a native image using GraalVM for better performance and reduced resource consumption.

## Getting Started

### Prerequisites

- Java 11 or higher
- Maven 3.6.0 or higher
- GraalVM (for native compilation)

### Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/your-username/dusty.git
   cd dusty
   ```

   2. **Build the application**

      ```bash
      mvn clean install
      ```

3. **Run the application**


   - *As a Spring Boot application*
      ```bash
      mvn spring-boot:run
      ``` 
   - *As a native application (GraalVM required)*
      ```bash
      mvn package -Pnative
      ./target/dusty
      ``` 

### Using the Application

#### REST API

Access Dusty's features programmatically through the REST API.

- **Endpoint**: `/api/v1/chat`
- **Methods**: `POST`

Example:

```bash
curl -X POST http://localhost:8080/api/v1/chat -H "Content-Type: application/json" -d '{
  "query": "What is the optimal pH for corn?"
}'
```

#### Vaadin Interface

Access the user interface by navigating to http://localhost:8080 in your web browser.

### Additional Features

- **Historical Query Analysis**: Track and analyze past queries to improve responses.
- **Personalized Recommendations**: Provide tailored advice based on user history and preferences.
- **Integration with External Databases**: Connect to external soil science databases for enriched information.
- **Custom Alerts**: Set up notifications for specific soil conditions or research updates.

## Contributing

I always welcome contributions to Dusty! If you have an idea for a new feature or have found a bug, please open an issue or submit a pull request.

1. Fork the repository
2. Create a new branch (`git checkout -b feature-branch`)
3. Make your changes
4. Commit your changes (`git commit -am 'Add new feature'`)
5. Push to the branch (`git push origin feature-branch`)
6. Create a new Pull Request

You can save the above content into a file named ADDITIONAL_FEATURES_AND_CONTRIBUTING.md.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

If you have any questions or need further assistance, please contact me at [codemountainlabs@gmail.com](mailto:codemountainlabs@gmail.com).

