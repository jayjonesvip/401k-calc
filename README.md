# 401k Retirement Calculator

## Preview
https://jayjonesvip.github.io/401k-calc/

## Overview
An interactive web-based 401k retirement savings calculator that helps users visualize their retirement savings growth from current age to retirement at 65. Features real-time adjustments with sliders and dynamic chart updates.

## Features

### Initial Input Form
- **Current Age**: Enter your age (18-64)
- **Current 401k Balance**: Your existing retirement savings
- **Annual Gross Salary**: Your current yearly income
- **Contribution Percentage**: What percent of your salary you contribute
- **Employer Match**: Optional checkbox (assumes employer matches up to 6%)

### Interactive Sliders
- **Contribution Percentage** (0-30%): Adjust how much you want to contribute
- **Annual Return Rate** (0-15%): Modify expected investment returns (default 5%)
- **Annual Salary Raise** (0-10%): Set expected yearly salary increases (default 2%)

### Display Elements
- **Total at Retirement**: Final balance at age 65
- **Starting Balance**: Your current 401k amount
- **Your Contributions**: Total amount you will contribute
- **Employer Match**: Total employer contributions
- **Investment Earnings**: Growth from compound interest
- **Interactive Chart**: Visual line graph showing balance growth over time

## How to Use

1. **Open the HTML file** in any modern web browser (Chrome, Firefox, Safari, Edge)

2. **Enter your information** in the input form:
   - Your current age
   - Current 401k balance
   - Annual salary
   - Contribution percentage
   - Check employer match if applicable

3. **Click "Calculate Retirement Plan"** to generate your projection

4. **Adjust the sliders** to explore different scenarios:
   - Increase contributions to see accelerated growth
   - Compare different return rates
   - Model salary increases over time
   - Watch the chart update in real-time

## Assumptions

- Retirement age is fixed at 65
- Employer match caps at 6% (if enabled)
- Annual raise compounds each year
- Investment returns compound annually
- No withdrawal penalties or taxes calculated
- Consistent contribution percentage throughout career

## Technical Details

### Technologies Used
- HTML5
- CSS3 (with gradients and modern styling)
- Vanilla JavaScript (no frameworks required)
- Chart.js 3.9.1 (loaded via CDN)

### Browser Compatibility
- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

### File Structure
```
401k-calculator/
├── index.html          (Main application file)
└── README.txt          (This file)
```

## Installation

No installation required! Simply:
1. Download the HTML file
2. Double-click to open in your default browser
3. Start calculating

OR

Host on any web server for online access.

## Calculations

### Annual Contribution Growth
```
Year 1 Contribution = Salary × Contribution%
Year 2 Contribution = (Salary × (1 + Raise%)) × Contribution%
Year N Contribution = (Salary × (1 + Raise%)^N) × Contribution%
```

### Balance Growth
```
Balance[year] = Balance[year-1] × (1 + ROI%) + Annual Contribution + Employer Match
```

### Employer Match
```
Employer Match = min(Contribution%, 6%) × Salary
```

## Tips for Best Results

1. **Be Conservative**: Use moderate return rates (5-7%) for realistic projections
2. **Account for Inflation**: Consider 2-3% annual raises as baseline
3. **Max Out Match**: Always contribute enough to get full employer match (free money!)
4. **Increase Over Time**: Use sliders to see impact of raising contributions as salary grows
5. **Compare Scenarios**: Try different combinations to find your optimal strategy

## Limitations

- Does not account for:
  - Inflation adjustments
  - Tax implications
  - 401k contribution limits ($23,000 in 2024)
  - Catch-up contributions (age 50+)
  - Market volatility
  - Fee structures
  - Required minimum distributions (RMDs)

## Disclaimer

This calculator is for educational and planning purposes only. It provides estimates based on assumed consistent returns and does not guarantee future results. Actual investment returns vary and can be negative. Consult with a qualified financial advisor for personalized retirement planning advice.

## Support

For issues or questions, this is a standalone tool with no formal support. The code is straightforward and can be modified to suit your specific needs.

## Version History

**v1.0** - Initial release
- Basic calculator with age, salary, and contribution inputs
- 5% fixed ROI
- Simple totals display

**v2.0** - Enhanced features
- Added current balance input
- Adjustable annual raise slider
- Improved visual design
- Real-time chart updates

## License

Free to use and modify for personal or commercial purposes.

---

Created with Chart.js | No backend required | Works offline
