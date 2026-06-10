# 📊 Amity Investment Performance Dashboard — R Shiny

An interactive **R Shiny** dashboard for investment performance analysis and portfolio reporting. The application integrates multiple financial datasets to deliver dynamic, real-time insights for institutional investment managers.

---

## 🚀 Features

- **Multi-Asset Class Tracking** — Monitors performance across equities, fixed income, hedge funds, and alternative assets
- - **Fund Performance Metrics** — Calculates returns, volatility, Sharpe ratios, and drawdowns
  - - **Benchmark Comparisons** — Side-by-side comparison against major benchmarks
    - - **Dynamic Visualizations** — Interactive charts powered by `ggplot2`, `plotly`, and `highcharter`
      - - **Automated Reporting** — Generates performance reporting from structured Excel data sources
        - - **Modular Shiny Architecture** — Separated into `global.R`, `ui.R`, `server.R`, and `app.R` for maintainability
         
          - ---

          ## 📂 Project Structure

          ```
          Amity-Investment-Performance-Dashboard-R-Shiny/
          │
          ├── app.R               # Main Shiny app entry point
          ├── global.R            # Global data loading, preprocessing, and library imports
          ├── ui.R                # User Interface layout and component definitions
          ├── server.R            # Server-side reactive logic and computations
          │
          ├── data/               # Input data files (Excel-based)
          │   ├── Amity Performance Reporting Monthly.xlsx
          │   ├── Asset Class Returns Data.xlsx
          │   └── HNA_Excel_20250501.xlsx
          │
          ├── docs/
          │   └── R Dashboard build Review.pptx  # Dashboard architecture documentation
          │
          ├── .gitignore
          └── README.md
          ```

          ---

          ## 🛠️ Requirements

          ### R Version
          - R >= 4.0.0
          - - RStudio (recommended)
           
            - ### Required R Packages
           
            - ```r
              install.packages(c(
                "shiny",
                "shinydashboard",
                "shinydashboardPlus",
                "shinyWidgets",
                "ggplot2",
                "plotly",
                "dplyr",
                "tidyr",
                "readxl",
                "lubridate",
                "scales",
                "DT",
                "highcharter",
                "PerformanceAnalytics",
                "xts",
                "zoo"
              ))
              ```

              ---

              ## ⚙️ How to Run

              1. **Clone the repository**
              2. ```bash
                 git clone https://github.com/DrUsama92/Amity-Investment-Performance-Dashboard-R-Shiny.git
                 cd Amity-Investment-Performance-Dashboard-R-Shiny
                 ```

                 2. **Install required packages** (see above)
                
                 3. 3. **Place data files** in the `data/` directory
                   
                    4. 4. **Launch the app** in RStudio:
                       5. ```r
                          shiny::runApp()
                          ```

                          Or run directly from the terminal:
                          ```bash
                          Rscript -e "shiny::runApp('.')"
                          ```

                          ---

                          ## 📊 Data Sources

                          The dashboard ingests structured Excel files containing:
                          - **Monthly performance data** — Fund-level and portfolio-level returns
                          - - **Asset class return data** — Multi-asset benchmark and return series
                            - - **Portfolio holdings data** — Position-level data for attribution analysis
                             
                              - > Note: Due to confidentiality, raw data files are not included in this repository. Please supply your own data following the expected schema.
                                >
                                > ---
                                >
                                > ## 🧮 Key Metrics Computed
                                >
                                > | Metric | Description |
                                > |--------|-------------|
                                > | Total Return | Cumulative portfolio return over selected period |
                                > | Annualized Return | Geometric annualized performance |
                                > | Volatility | Annualized standard deviation of returns |
                                > | Sharpe Ratio | Risk-adjusted return (excess return / volatility) |
                                > | Max Drawdown | Largest peak-to-trough decline |
                                > | Information Ratio | Active return relative to tracking error |
                                > | Benchmark Alpha | Excess return vs. selected benchmark |
                                >
                                > ---
                                >
                                > ## 📸 Dashboard Overview
                                >
                                > The dashboard is organized into the following modules:
                                >
                                > - **Performance Overview** — Summary KPIs, sparklines, and period selectors
                                > - - **Fund Analysis** — Deep-dive into individual fund metrics and attribution
                                >   - - **Asset Allocation** — Pie/donut charts and allocation drift
                                >     - - **Risk Metrics** — Volatility, drawdown, and correlation matrix
                                >       - - **Comparative Analysis** — Cross-fund and cross-benchmark comparison tables
                                >        
                                >         - ---
                                >
                                > ## 👤 Author
                                >
                                > **Dr. Usama Khan**
                                > Data Scientist & Statistician | Financial Analytics Expert
                                > [GitHub](https://github.com/DrUsama92) | [LinkedIn](https://linkedin.com/in/dr-usama)
                                >
                                > ---
                                >
                                > ## 📄 License
                                >
                                > This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
                                >
                                > ---
                                >
                                > ## 🔗 Related Projects
                                >
                                > - [Investment-Performance-Risk-Analytics-Dashboard-R-Shiny-](https://github.com/DrUsama92/Investment-Performance-Risk-Analytics-Dashboard-R-Shiny-)
                                > - - [R-Shiny-Dashboard-_Structured-Finance-Regulatory-Capital-Analytics](https://github.com/DrUsama92/R-Shiny-Dashboard-_Structured-Finance-Regulatory-Capital-Analytics)
