# Delaunay Triangulation Algorithm

## Project Overview

This project implements an **incremental algorithm** for creating **Delaunay triangulations**, a critical operation in computational geometry. The method starts from a base triangle and iteratively adds points while ensuring the triangulation maintains the Delaunay property. The report provides detailed theoretical foundations, algorithmic steps, and implementation strategies.

## Features

- **Convex Hull Construction**: Computes the convex hull of a set of points.
- **Delaunay Triangulation**: Ensures that no point lies inside the circumcircle of any triangle in the triangulation.
- **Flip Propagation**: Dynamically adjusts triangulation to preserve the Delaunay property.
- **Grid-Based Point Initialization (Snake)**: Optimizes the initial choice of points to maximize efficiency.

## Algorithm Description

1. **Initial Setup**:
   - Create a base triangle containing a subset of points.
   - Use a grid structure to optimize the initial point selection (`Snake` operation).

2. **Triangulation Expansion**:
   - Add new points iteratively.
   - Determine if a point is inside or outside the existing triangulation.
   - Update the triangulation by adding new triangles and maintaining the Delaunay property.

3. **Flip Propagation**:
   - Adjust the triangulation locally by flipping edges to satisfy the Delaunay condition.

4. **Finalization**:
   - The resulting triangulation is a Delaunay triangulation.

## Computational Complexity

- Average complexity for point addition: **O(n log n)**.
- Efficient handling of both internal and external points using geometric operations and a pointer-based data structure.

## Getting Started

### Repository Structure

- `Report.pdf`: Technical report with theoretical background, implementation details, and results.
- `Presentation.pdf` / `Presentation.pptx`: Slide deck summarizing the project.
- `LICENSE`: MIT License file.

### Prerequisites

- **Programming Language**: C++
- **Libraries/Dependencies**:
  - [List of required libraries/tools]

### Running the Project

To run the project:

1. Clone the repository:

```bash
git clone https://github.com/MaddalenaGhiotti/DelaunayProject.git
```

2. Navigate to the project directory:

```bash
cd DelaunayProject
```

3. Run the main script (if available):

```bash
python main.py
```

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Authors

- Maddalena Ghiotti
- Aldo Sambo
- Emilio Zorzi
