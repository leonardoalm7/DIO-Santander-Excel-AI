# Financial Investment Simulator  

**Project from Bootcamp Santander - Excel with Artificial Intelligence**  
*Course taught on [DIO (Digital Innovation One)](https://www.dio.me/)*  

## 📌 Overview  
This Excel-based financial simulator helps users project long-term investment growth based on monthly contributions, expected returns, and risk profiles (Conservative, Moderate, or Aggressive). It also suggests asset allocation for Real Estate Investment Funds (FIIs) according to the selected profile.

---

## 🛠️ Features  
- **Salary-Based Investment Suggestion**: Recommends investing 30% of the entered salary.  
- **Future Value Projections**: Calculates accumulated wealth and monthly dividends over 2, 5, 10, 20, or 30 years.  
- **Customizable Inputs**:  
  - Monthly investment amount (`Quanto investir por mês?`).  
  - Investment duration (`Por Quantos Anos?`).  
  - Expected monthly return (`Taxa de Rendimento mensal?`).  
- **Risk Profile Allocation**:  
  - Automatically suggests FII portfolio distribution (PAPEL, TIJOLO, HÍBRIDOS, etc.) based on the selected profile (Moderate by default).  

---

## 📊 How It Works  
### 1. **Configuration Tab (`Simulacao`)**  
- Enter your **salary** (e.g., R$10,000) to see the suggested investment (30%).  
- Adjust the **monthly investment**, **duration**, and **expected return rate** in the `INVESTIMENTO MENSAL` section.  
- View projected wealth (`Patrimônio acumulado`) and dividends (`Dividendos Mensais`) in the results table.  

### 2. **FII Allocation**  
- The tool uses a **Database** sheet to fetch recommended FII allocations (% per type) based on your risk profile.  
- Example: A "Moderate" profile allocates 32% to PAPEL, 35% to TIJOLO, etc.  

---

## 🔍 Key Formulas  
- **Future Value (FV)**: `=FV(taxa_mensal, qtd_anos*12, aporte*-1)`  
- **Dividends Calculation**: `=patrimonio*rendimento_carteira`  
- **Dynamic FII Allocation**: Uses `VLOOKUP` to match risk profiles with predefined % allocations.  

---

## 📥 How to Use  
1. Download the `Simulador_Financeiro_Leonardo_Braga_de_Almeida.xlsx` file.  
2. Open in Excel or Google Sheets.  
3. Update the yellow-highlighted fields in the `Simulacao` tab:  
   - **Salário** (Salary)  
   - **Quanto investir por mês?** (Monthly investment)  
   - **Por Quantos Anos?** (Investment duration)  
4. Review the projected results and FII allocation table.  

---

## 🎓 Course Context  
Developed as part of the **Bootcamp Santander - Excel with AI** on [DIO](https://www.dio.me/), this project demonstrates advanced Excel functions (FV, VLOOKUP) and financial planning concepts.  
