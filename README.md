# Daniel Spears — Project Portfolio

A collection of full-stack applications, data visualization tools, and hardware projects demonstrating expertise in Go, Python, Next.js, and embedded systems.

🔗 **Live Portfolio:** [portfolio.danielspears.com](https://portfolio.danielspears.com)

---

## Web Applications

### AI Model Interaction Suite
**Tech Stack:** Next.js, OpenAI, Anthropic, Cohere, Google Gemini, Mistral AI, Pinecone, Prisma, Eleven Labs

A comprehensive platform for interacting with multiple Large Language Models. Designed as a monolithic "all-in-one" environment for rapid prototyping and discovering optimal AI interaction patterns.

**Features:**
- Multi-provider LLM support (OpenAI, Claude, Cohere, Gemini, Mistral)
- Document processing (PDF, DOCX, XLSX, CSV)
- Web content scraping and analysis
- Vector search with Pinecone for RAG workflows
- Text-to-speech via Eleven Labs
- Real-time chat interface

---

### AuthenticationRAG
**Tech Stack:** Next.js 15, Supabase Auth, OpenAI, Pinecone

A protected RAG (Retrieval-Augmented Generation) chatbot with role-based access control.

**Features:**
- Magic link authentication via Supabase
- User/admin role management with profiles table
- Admin console for user invites and bulk CSV seeding
- Protected RAG endpoint combining OpenAI embeddings with Pinecone vector search

---

### Go Poll
**Tech Stack:** Go, PostgreSQL, GORM, Firebase Authentication

A polling and survey web application with public voting and authenticated admin functionality.

**Features:**
- Public API for polls, voting, and aggregated reports
- Admin API for poll creation and data management
- Firebase-backed authentication with optional custom claim enforcement
- Automatic database migrations via GORM
- Static frontend pages for voting, admin, and reporting

---

### Video Server
**Tech Stack:** Go, SQLite, FFmpeg, HTTP/2

A YouTube-style video management and streaming application with passwordless authentication.

**Features:**
- Automatic video ingestion and thumbnail generation via FFmpeg
- Magic-link email authentication for admins
- Per-user access control with audit logging
- Tag/department filtering with watch-progress tracking
- SQLite with automatic schema migration
- Docker and docker-compose support

---

## Data Visualization & Analytics

### Economic Data Dashboard
**Tech Stack:** Python, Flask, D3.js, Redis, Docker

A high-performance dashboard for real-time visualization of economic indicators from FRED, BLS, and US Census Bureau APIs.

**Features:**
- 35+ national economic indicators (unemployment, GDP, inflation, housing)
- Louisiana-specific state-level metrics
- Interactive sparkline charts with 12-month rolling averages
- Gauge view for month-over-month changes
- Parallel data loading with Redis caching
- Circuit breaker pattern for API resilience
- Gunicorn production server with 4 workers

**Dashboards:**
- National Economic Dashboard
- Louisiana State Dashboard  
- BLS Labor Statistics Dashboard
- Census Demographics Dashboard

---

### Charts — Economic Data Visualization Platform
**Tech Stack:** Python, Pandas, GeoPandas, D3.js

Interactive choropleth maps and time-series charts for economic data visualization.

**Features:**
- State and county-level unemployment choropleth maps
- Interactive time controls (slider, play/pause, speed adjustment)
- D3.js time-series charts with zoom/brush functionality
- FIPS code matching and data validation
- Automatic API caching with fallback support
- Support for BLS, FRED, and Census Bureau APIs

**Outputs:**
- State unemployment maps (all 50 states)
- County unemployment maps (3,100+ counties)
- Louisiana parish-level maps
- Individual time-series charts for 100+ economic series

---

## Developer Tools

### PDF/DOCX Redaction Tool
**Tech Stack:** Python 3.13, FastAPI

Production-ready API for automatically redacting sensitive PII from documents.

**Default Redaction (always active):**
- Social Security Numbers (SSN) with strict validation
- Employer Identification Numbers (EIN/FEIN) with prefix validation

**Optional Patterns:**
- Dates of Birth, Credit Cards (Luhn + BIN validation), Phone Numbers
- Email Addresses, IPv4 Addresses, Street Addresses

**Enterprise Features:**
- Structured JSON logging
- Rate limiting per IP
- File size validation
- Async file I/O
- CORS security and API key authentication
- Sentry integration for error monitoring
- Health check endpoint
- Docker support

---

### Interactive OCR Tool
**Tech Stack:** Python, FastAPI, Tesseract

Visual field selector for extracting structured text from forms and images.

**Features:**
- Draw selection boxes directly on images
- Automatic coordinate scaling
- CSV export with proper row/column structure
- Save/load reusable field configurations
- Perfect for processing sign-in sheets, surveys, and applications

---

## Hardware / Embedded Systems

### Arduino Camera Slider Controller
**Tech Stack:** Arduino Nano, C++, PlatformIO, A4988 Driver, OLED Display

A feature-rich motorized camera slider with multiple operating modes.

**Operating Modes:**
- **Manual Mode:** Direct control via rotary encoder
- **Auto Slide Mode:** Continuous back-and-forth motion
- **Timelapse Mode:** Interval-based movements for time-lapse photography

**Features:**
- Smooth acceleration/deceleration via AccelStepper library
- Automatic homing sequence with limit switch
- Real-time OLED display (position in mm, speed, mode)
- NEMA 17 stepper motor with A4988 driver
- 1/16 microstepping for smooth operation

**Hardware:**
- Arduino Nano (ATmega328P)
- NEMA 17 stepper motor
- A4988 stepper driver
- SSD1306 128x64 OLED (I2C)
- KY-040 rotary encoder
- Limit switch for homing

---

### Mail Scale
**Tech Stack:** Arduino Nano, C++, PlatformIO, HX711 Load Cell

A precision digital scale with EEPROM-based calibration persistence.

**Features:**
- HX711 load cell with moving average smoothing
- Stability indicator for accurate readings
- Multiple units: grams, pounds, ounces
- Auto-sleep after 2 minutes of inactivity
- EEPROM storage for calibration data and preferences
- Tare, unit cycle, and factory reset via button controls

---

## Tech Stack Summary

| Category | Technologies |
|----------|-------------|
| **Languages** | Go, Python, TypeScript/JavaScript, C++ |
| **Frontend** | Next.js, React, D3.js, Vanilla JS |
| **Backend** | Go (net/http), Flask, FastAPI, Node.js |
| **Databases** | PostgreSQL, SQLite, Supabase, Pinecone |
| **AI/ML** | OpenAI, Anthropic Claude, Cohere, Google Gemini, Mistral |
| **DevOps** | Docker, Docker Compose, Gunicorn |
| **Caching** | Redis, Upstash |
| **Auth** | Firebase Auth, Supabase Auth, Magic Links |
| **Hardware** | Arduino Nano, ESP32, Stepper Motors, Load Cells |
| **APIs** | FRED, BLS, US Census Bureau, Eleven Labs |

---

## Contact

📧 See [portfolio.danielspears.com](https://portfolio.danielspears.com) for contact information.
