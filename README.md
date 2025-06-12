# GNN-Based Market Structure Analysis

This project constructs and visualizes a **stock correlation network** using daily returns from 30 major equities across sectors. It applies graph-based techniques to uncover latent market structure, sectoral clusters, and high-correlation pathways — laying the foundation for GNN-based learning or portfolio modeling.

---

## 📌 Project Highlights

- Collected 10 years of data for 30 large-cap U.S. stocks
- Computed pairwise correlations of log returns
- Constructed undirected stock network with edge thresholding
- Visualized sector-specific clusters with color-coded nodes
- Applications to:
  - Market structure discovery
  - Sector co-movement analysis
  - GNN or graph signal processing foundations

---

## 🧠 Methodology

1. Retrieve daily adjusted close prices via `yfinance`
2. Compute log returns → Pearson correlation matrix
3. Threshold edges at ρ > 0.3 to form adjacency graph
4. Visualize using NetworkX with sector-based color mapping

---

## 🖼 Example Output

![Correlation Network](correlation_network.png)

- Nodes: Stocks, colored by sector
- Edges: Pairwise correlations > 0.3
- Highlights natural clusters (Tech, Energy, Healthcare...)

---

## ⚙️ Run the Code

### 1. Install dependencies:
```bash
pip install pandas yfinance networkx matplotlib seaborn
