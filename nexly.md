---
layout: default
title: Nexly
---

{% include back_to_home.html %}

{% assign nexly = site.data.experience | where: "company", "Nexly" | first %}

# {{ nexly.company }} - {{ nexly.position }}

<div style="text-align: center; margin: 20px 0;">
  <a href="https://github.com/davidRozycki">
    <img src="http://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=davidRozycki&theme=default" alt="GitHub Profile Details" style="max-width: 100%; height: auto;">
  </a>
</div>

**Development Activity:**
- 🚀 **300+ contributions** in 2024
- 🚀 **500+ contributions** in 2025
- ✅ **Hundreds of Jira tasks** completed, pull requests authored and reviewed
- 🎯 **Dozens of features** shipped to production

---

## Overview

<video width="100%" controls>
  <source src="assets/videos/nexly_hero.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

Nexly is a platform that automates financial statement review. As co-founder and backend developer, I've built the technical foundation and core features that power the platform.

**What Nexly does:**
- Automates the review process of financial statements, saving time and reducing risk
- Helps Auditors and Accountants find discrepancies in financials, before they get published
- Empowers teams and their stakeholders to collaborate on financial statement review

---

## Features

<section class="experience-section">
  <!-- 1. Mathematical Accuracy -->
  <div class="experience-card">
    <div class="experience-header">
      <div class="company-info">
        <div class="company-details">
          <h3 class="position-title">Mathematical Accuracy</h3>
        </div>
      </div>
    </div>
    
    <video width="80%" controls style="margin: 20px auto; border-radius: 8px; display: block;">
      <source src="assets/videos/nexly_ma.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
    
    <div class="experience-content">
      <p>Automatically validate mathematical accuracy across all tables in financial documents, eliminating calculation errors before publication.</p>
      
      <div class="highlights">
        <div class="highlight-item">
          <p class="highlight-description">• Comprehensive validation of all sums and calculations throughout the document</p>
        </div>
        <div class="highlight-item">
          <p class="highlight-description">• Multi-directional sum verification (horizontal, vertical, and cross-table calculations)</p>
        </div>
        <div class="highlight-item">
          <p class="highlight-description">• Advanced handling of complex tables with non-adjacent sum components and nested calculations</p>
        </div>
      </div>
    </div>
  </div>
  
  <!-- 2. Internal Consistency -->
  <div class="experience-card">
    <div class="experience-header">
      <div class="company-info">
        <div class="company-details">
          <h3 class="position-title">Internal Consistency</h3>
        </div>
      </div>
    </div>
    
    <video width="80%" controls style="margin: 20px auto; border-radius: 8px; display: block;">
      <source src="assets/videos/nexly_ic.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
    
    <div class="experience-content">
      <p>Intelligently link and cross-reference values throughout financial documents, ensuring consistency and enabling rapid navigation between related items.</p>
      
      <div class="highlights">
        <div class="highlight-item">
          <p class="highlight-description">• Smart linking between all document sections, connecting related values across statements and notes</p>
        </div>
        <div class="highlight-item">
          <p class="highlight-description">• Context-aware matching that goes beyond simple text search, understanding financial relationships</p>
        </div>
        <div class="highlight-item">
          <p class="highlight-description">• Instant navigation between primary statements, footnotes, and supporting schedules</p>
        </div>
      </div>
    </div>
  </div>
  
  <!-- 3. Prior Year Consistency -->
  <div class="experience-card">
    <div class="experience-header">
      <div class="company-info">
        <div class="company-details">
          <h3 class="position-title">Prior Year Consistency</h3>
        </div>
      </div>
    </div>
    
    <video width="80%" controls style="margin: 20px auto; border-radius: 8px; display: block;">
      <source src="assets/videos/nexly_pyc.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
    
    <div class="experience-content">
      <p>Automatically compare current year figures with prior year data to identify discrepancies, reclassifications, and ensure comparative accuracy.</p>
      
      <div class="highlights">
        <div class="highlight-item">
          <p class="highlight-description">• Automated comparison of current and prior year financial statement line items</p>
        </div>
        <div class="highlight-item">
          <p class="highlight-description">• Detection of unexplained variances and potential reclassification issues</p>
        </div>
        <div class="highlight-item">
          <p class="highlight-description">• Validation of opening balance consistency and comparative period adjustments</p>
        </div>
      </div>
    </div>
  </div>
  
  <!-- 4. Nexly AI Chat -->
  <div class="experience-card">
    <div class="experience-header">
      <div class="company-info">
        <div class="company-details">
          <h3 class="position-title">Nexly AI</h3>
        </div>
      </div>
    </div>
    
    <video width="80%" controls style="margin: 20px auto; border-radius: 8px; display: block;">
      <source src="assets/videos/nexly_ai_chat.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
    
    <div class="experience-content">
      <p>Interact with your financial statements through our specialized AI assistant, trained specifically on financial frameworks and accounting standards.</p>
      
      <div class="highlights">
        <div class="highlight-item">
          <p class="highlight-description">• Framework-aware AI model trained on accounting standards, eliminating financial reporting hallucinations</p>
        </div>
        <div class="highlight-item">
          <p class="highlight-description">• Comprehensive analysis of primary statements, notes, and disclosures with framework compliance insights</p>
        </div>
        <div class="highlight-item">
          <p class="highlight-description">• Intelligent completeness assessment for notes and disclosures based on applicable reporting frameworks</p>
        </div>
      </div>
    </div>
  </div>
