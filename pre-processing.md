---
layout: page
title: "Pre-processing"
permalink: /pre-processing/
---

<!-- # Pre-processing Tools -->

Pre-processing is the foundational step in seismic data processing, involving the preparation and conditioning of raw seismic data for subsequent analysis. This stage encompasses data format conversion, quality control, filtering, gain adjustments, and geometric corrections. Effective pre-processing is crucial for ensuring data quality and setting up successful downstream processing workflows.

## Available Tools

---

<details class="tool-card collapsible">
  <summary class="tool-header">
    <div style="display: flex; align-items: center; flex: 1;">
      <h3 class="tool-title">SeismicPro</h3>
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
        <strong>Institution:</strong> GeoscienceML
      </div>
      <div class="tool-meta-item">
        <strong>Last Updated:</strong> 2024
      </div>
    </div>
    
    <div class="tool-description">
      <p>SeismicPro is a comprehensive framework for accelerating pre-stack seismic data processing with deep learning models. It provides efficient SEG-Y data handling, extensive processing capabilities, and pipeline-based workflows. The framework combines traditional seismic processing methods with modern deep learning approaches, supporting everything from basic data conditioning to advanced AI-driven analysis.</p>
    </div>
    
    <div class="tool-features">
      <h4>Key Features:</h4>
      <ul>
        <li>Efficient SEG-Y format reading and processing</li>
        <li>Support for stacking velocities and auxiliary data</li>
        <li>Massively parallel data transformation</li>
        <li>Pipeline-based processing workflows</li>
        <li>Integration with deep learning models (UNet, EfficientNet)</li>
        <li>Automatic stacking velocity picking</li>
        <li>NMO correction and gather stacking</li>
        <li>Interactive quality maps and visualization</li>
        <li>Muting and filtering operations</li>
        <li>Comprehensive tutorial documentation</li>
      </ul>
    </div>
    
    <div class="tool-features">
      <h4>Processing Capabilities:</h4>
      <ul>
        <li>Data loading and header management</li>
        <li>Velocity spectrum analysis</li>
        <li>Gather sorting and organization</li>
        <li>Amplitude corrections and scaling</li>
        <li>Noise reduction and filtering</li>
        <li>Geometric transformations</li>
        <li>Quality control and validation</li>
      </ul>
    </div>
    
    <div class="tool-features">
      <h4>Requirements:</h4>
      <ul>
        <li>Python 3.8+</li>
        <li>PyTorch</li>
        <li>segyio for SEG-Y handling</li>
        <li>pandas, numpy</li>
        <li>Compatible with Ubuntu 20.04 and Windows Server 2022</li>
        <li>GPU recommended for deep learning components</li>
      </ul>
    </div>
    
    <div class="tool-links">
      <a href="https://github.com/GeoscienceML/SeismicPro" class="btn btn-primary" target="_blank">View on GitHub</a>
      <a href="https://github.com/GeoscienceML/SeismicPro/blob/master/tutorials" class="btn btn-secondary" target="_blank">Tutorials</a>
    </div>
  </div>
</details>

---

## Contributing New Tools

To add a new pre-processing tool to this page:

1. **Fork this repository**
2. **Edit this file** (`pre-processing.md`)
3. **Add your tool** using the template below
4. **Submit a pull request**

### Tool Template

```markdown
<details class="tool-card collapsible">
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

- [First Break Analysis](/first-break-analysis/) - Automatic picking and analysis tools
- [Velocity Analysis](/) (Coming soon)
- [Migration](/) (Coming soon)

---

*Want to suggest a tool? [Create an issue](https://github.com/dylanmikesell/seismic-software/issues) or [submit a pull request](https://github.com/dylanmikesell/seismic-software/pulls).*