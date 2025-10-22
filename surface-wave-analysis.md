---
layout: page
title: "Surface Wave Analysis"
permalink: /surface-wave-analysis/
---

# Surface Wave Analysis Tools

Surface wave analysis is a crucial technique in near-surface geophysics for characterizing the shallow subsurface velocity structure. This method utilizes the dispersive properties of surface waves (primarily Rayleigh waves) to determine shear-wave velocity profiles. Surface wave analysis includes multichannel analysis of surface waves (MASW), spatial autocorrelation (SPAC), and other dispersion-based techniques used in engineering geophysics, earthquake seismology, and environmental studies.

## Available Tools

<details class="tool-card collapsible">
  <summary class="tool-header">
    <div style="display: flex; align-items: center; flex: 1;">
      <h3 class="tool-title">hvsrpy</h3>
      <span class="tool-status maintained" style="margin-left: auto;">Maintained</span>
    </div>
    <span class="collapse-indicator">▼</span>
  </summary>
  
  <div class="tool-content">
    <div class="tool-meta">
      <div class="tool-meta-item">
        <strong>Language:</strong> Python
      </div>
      <div class="tool-meta-item">
        <strong>License:</strong> GPL-3.0
      </div>
      <div class="tool-meta-item">
        <strong>Institution:</strong> Virginia Tech (Joseph P. Vantassel)
      </div>
      <div class="tool-meta-item">
        <strong>Last Updated:</strong> 2025
      </div>
    </div>
    
    <div class="tool-description">
      <p>An open-source Python package for performing horizontal-to-vertical spectral ratio (HVSR) processing of microtremor and earthquake recordings. HVSR is a fundamental technique in surface wave analysis for site characterization and determining fundamental site frequencies.</p>
    </div>
    
    <div class="tool-features">
      <h4>Key Features:</h4>
      <ul>
        <li>Support for multiple data formats (MiniSEED, SAF, MiniShark, SAC, GCF, PEER)</li>
        <li>Multiple methods for combining horizontal components (geometric-mean, arithmetic-mean, etc.)</li>
        <li>Lognormal distribution support for site resonant frequency with uncertainty representation</li>
        <li>Advanced statistical approaches incorporating azimuthal and spatial variability</li>
        <li>Automated window rejection algorithms with frequency-domain processing</li>
        <li>SESAME (2004) peak reliability and clarity criteria checking</li>
        <li>Command line interface (CLI) for batch processing with multiprocessing</li>
        <li>Direct access to raw HVSR data from each time window and azimuth</li>
        <li>Extensive validation and comparison with Geopsy software</li>
      </ul>
    </div>
    
    <div class="tool-links">
      <a href="https://github.com/jpvantassel/hvsrpy" class="btn btn-primary" target="_blank">View on GitHub</a>
      <a href="https://hvsrpy.readthedocs.io/en/latest/" class="btn btn-secondary" target="_blank">Documentation</a>
    </div>
  </div>
</details>

---

## Contributing New Tools

To add a new surface wave analysis tool to this page:

1. **Fork this repository**
2. **Edit this file** (`surface-wave-analysis.md`)
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

- [Pre-processing](/pre-processing/) - Data conditioning and format conversion
- [First Break Analysis](/first-break-analysis/) - Automatic picking and analysis tools
- [Velocity Analysis](/) (Coming soon)
- [Tomography](/) (Coming soon)

---

*Want to suggest a tool? [Create an issue](https://github.com/dylanmikesell/seismic-software/issues) or [submit a pull request](https://github.com/dylanmikesell/seismic-software/pulls).*