</section>

---

## My Involvement

### Technical Leadership

As co-founder and backend developer, I've been responsible for:

- **Architecture Design:** In partnership with our CTO, designed and implemented a dual-architecture backend system combining event-driven document processing pipelines with a microservices-based AI agent orchestration layer. Selected Firebase for real-time document state management, Azure and Google Cloud for OCR services, and FastAPI for the AI agents microservice, enabling horizontal scalability and independent deployment of intelligent validation components.
- **System Design:** Architected our internal pipeline-manager, an event-driven document processing system using Firebase listeners and async worker queues that processes financial documents through multiple stages (OCR extraction, table normalization, value extraction, validation). Designed the AI Agents microservice with LangGraph-based workflows, enabling complex multi-step reasoning chains for financial statement validation with support for multiple LLM providers (OpenAI, Claude, Gemini).
- **Technical Decisions:** 
  - Implemented multi-OCR strategy (including Azure OCR) to achieve 95%+ accuracy on complex financial tables, reducing manual review time by 60%
  - Designed unified LLM service with automatic provider fallback and rate limiting, reducing API costs by 40% while maintaining nearly 100% availability
  - Adopted async-first architecture with asyncio throughout the stack, enabling processing of many documents concurrently on single VM instances (or multiple VM for horizontal scaling)

### Development Work

**Core Features Built:**
- **Multi-Provider LLM Service with Intelligent Fallback:**
  - Built unified interface supporting OpenAI, Anthropic Claude, and Google Gemini with automatic provider switching, retry logic with exponential backoff, and rate limiting. Implemented structured output parsing with Pydantic validation, reducing LLM response errors and enabling seamless model upgrades without code changes.

- **Mathematical Accuracy (MA) Filtering System**
  - Developed sophisticated pattern-based validation filtering service that analyzes financial statement calculations, identifies false positives using statistical thresholds, and filters out noise from validation results. Reduced false positive validation alerts by 70%, significantly improving reviewer efficiency and system trust.
  - Reference reports analyzed with Nexly achieved a Mathematical Accuracy score of:
    - 95% in terms of **Coverage** (identified total rows, both horizontal and vertical)
    - 90%+ in terms of **Accuracy** (True Positives + True Negatives)
    - Less than 10% **Error Rate** (False Positives + False Negatives)
  
- **Advanced Table Normalization Pipeline:**
  - Engineered table processing system handling merged cells, complex layouts, and coordinate-based value linking. Integrated Claude AI for intelligent table structure normalization, achieving 90%+ accuracy on complex financial tables with nested headers and irregular layouts.
  
- **Prior Year (PY) Validation Agent:**
  - Designed and implemented specialized AI agent for cross-year financial statement consistency validation. Built three distinct workflow types (extracted values, linked objects, table links) with procedural step execution, Firebase integration for data fetching, and comprehensive error handling.
  
- **Value Normalization & Multi-Format Number Parsing:**
  - Created robust number parsing system supporting US, European, Indian, and other international formats with automatic format detection, currency symbol handling, and decimal precision preservation. Handles edge cases like parenthetical negatives, thousands separators, and mixed formats within single documents.
  
- **Real-Time Document Processing Pipeline):**
  - Architected event-driven pipeline using Firebase real-time listeners, async worker queues, and state machine pattern for document lifecycle management. Supports multiple document types with configurable processing stages, automatic retries, and comprehensive status tracking. Processes documents end-to-end in a few minutes.

**Technology Stack:**
- **Backend:** Python 3.12, FastAPI, asyncio/aiohttp, LangChain, LangGraph, Pydantic, Poetry
- **Databases:** Firebase Firestore (real-time document state), Firebase Storage (document files), in-memory caching
- **Infrastructure:** Google Cloud Platform (Vertex AI, Document AI), Azure (Document Intelligence, OpenAI), Docker containerization, cloud Linux VMs
- **APIs & Integration:**
  - RESTful APIs with FastAPI (AI agents microservice)
  - Firebase Admin SDK for real-time listeners and data management
  - Multi-provider LLM APIs (OpenAI, Anthropic, Google Gemini) with unified interface
  - Azure Document Intelligence and Google Document AI for OCR, as well as Tesseract and Ghostscript
  - Sentry for error tracking and performance monitoring

### Impact & Achievements

- **Scale:** [Metric about users, requests, data processed]
- **Performance:** [Performance improvements you achieved]
- **Reliability:** [Uptime, error rates, system stability]
- **Team:** [If you built or led a team]

---

## Technical Challenges & Solutions

### Challenge 1: [Name of challenge]
**Problem:** [Describe the technical challenge]  
**Solution:** [How you solved it]  
**Result:** [The outcome and impact]

### Challenge 2: [Name of challenge]
**Problem:** [Describe the technical challenge]  
**Solution:** [How you solved it]  
**Result:** [The outcome and impact]

---

{% include back_to_home.html %}
