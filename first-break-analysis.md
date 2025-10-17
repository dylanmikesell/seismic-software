---
layout: page
title: "First Break Analysis"
permalink: /first-break-analysis/
---

<!-- # First Break Analysis Tools -->

First break picking is a fundamental step in seismic data processing, involving the identification of the first arrival times of seismic waves. Accurate first break picking is crucial for velocity analysis, static corrections, and overall data quality. This page lists open-source tools specifically designed for automated and semi-automated first break analysis.

## Available Tools

---

<details class="tool-card collapsible" open>
  <summary class="tool-header">
    <div style="display: flex; align-items: center; flex: 1;">
      <h3 class="tool-title">HardPicks</h3>
      <span class="tool-status maintained" style="margin-left: auto;">Actively Maintained</span>
    </div>
    <span class="collapse-indicator">▼</span>
  </summary>
  
  <div class="tool-content">
    <div class="tool-meta">
      <div class="tool-meta-item">
        <strong>Language:</strong> Python
      </div>
      <div class="tool-meta-item">
        <strong>License:</strong> Apache 2.0
      </div>
      <div class="tool-meta-item">
        <strong>Institution:</strong> Mila (Quebec AI Institute)
      </div>
      <div class="tool-meta-item">
        <strong>Last Updated:</strong> 2024
      </div>
    </div>
    
    <div class="tool-description">
      <p>HardPicks is a machine learning-based tool for automatic first break picking in seismic data. Developed at Mila (Quebec AI Institute), it leverages deep learning techniques to provide accurate and robust first break detection across various seismic data types and acquisition geometries.</p>
    </div>
    
    <div class="tool-features">
      <h4>Key Features:</h4>
      <ul>
        <li>Deep learning-based automatic picking algorithm</li>
        <li>Support for multiple seismic data formats</li>
        <li>Robust performance across different acquisition types</li>
        <li>Quality control and uncertainty estimation</li>
        <li>Batch processing capabilities</li>
        <li>Interactive visualization tools</li>
        <li>Comprehensive documentation and examples</li>
      </ul>
    </div>
    
    <div class="tool-features">
      <h4>Requirements:</h4>
      <ul>
        <li>Python 3.7+</li>
        <li>PyTorch</li>
        <li>NumPy, SciPy, Matplotlib</li>
        <li>GPU recommended for large datasets</li>
      </ul>
    </div>
    
    <div class="tool-links">
      <a href="https://github.com/mila-iqia/hardpicks" class="btn btn-primary" target="_blank">View on GitHub</a>
      <a href="https://github.com/mila-iqia/hardpicks#installation" class="btn btn-secondary" target="_blank">Installation Guide</a>
    </div>
  </div>
</details>

---

## Contributing New Tools

To add a new first break analysis tool to this page:

1. **Fork this repository**
2. **Edit this file** (`first-break-analysis.md`)
3. **Add your tool** using the template below
4. **Submit a pull request**

### Tool Template

```markdown
<details class="tool-card collapsible" open>
  <summary class="tool-header">
    <div style="display: flex; align-items: center; flex: 1;">
      <h3 class="tool-title">Tool Name</h3>
      <span class="tool-status [maintained|unmaintained|unknown]" style="margin-left: auto;">Status</span>
    </div>
    <span class="collapse-indicator">▼</span>
  </summary>
  
  <div class="tool-content">
    <div class="tool-meta">
      <div class="tool-meta-item">
        <strong>Language:</strong> Programming Language
      </div>
      <div class="tool-meta-item">
        <strong>License:</strong> License Type
      </div>
      <div class="tool-meta-item">
        <strong>Institution:</strong> Institution/Author
      </div>
      <div class="tool-meta-item">
        <strong>Last Updated:</strong> Year
      </div>
    </div>
    
    <div class="tool-description">
      <p>Brief description of the tool...</p>
    </div>
    
    <div class="tool-features">
      <h4>Key Features:</h4>
      <ul>
        <li>Feature 1</li>
        <li>Feature 2</li>
      </ul>
    </div>
    
    <div class="tool-links">
      <a href="GITHUB_URL" class="btn btn-primary" target="_blank">View on GitHub</a>
      <a href="DOCS_URL" class="btn btn-secondary" target="_blank">Documentation</a>
    </div>
  </div>
</details>
```

## Related Methods

- [Velocity Analysis](/) (Coming soon)
- [Travel Time Tomography](/) (Coming soon)
- [Static Corrections](/) (Coming soon)

---

*Want to suggest a tool? [Create an issue](https://github.com/dylanmikesell/seismic-software/issues) or [submit a pull request](https://github.com/dylanmikesell/seismic-software/pulls).*