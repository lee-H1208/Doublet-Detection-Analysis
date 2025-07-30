# Doublet-Detection-Analysis

![Poster](URECA_Poster.jpg)

## Overview

This repository contains code and analysis comparing six doublet detection methods for single-cell RNA-seq data.
Since this was a group project, I have included all the code that I oversaw.

## Contents

The following folders contain individual notebooks used to run each doublet detection method. These are included to fully demonstrate the usage and configuration of each tool.
- `\COMPOSITE`
- `\DoubletDetection`
- `\Scrublet`
- `\scDblFinder`

These folders contain images that were used for our poster and other analyses.
- `\Graphs`
- `\images`

The following two folders contain separate analyses designed to provide deeper insight into the performance of each doublet detection method.
- `PseudoDoublets`: After removing all doublets identified by any method from each dataset, new artificial doublets were generated using scDblFinder’s `getArtificialDoublets` function. The doublet detection methods were then re-run to evaluate their performance on this clean, labeled dataset.
- `\scDblFinder_experiment`: After removing all doublets identify by any method from each dataset, scDblFinder was conducted on each dataset again. The goal was to see whether the method is biased towards the expected number of doublets of each dataset.

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/Doublet-Detection-Analysis.git
   cd Doublet-Detection-Analysis
