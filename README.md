# ArcGIS Portal Title Cleaner
## Overview
This script automates the process of cleaning and standardizing item titles in an ArcGIS Online or Enterprise portal. It connects via ArcGIS Pro (SSO), retrieves all items owned by the user, and renames them by:
- Converting titles to lowercase
- Replacing spaces with underscores
- Collapsing multiple underscores

Web Maps and Web Experiences are skipped, as they do not support renaming via the API.

## Features
- Works with both root and folder items
- Skips unsupported item types
- Retries failed updates up to 3 times
- Provides a summary report of renamed, skipped, and failed items

## Requirements
- ArcGIS Pro installed and signed in
- Python environment with the following packages:
  - `arcgis`
  - `tqdm`

## Installation
```bash
pip install -r requirements.txt# arcgis-title-cleaner
