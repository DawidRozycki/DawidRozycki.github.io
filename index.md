---
layout: default
title: Home
---

# 👋 Hey!

I'm a backend developer and entrepreneur passionate about building scalable solutions and innovative products.

<section class="experience-section">
  <h2>Current Projects</h2>
  
  {% assign nexly = site.data.experience | where: "company", "Nexly" | first %}
  <div class="experience-card">
    <div class="experience-header">
      <div class="company-info">
        <img src="{{ nexly.logo }}" alt="{{ nexly.company }} logo" class="company-logo">
        <div class="company-details">
          <h3 class="position-title">{{ nexly.position }}</h3>
          <h4 class="company-name">{{ nexly.company }}</h4>
          <div class="job-meta">
            <span class="duration">{{ nexly.duration }}</span>
            {% if nexly.status %}
            <span class="type" style="background: #f39c12; color: white; padding: 4px 8px; border-radius: 12px; font-size: 0.9em;">{{ nexly.status }}</span>
            {% endif %}
          </div>
        </div>
      </div>
    </div>
    
    <video width="60%" controls style="margin: 20px auto; border-radius: 8px; display: block;">
      <source src="assets/videos/nexly/nexly_hero.mp4" type="video/mp4">
      Your browser does not support the video tag.
    </video>
    
    <div class="experience-content">
      <div class="highlights">
        {% for highlight in nexly.highlights %}
        <div class="highlight-item">
          <h5 class="highlight-title">{{ highlight.title }}</h5>
          <p class="highlight-description">{{ highlight.description }}</p>
        </div>
        {% endfor %}
      </div>
      
      <div class="technologies">
        <strong>Technologies:</strong>
        {% for tech in nexly.technologies %}
        {% if tech == "Python" or tech == "AI" or tech == "MS Azure" or tech == "Google GCP" or tech == "Firebase" %}
        <span class="tech-tag tech-tag-highlight">{{ tech }}</span>
        {% else %}
        <span class="tech-tag">{{ tech }}</span>
        {% endif %}
        {% endfor %}
      </div>
      
      <div style="margin-top: 20px; padding: 15px; background: #f8f9fa; border-radius: 8px; border-left: 4px solid #3498db;">
        <strong>🔗 Links:</strong>
        <div style="margin-top: 10px; display: flex; gap: 15px; flex-wrap: wrap;">
          <a href="/nexly" style="display: inline-block; padding: 8px 16px; background: #3498db; color: white; text-decoration: none; border-radius: 5px; font-weight: 500;">📖 Learn More</a>
          <a href="{{ nexly.website }}" style="display: inline-block; padding: 8px 16px; background: #3498db; color: white; text-decoration: none; border-radius: 5px; font-weight: 500;">🌐 Visit Nexly</a>
        </div>
      </div>
    </div>
  </div>
  
  {% assign nextideas = site.data.experience | where: "company", "NextIdeas.app" | first %}
  <div class="experience-card">
    <div class="experience-header">
      <div class="company-info">
        <img src="{{ nextideas.logo }}" alt="{{ nextideas.company }} logo" class="company-logo">
        <div class="company-details">
          <h3 class="position-title">{{ nextideas.position }}</h3>
          <h4 class="company-name">{{ nextideas.company }}</h4>
          <div class="job-meta">
            <span class="duration">{{ nextideas.duration }}</span>
            {% if nextideas.status %}
            <span class="type" style="background: #27ae60; color: white; padding: 4px 8px; border-radius: 12px; font-size: 0.9em;">{{ nextideas.status }}</span>
            {% endif %}
          </div>
        </div>
      </div>
    </div>
    
    <div style="width: 60%; height: 300px; margin: 20px auto; border-radius: 8px; background: linear-gradient(135deg, #667eea 0%, #764ba2 100%); display: flex; align-items: center; justify-content: center; color: white; font-size: 48px;">
      💡
    </div>
    
    <div class="experience-content">
      <div class="highlights">
        {% for highlight in nextideas.highlights %}
        <div class="highlight-item">
          <h5 class="highlight-title">{{ highlight.title }}</h5>
          <p class="highlight-description">{{ highlight.description }}</p>
        </div>
        {% endfor %}
      </div>
      
      <div class="technologies">
        <strong>Technologies:</strong>
        {% for tech in nextideas.technologies %}
        {% if nextideas.tech_highlights contains tech %}
        <span class="tech-tag tech-tag-highlight">{{ tech }}</span>
        {% else %}
        <span class="tech-tag">{{ tech }}</span>
        {% endif %}
        {% endfor %}
      </div>
      
      <div style="margin-top: 20px; padding: 15px; background: #f8f9fa; border-radius: 8px; border-left: 4px solid #3498db;">
        <strong>🔗 Links:</strong>
        <div style="margin-top: 10px; display: flex; gap: 15px; flex-wrap: wrap;">
          <a href="/nextideas" style="display: inline-block; padding: 8px 16px; background: #3498db; color: white; text-decoration: none; border-radius: 5px; font-weight: 500;">📖 Learn More</a>
          <a href="{{ nextideas.website }}" target="_blank" style="display: inline-block; padding: 8px 16px; background: #3498db; color: white; text-decoration: none; border-radius: 5px; font-weight: 500;">🌐 Visit NextIdeas.app</a>
        </div>
      </div>
    </div>
  </div>
  
  <div class="experience-card">
    <div class="experience-header">
      <div class="company-info">
        <div class="company-details">
          <h3 class="position-title">📄 Curriculum Vitae</h3>
          <h4 class="company-name">Professional Experience & Skills</h4>
        </div>
      </div>
    </div>
    
    <div class="experience-content">
      <p>Backend developer and AI engineer with 7+ years of experience building scalable systems across fintech, banking, and energy sectors. Specialized in Python, AI/ML frameworks (PyTorch, TensorFlow, LangChain), and cloud infrastructure (Azure, GCP, Firebase), with a track record of delivering high-impact solutions from prototype to production.</p>
      
      <div class="highlights">
        <div class="highlight-item">
          <h5 class="highlight-title">Current Focus</h5>
          <p class="highlight-description">• Co-Founder & Lead Backend Developer at Nexly (AI-powered audit automation)</p>
          <p class="highlight-description">• Solo-Founder at NextIdeas.app (AI-driven idea validation platform)</p>
        </div>
        <div class="highlight-item">
          <h5 class="highlight-title">Previous Experience</h5>
          <p class="highlight-description">• Assistant Vice President, Credit Suisse (Credit Portfolio Analytics & Risk Management)</p>
          <p class="highlight-description">• Data Scientist, Standard Chartered Bank (IBOR Transition & Interest Rate Risk Modeling)</p>
          <p class="highlight-description">• Market Risk Specialist, PKO BP & PGE (Derivatives Valuation & Risk Analytics)</p>
        </div>
        <div class="highlight-item">
          <h5 class="highlight-title">Core Expertise</h5>
          <p class="highlight-description">• Multimodal & Generative AI: Document understanding, LLM orchestration, computer vision integration</p>
          <p class="highlight-description">• Distributed Systems: Cloud-native deployment, async pipelines, microservices architecture</p>
          <p class="highlight-description">• Financial Modeling: Credit risk analytics, quantitative modeling, algorithmic validation</p>
        </div>
        <div class="highlight-item">
          <h5 class="highlight-title">Education & Certifications</h5>
          <p class="highlight-description">• Master's in Finance & Accounting (SGH Warsaw School of Economics)</p>
          <p class="highlight-description">• Postgraduate in Data Science (University of Warsaw)</p>
          <p class="highlight-description">• CFA Level 1 (CFA Institute)</p>
        </div>
      </div>
      
      <div style="margin-top: 20px; padding: 15px; background: #f8f9fa; border-radius: 8px; border-left: 4px solid #3498db;">
        <strong>🔗 Links:</strong>
        <div style="margin-top: 10px; display: flex; gap: 15px; flex-wrap: wrap;">
          <a href="/cv" style="display: inline-block; padding: 8px 16px; background: #3498db; color: white; text-decoration: none; border-radius: 5px; font-weight: 500;">📖 View Full CV</a>
        </div>
      </div>
    </div>
  </div>
</section>
