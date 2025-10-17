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

<details class="tool-card collapsible" open>
  <summary class="tool-header">
    <div style="display: flex; align-items: center; flex: 1;">
      <h3 class="tool-title">FirstBreaksPicking</h3>
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
        <strong>Institution:</strong> DaloroAT
      </div>
      <div class="tool-meta-item">
        <strong>Last Updated:</strong> 2024
      </div>
    </div>
    
    <div class="tool-description">
      <p>FirstBreaksPicking is a robust neural network-based tool for automated first break picking on 2D seismic gathers. Unlike traditional methods that process individual traces, this tool leverages spatial relationships between adjacent traces by processing entire seismic gathers as images, making it more robust to noise and varying data quality conditions.</p>
    </div>
    
    <div class="tool-features">
      <h4>Key Features:</h4>
      <ul>
        <li>UNet3+ neural network architecture for improved accuracy</li>
        <li>2D gather-based processing (not individual traces)</li>
        <li>Desktop GUI application with interactive visualization</li>
        <li>GPU acceleration support (CUDA compatible)</li>
        <li>Robust performance on noisy data</li>
        <li>Real-time parameter adjustment and visualization</li>
        <li>SGY file format support</li>
        <li>Spectrum analysis tools</li>
        <li>Manual picks editing and management</li>
        <li>Compiled executable versions available</li>
      </ul>
    </div>
    
    <div class="tool-features">
      <h4>Requirements:</h4>
      <ul>
        <li>Python 3.7+</li>
        <li>ONNX runtime</li>
        <li>Pre-trained model (downloadable)</li>
        <li>Optional: NVIDIA GPU with CUDA 11.6+ for acceleration</li>
        <li>SGY format seismic data</li>
      </ul>
    </div>
    
    <div class="tool-links">
      <a href="https://github.com/DaloroAT/first_breaks_picking" class="btn btn-primary" target="_blank">View on GitHub</a>
      <a href="https://github.com/DaloroAT/first_breaks_picking#installation" class="btn btn-secondary" target="_blank">Installation Guide</a>
    </div>
  </div>
</details>

<details class="tool-card collapsible" open>
  <summary class="tool-header">
    <div style="display: flex; align-items: center; flex: 1;">
      <h3 class="tool-title">geo-stack First Break Picking</h3>
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
        <strong>License:</strong> MIT
      </div>
      <div class="tool-meta-item">
        <strong>Institution:</strong> geo-stack (Amir Mardan)
      </div>
      <div class="tool-meta-item">
        <strong>Last Updated:</strong> 2024
      </div>
    </div>
    
    <div class="tool-description">
      <p>A comprehensive deep learning framework for first break picking using U-Net segmentation. This tool treats first break picking as a segmentation problem, dividing seismic data into "before FB" and "after FB" segments. The approach includes extensive data preprocessing, augmentation, and training capabilities, making it suitable for both research and production environments.</p>
    </div>
    
    <div class="tool-features">
      <h4>Key Features:</h4>
      <ul>
        <li>U-Net based segmentation approach with ResNet encoder</li>
        <li>Comprehensive data preprocessing pipeline</li>
        <li>Data augmentation with overlapping subimages</li>
        <li>Custom training workflow with validation</li>
        <li>Fine-tuning capabilities for domain adaptation</li>
        <li>Batch processing and single shot prediction modes</li>
        <li>Multiple model architectures (U-Net variants)</li>
        <li>Learning rate scheduling and checkpointing</li>
        <li>Smoothing algorithms for artifact reduction</li>
        <li>Published academic methodology</li>
      </ul>
    </div>
    
    <div class="tool-features">
      <h4>Requirements:</h4>
      <ul>
        <li>Python 3.7+</li>
        <li>PyTorch</li>
        <li>NumPy, Pandas</li>
        <li>Data in .npy and .txt formats</li>
        <li>GPU recommended for training</li>
        <li>Proper dataset preparation with FB annotations</li>
      </ul>
    </div>
    
    <div class="tool-links">
      <a href="https://github.com/geo-stack/first_break_picking" class="btn btn-primary" target="_blank">View on GitHub</a>
      <a href="https://geo-stack.github.io/first_break_picking" class="btn btn-secondary" target="_blank">Documentation</a>
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