# 🌌 Universe Database Project

This repository contains the SQL schema and data dump (`universe.sql`) for a fictional universe database designed as part of the [freeCodeCamp.org](https://www.freecodecamp.org/) **Relational Database Certification** project.

The goal of this project is to practice and demonstrate proficiency in creating relational databases using PostgreSQL, with proper data modeling, constraints, and relationships between tables such as galaxies, stars, planets, and moons.

---

## 📂 What's Inside

- `universe.sql`: A complete SQL dump of the `universe` database.
  - Includes `CREATE TABLE` statements
  - Contains data `INSERT` statements
  - Preserves relationships, constraints, and sample data

---

## 🧱 Schema Overview

The database includes the following tables:

- **galaxy**: Represents galaxies in the universe (e.g. Milky Way, Andromeda)
- **star**: Stars belonging to a galaxy (e.g. Sun, Sirius)
- **planet**: Planets orbiting stars (e.g. Earth, Mars)
- **moon**: Moons orbiting planets (e.g. Moon, Europa)
- **planet_type**: (Bonus) A lookup table for types of planets (e.g. Terrestrial, Gas Giant)

Each table includes appropriate data types, primary keys, foreign keys, constraints (`NOT NULL`, `UNIQUE`), and realistic sample data.

---

## ✅ Features

- 5+ relational tables with realistic structure
- Proper use of `INT`, `BOOLEAN`, `NUMERIC`, `TEXT`, and `VARCHAR`
- At least 3 rows per table (and more for stars, planets, moons)
- Foreign key relationships enforced
- All `name` fields are `VARCHAR` and unique
- `pg_dump` exported file is ready for restoration

---

## 🚀 Getting Started

To restore the database:

```bash
psql -U postgres < universe.sql
