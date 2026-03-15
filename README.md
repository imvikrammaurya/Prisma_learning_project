# Job Board Platform

## Introduction

A full-stack Job Board Platform that allows users to post, discover, and apply for job opportunities in a seamless way.

The application includes secure authentication, dynamic job pages, and a personalized dashboard where users can manage their job listings and applications. Recruiters can post job offers with details such as title, description, job type, and location, while job seekers can easily search and apply for relevant positions.

Jobs can be filtered using advanced search powered by Prisma query filters, and each job has its own dynamic detail page with a simple Apply workflow.

This project demonstrates modern full-stack development using Next.js, Prisma, PostgreSQL, and TailwindCSS.

---

## Tech Stack

- **TypeScript** – Static typing and better developer experience
- **Next.js 16** – Full-stack React framework with Server Components
- **Prisma** – Type-safe ORM for database management
- **PostgreSQL** – Relational database
- **TailwindCSS** – Utility-first CSS framework for styling
- **React Hooks** – Client-side state and UI interactivity
- **NextAuth.js** – Authentication and session management

---

## Features

### Post Job Offers

Authenticated users can create job postings with title, description, job type, and location.

### Advanced Search

Search and filter jobs by:

- Keyword
- Job type (Full-time, Part-time, Contract)
- Location

Powered by Prisma query filters for efficient database searching.

### User Dashboard

Users can manage their activity through a personalized dashboard:

- View posted jobs
- See number of applicants for each job

### Job Applications

Users can apply to available jobs. The dashboard shows all submitted applications along with their statuses.

### Dynamic Job Pages

Each job has its own dynamic route displaying detailed information and an Apply button.

### Authentication and Authorization

Users must be signed in to:

- Post job listings
- Apply to jobs

Authentication is handled using NextAuth.js.

---

## Getting Started

### Prerequisites

Make sure you have installed:

- **Node.js (v18 or higher)**
- **PostgreSQL**

---

## Installation

Clone the repository:

```bash
git clone https://github.com/imvikrammaurya/Prisma_learning_project.git
cd Prisma_learning_project
```

Install dependencies:

```bash
npm install
```

---

## Environment Variables

Create a `.env` file in the root directory.

Example:

```env
DATABASE_URL="postgresql://USER:PASSWORD@localhost:5432/jobboard"
NEXTAUTH_SECRET=your_secret_key
NEXTAUTH_URL=http://localhost:3000
```

---

## Database Setup

Run Prisma commands to generate the client and apply migrations:

```bash
npx prisma generate
npx prisma migrate dev
```

---

## Run the Development Server

```bash
npm run dev
```

The application will be available at:

```
http://localhost:3000
```

---

## Useful Resources

Next.js Documentation  
https://nextjs.org/docs

Prisma Documentation  
https://www.prisma.io/docs

PostgreSQL Documentation  
https://www.postgresql.org/docs/

Tailwind CSS Documentation  
https://tailwindcss.com/docs

Vercel Deployment Platform  
https://vercel.com/

---

## Future Improvements

- Job bookmarking
- Email notifications for applications
- Admin moderation panel
- Resume uploads

---

## License

This project is open-source and available under the MIT License.
