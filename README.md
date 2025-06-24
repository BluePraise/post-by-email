# Post by Email

A modern, secure, and minimal solution to publish blog posts by sending an email.

## ✨ What is this project?

Post by Email lets you publish content to your static site generator (SSG) by sending an email. No need to log in to a CMS, no browser tabs, no distractions—just write an email and hit send.

## 🎯 Why build this?

Logging in to a CMS or creating yet another platform account is often unnecessary friction. WordPress supports email-based posting but is bloated and insecure. This project is a cleaner alternative, engineered from scratch with security, performance, and developer experience in mind.

## 🧠 What I'm Learning

- Full-stack development techniques
- Email parsing and handling
- Secure service design and authentication
- AWS (SES, Lambda, S3, IAM)
- DevOps workflows (CI/CD, logging, error handling)
- Build versioning and release management
- GitHub integrations (Probot, auto-triage bots)

## 🛠️ Tech Stack (Planned)

- Node.js / Express
- AWS SES for inbound email
- AWS Lambda for processing
- S3 for media storage
- GitHub Actions for CI
- A static site generator like Astro or Eleventy

## 🚧 Milestones

1. Define email format and content schema
2. Set up email receiving and forwarding (SES)
3. Parse and sanitize incoming email
4. Store images in S3
5. Generate markdown post and trigger SSG build
6. Secure access, validate sender
7. Deploy initial version and test
8. Add GitHub issue triage via Probot

## 📬 How It Works (Planned)

1. User sends an email to a custom address
2. SES receives and routes the email to a Lambda function
3. The function extracts content and attachments
4. It saves media to S3 and generates markdown
5. Triggers a rebuild of the SSG site

## 🧭 Future Plans & Features

- CLI installer for interactive setup (`npx create-post-by-email`)
- Git-based media storage option
- Developer documentation:
  - `INSTALL.md` with step-by-step instructions
  - `docs/setup-aws.md` for AWS integration
  - `docs/using-with-eleventy.md` for SSG integration
- Sample content in the `examples/` directory
- GitHub Actions workflow for CI/CD and validation
- Authentication and multi-user support:
  - Verified sender list
  - HMAC or JWT signature checks
  - Optional dashboard for post management

## 📝 License

MIT
