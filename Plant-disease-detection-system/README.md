---

# Plant Disease Detection System

This project is an end-to-end **plant disease detection platform** that integrates a **Next.js frontend**, **backend services (Flask + Node.js)**, and **machine learning models** (Python/JS). It enables users to upload plant images, run them through trained deep learning models, and receive disease predictions in real time.

---

## Project Overview

* **Frontend (Next.js)**: User interface for uploading plant images and displaying predictions.
* **Backend (Flask & Node.js)**: Handles requests, manages ML model execution, and provides APIs for predictions.
* **Machine Learning Models**: Python- and JS-based integrations for plant disease classification.
* **Database**: Configurable SQL database for logging predictions and user activity.

---

## Repository Structure

```
├── app/                        # Core Next.js application
├── components/                 # Reusable UI components
├── lib/                        # Utility functions
├── models/                     # ML models and related code
├── public/                     # Static assets
├── scripts/                    # Setup and helper scripts
├── styles/                     # Global and module CSS/SCSS
│
├── .env.local                  # Local environment variables
├── .gitattributes              # Git attributes
├── .gitignore                  # Ignored files and directories
│
├── DATABASE_SETUP_GUIDE.md     # Database configuration instructions
├── TROUBLESHOOTING.md          # Common issues and solutions
│
├── components.json             # UI component configuration
├── middleware.ts               # Next.js middleware
├── model_integration.py        # Python ML model integration
├── model_integration_code.js   # JS ML model integration
├── next.config.mjs             # Next.js config
├── package.json                # Node.js dependencies
├── package-lock.json           # Dependency lockfile
├── postcss.config.mjs          # PostCSS config
├── requirements.txt            # Python dependencies
├── setup-database.sql          # Database schema setup
├── test-database.js            # Database tests
├── test-env.js                 # Environment validation
├── tsconfig.json               # TypeScript config
└── README.md                   # Project documentation
```

---

## Installation & Setup

### Prerequisites

* **Node.js** (>= 18)
* **Python** (>= 3.9)
* **MySQL or PostgreSQL** database
* **npm / yarn / pip** package managers

### 1. Clone the Repository

```bash
git clone https://github.com/ayelefransi/Plant-disease-detection-system.git
cd Plant-disease-detection-system
```

### 2. Install Dependencies

**Frontend (Next.js)**

```bash
npm install
```

**Backend (Python/Flask)**

```bash
pip install -r requirements.txt
```

### 3. Environment Configuration

Create a `.env.local` file in the root directory and set required environment variables:

```bash
DATABASE_URL=your_database_connection_string
API_KEY=your_api_key
```

### 4. Database Setup

Run the provided SQL script:

```bash
mysql -u username -p < setup-database.sql
```

Or follow detailed steps in **DATABASE_SETUP_GUIDE.md**.

---

## Running the Project

### Start Next.js (Frontend)

```bash
npm run dev
```

Default: `http://localhost:3000`

### Start Backend (Python)

```bash
python model_integration.py
```

### Start Backend (Node.js)

```bash
node model_integration_code.js
```

---

## Testing

Run database tests:

```bash
node test-database.js
```

Run environment checks:

```bash
node test-env.js
```

---

## Troubleshooting

See **TROUBLESHOOTING.md** for solutions to common setup and runtime issues.

---

## Future Enhancements

* Mobile app integration with TensorFlow Lite.
* Expanded dataset for additional plant species.
* Automated deployment using Docker & CI/CD pipelines.

---

## License

This project is licensed under the MIT License.

---

## Author

**Fransi Ayele**
AI & ML Engineer | Deep Learning & Computer Vision
GitHub: [ayelefransi](https://github.com/ayelefransi)

---
