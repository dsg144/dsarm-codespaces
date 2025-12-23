# DSAR Assignments (Codespaces)

This repository is the **Codespaces launchpad** for DSAR labs and exercises. The **course website and Canvas** are the main sources for instructions, due dates, and grading details. Use this repo to open the notebooks in **GitHub Codespaces**, complete the work, then **download your `.ipynb`** and submit it to **Gradescope**.

## What students do each week

1. Open this repo on GitHub.
2. Click **Code** (green button) → **Codespaces** → **Create codespace on main**.
3. In Codespaces, open the assigned notebook from the **labs** or **exercises** folder.
4. Complete the notebook.
5. Download the finished `.ipynb` and submit to **Gradescope**.

## Downloading your notebook for Gradescope

In Codespaces:
- In the file explorer, right-click the notebook file (for example `Lab4.ipynb`)
- Choose **Download…**
- Upload that downloaded `.ipynb` to the Gradescope assignment in Canvas

Tip: Make sure you download the notebook from the **correct folder** and that your latest changes are saved before downloading.

## Repository layout

- `labs/`  
  Lab notebooks and shared lab datasets.

- `labs/data/`  
  Shared datasets grouped by which labs use them (for example `L2L3/`, `L4L5/`).

- `exercises/`  
  Exercise notebooks and any exercise-specific data/assets.

- `.devcontainer/`  
  One shared Codespaces environment for the entire course.

## Assignments index

| Type | Where to find it | Notes |
|---|---|---|
| Labs 1–9 | `labs/Lab1.ipynb` … `labs/Lab9.ipynb` | Labs use shared datasets in `labs/data/` |
| Lab 10 | `labs/Lab10/` | You will **create a new notebook from scratch** in this folder (see Lab 10 directions in Canvas/website) |
| Exercises | `exercises/E##_.../` | Each exercise folder is self-contained with its notebook and supporting files |

## Lab datasets

Lab datasets live here:

- `labs/data/L1/`
- `labs/data/L2L3/`
- `labs/data/L4L5/`
- `labs/data/L6L10/` (if applicable)

Do not rename or edit the original CSV files in `labs/data/`.

## Exercise 8 (Neuroimaging) data behavior

Exercise 8 includes small instructor-provided files in its `data/` folder (for example an ROI mask and QC image). Larger neuroimaging files are **downloaded at runtime** into the exercise’s `data/` subfolders.

- Downloaded subject folders (for example `data/sub-*/`) are intentionally **not tracked by git**.
- If a download fails due to temporary network issues, rerun the download cell or switch subjects as instructed in the notebook.

## Environment and dependencies

This repo uses **one shared environment** for all assignments:
- Codespaces uses the config in `.devcontainer/`
- Python dependencies are installed from the repo’s shared requirements

If you see an import error, first try:
1. Restart the kernel
2. Rebuild the container (Codespaces menu → “Rebuild Container”)
3. Rerun the first setup cells in the notebook (if present)

## Troubleshooting

**My notebook will not run because a file is missing**
- Confirm you opened the notebook from the correct folder (`labs/` vs `exercises/`)
- Confirm you did not change the expected file paths in the starter code
- If the notebook downloads data, rerun the download cell and confirm the target file exists

**I downloaded the notebook but my changes are not there**
- Save the notebook in Codespaces (File → Save)
- Restart the kernel if outputs look stale
- Download again after saving

**Codespaces is slow**
- Close extra notebook tabs
- Restart the kernel
- If needed, rebuild the container

## For instructors and TAs (repo intent)

This repo is intentionally scoped to:
- Launch notebooks in Codespaces reliably
- Provide stable relative file paths
- Keep large runtime downloads out of version control

Course-facing materials, rubrics, directions, and links belong on the course website and in Canvas.
