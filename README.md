# 🕵️‍♂️ Members Only! - Rails Authentication Project

Welcome to **Members Only!**, an exclusive clubhouse app built with Ruby on Rails. This app demonstrates how to implement authentication using Devise and control access to content based on user sign-in status.

## 📖 Introduction

This project focuses on implementing a simple authentication system where:
- **Logged-in users** can see who wrote each post.
- **Guests** can only view anonymous posts.

The goal is to learn how to use Devise for authentication, associate posts with users, and restrict access to specific features based on user authentication status.

---

## 🚀 Features

- User authentication with Devise
- Post creation by signed-in users
- Posts show anonymous authors to guests
- Members can see who authored each post
- Clean, professional UI using Bootstrap (optional)

---

## 🛠 Tech Stack

- Ruby on Rails
- Devise (Authentication)
- Bootstrap (for styling, optional)
- SQLite (default development database)

---

## 🧱 Models

### User
- `name` :string
- `email` :string (Devise-managed)
- `password` :string (Devise-managed)
- Association: `has_many :posts`

### Post
- `title` :string
- `body` :text
- `user_id` :integer (author)
- Association: `belongs_to :user`

---

## ⚙️ Setup Instructions

### 1. Clone the repo

```bash
git clone https://github.com/yourusername/members-only.git
cd members-only
