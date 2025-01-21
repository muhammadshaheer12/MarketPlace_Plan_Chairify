# MarketPlace_Plan_Chairify

# Chairify Platform

Chairify is an e-commerce platform specializing in selling chairs. This README outlines the core functionalities, setup instructions, and technologies used in the development of Chairify, including its integration with Sanity CMS for backend management.

## Features

### Core Functionalities
- **Product Listings**: Browse a variety of chairs with details such as name, price, description, and images.
- **Filters and Search**: Refine product listings by category, material, or price range, and search for specific chairs.
- **Shopping Cart**: Add, update, or remove items from the cart.
- **Product Details Page**: View detailed information about each chair.
- **User Account Management**: Register, log in, and manage user profiles.
- **Checkout Process**: Secure payment gateway integration for smooth transactions.

### Additional Features
- **Sanity CMS Integration**: Manage products, categories, and content dynamically through the Sanity CMS backend.
- **Responsive Design**: Optimized for desktops, tablets, and mobile devices.
- **Error Handling**: Graceful handling of API errors and user input validation.
- **Performance Optimization**: Fast loading times with lazy loading, image compression, and minified assets.

## Technologies Used

- **Frontend**: React.js, Tailwind CSS
- **Backend**: Sanity CMS, Node.js, Express.js
- **Database**: Sanity CMS backend
- **Testing Tools**: Cypress, React Testing Library, Postman
- **Deployment**: Docker, Vercel

## Installation and Setup

### Prerequisites
- Node.js (v14 or later)
- Sanity CLI
- Docker (optional for containerized deployment)

### Steps to Run Locally
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/chairify.git
   cd chairify
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Set up Sanity CMS:
   - Install the Sanity CLI:
     ```bash
     npm install -g @sanity/cli
     ```
   - Navigate to the `backend` folder and initialize Sanity:
     ```bash
     cd backend
     sanity init
     ```
   - Connect to your Sanity project or create a new one.

4. Set up environment variables:
   Create a `.env` file in the root directory and add the following variables:
   ```env
   SANITY_PROJECT_ID=<your-sanity-project-id>
   SANITY_DATASET=<your-sanity-dataset>
   SANITY_API_TOKEN=<your-sanity-api-token>
   ```

5. Start the development server:
   ```bash
   npm start
   ```

6. Access the platform at `http://localhost:3000`.

### Running Tests
To execute tests, run:
```bash
npm test
```

## Folder Structure
```
chairify/
├── public/         # Static assets
├── src/
│   ├── components/ # Reusable UI components
│   ├── pages/      # Page components
│   ├── hooks/      # Custom React hooks
│   ├── utils/      # Utility functions
│   └── App.js      # Main application file
├── backend/        # Sanity CMS project files
├── .env            # Environment variables
├── package.json    # Project metadata
└── README.md       # Project documentation
```

## Deployment

### Docker Deployment
1. Build the Docker image:
   ```bash
   docker build -t chairify .
   ```

2. Run the container:
   ```bash
   docker run -p 3000:3000 chairify
   ```

### Vercel Deployment
1. Connect your GitHub repository to Vercel.
2. Set the environment variables in Vercel's settings.
3. Deploy the project directly from Vercel.

## Contributing

We welcome contributions! Please follow these steps:
1. Fork the repository.
2. Create a new branch for your feature:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add new feature"
   ```
4. Push to your branch:
   ```bash
   git push origin feature-name
   ```
5. Open a pull request.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Contact
For any questions or support, please contact us at support@chairify.com.
