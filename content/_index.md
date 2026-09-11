---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2026-01-05
type: landing

sections:
  # Developer Hero - Gradient background with name, role, social, and CTAs
  - block: dev-hero
    id: hero
    content:
      username: me
      greeting: "Hi, I'm"
      name: "Atharva B."
      show_status: true
      show_scroll_indicator: false
      typewriter:
        enable: true
        prefix: "I focus on"
        strings:
          - "DSA and problem solving"
          - "system design and core concepts"
          - "backend systems"
          - "applied AI workflows"
        type_speed: 70
        delete_speed: 40
        pause_time: 2500
      cta_buttons:
        - text: View My Work
          url: "#projects"
          icon: arrow-down
        - text: Download Resume
          url: "/uploads/resume.pdf"
          icon: arrow-down-tray
    design:
      style: centered
      avatar_shape: circle
      animations: true
      background:
        color:
          light: "#fafafa"
          dark: "#0a0a0f"
      spacing:
        padding: ["2.5rem", "0", "3rem", "0"]
  
  # Filterable Portfolio - Alpine.js powered project filtering
  - block: portfolio
    id: projects
    content:
      title: "Selected Projects"
      subtitle: "A focused mix of systems engineering, applied AI, and security work"
      count: 0
      filters:
        folders:
          - projects
      buttons:
        - name: All
          tag: '*'
        - name: AI & Backend
          tag: AI-Backend
        - name: Systems
          tag: Systems
        - name: Security
          tag: Security
      default_button_index: 0
    design:
      columns: 3
      background:
        color:
          light: "#ffffff"
          dark: "#0d0d12"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]
  
  # Visual Tech Stack - Icons organized by category
  - block: tech-stack
    id: skills
    content:
      title: "Tech Stack"
      subtitle: "The core tools I use across systems engineering, backend work, and applied AI"
      categories:
        - name: Languages & Core
          items:
            - name: Python
              icon: devicon/python
            - name: C
              icon: devicon/c
            - name: TypeScript
              icon: devicon/typescript
            - name: Assembly (x86_64)
              icon: devicon/gcc
            - name: Bash
              icon: devicon/bash
            - name: SQL
              icon: devicon/postgresql
        - name: Backend & Systems
          items:
            - name: FastAPI
              icon: devicon/fastapi
            - name: Django
              icon: devicon/python
            - name: Redis
              icon: devicon/redis
            - name: PostgreSQL
              icon: devicon/postgresql
        - name: AI Tools & Frameworks
          items:
            - name: Ollama
              icon: devicon/python
            - name: MCP
              icon: devicon/python
            - name: Pinecone
              icon: devicon/python
            - name: PyTorch
              icon: devicon/pytorch
            - name: TensorFlow
              icon: devicon/tensorflow
        - name: DevOps & Environment
          items:
            - name: Docker
              icon: devicon/docker
            - name: Kubernetes
              icon: devicon/kubernetes
            - name: AWS
              icon: devicon/amazonwebservices
            - name: Linux (Arch)
              icon: devicon/archlinux
    design:
      style: grid
      show_levels: false
      background:
        color:
          light: "#f5f5f5"
          dark: "#08080c"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]
  
  # Experience Timeline
  - block: resume-experience
    id: experience
    content:
      title: Professional Experience
      date_format: Jan 2006
      items:
        - title: Cyber Security Intern
          company: VCF Cyber Solutions Pvt. Ltd.
          company_url: ''
          company_logo: ''
          location: Remote
          date_start: '2025-12-01'
          date_end: '2026-03-31'
          description: |2-
            * Analyzed security architecture across 7 core infrastructure domains (Network, Cloud, Endpoint, IAM)
            * Performed vulnerability assessments using Nmap, Wireshark, and Aircrack-ng across 15+ subnet segments
            * Replicated attack vectors using Metasploit and authored 20+ technical mitigation reports
        - title: Software Engineer Intern
          company: Apexa IQ
          company_url: ''
          company_logo: ''
          location: Remote
          date_start: '2025-09-01'
          date_end: '2025-10-31'
          description: |2-
            * Built Python REST APIs (FastAPI) maintaining sub-500ms latency across high-throughput endpoints
            * Authored 40+ pages of detailed technical documentation, reducing developer setup time by 2 weeks
            * Containerized microservice environments using Docker for standardized deployment workflows
        - title: Technical Advisor
          company: Mozilla Open Source Community
          company_url: ''
          company_logo: ''
          location: Shegaon, India
          date_start: '2023-08-01'
          date_end: '2024-08-31'
          description: |2-
            * Led hands-on technical sessions on Git, Linux command line, and Web Security for 50+ junior students
            * Mentored 15+ peers on open-source contribution practices, leading to 5 accepted external PRs
    design:
      columns: '1'
      background:
        color:
          light: "#ffffff"
          dark: "#0d0d12"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]
  
  # Publications
  - block: collection
    id: publications
    content:
      title: Publications
      subtitle: 'Recent writing and Medium posts on security, privacy, and web abuse detection'
      text: ''
      filters:
        folders:
          - publications
        exclude_featured: false
      count: 3
      order: desc
    design:
      view: card
      columns: 3
      background:
        color:
          light: "#f5f5f5"
          dark: "#08080c"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]
  
  # Contact Section
  - block: contact-info
    id: contact
    content:
      title: Get In Touch
      subtitle: "Let's build reliable systems and AI products together"
      text: |-
        I'm especially interested in AI engineering, systems engineering, backend development, and real-world problem solving.
        If you're hiring for an internship or want to discuss practical engineering work, feel free to reach out.
      email: atharvabodade@gmail.com
      autolink: true
    design:
      columns: '1'
      background:
        color:
          light: "#ffffff"
          dark: "#0d0d12"
      spacing:
        padding: ["4rem", "0", "4rem", "0"]
  
  # CTA Card
  - block: cta-card
    content:
      title: "Open to Opportunities"
      text: |-
        I am a final-year Information Technology student seeking **AI Engineering**, **Systems Engineering**, or **Backend** internship roles.
        
        I learn quickly, adapt to new tools fast, and like turning core concepts into practical software.
      button:
        text: 'Download Resume'
        url: /uploads/resume.pdf
        new_tab: true
    design:
      card:
        css_class: 'bg-gradient-to-br from-primary-200 via-primary-100 to-secondary-200 dark:from-primary-600 dark:via-primary-700 dark:to-secondary-700'
        text_color: dark
      background:
        color:
          light: "#f5f5f5"
          dark: "#08080c"
      spacing:
        padding: ["4rem", "0", "6rem", "0"]
---
