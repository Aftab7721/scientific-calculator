# Scientific Calculator

A professional, feature-rich scientific calculator web application built with React. This calculator provides advanced mathematical operations, intuitive user interface, and comprehensive functionality comparable to commercial scientific calculators.

## Features

### Core Functionality
- **Basic Operations**: Addition, subtraction, multiplication, division
- **Scientific Functions**: Trigonometric, logarithmic, exponential, and root functions
- **Advanced Features**: Memory operations, calculation history, keyboard support
- **Professional UI**: Modern dark theme with smooth animations and responsive design

### Mathematical Operations

#### Basic Arithmetic
- Addition (+), Subtraction (-), Multiplication (×), Division (÷)
- Percentage calculations (%)
- Sign change (±)
- Decimal point handling with precision

#### Scientific Functions
- **Trigonometric**: sin, cos, tan, asin, acos, atan
- **Logarithmic**: log (base 10), ln (natural log)
- **Exponential**: e^x, 10^x, x^y (power function)
- **Root Functions**: √x (square root), ∛x (cube root), x^(1/y) (nth root)
- **Other**: x! (factorial), |x| (absolute value), x², x³

#### Mathematical Constants
- π (pi) - 3.14159...
- e (Euler's number) - 2.71828...

### Advanced Features

#### Memory Operations
- **MC** (Memory Clear): Clear memory
- **MR** (Memory Recall): Recall value from memory
- **MS** (Memory Store): Store current result in memory
- **M+** (Memory Add): Add current result to memory
- **M-** (Memory Subtract): Subtract current result from memory

#### Angle Mode
- **DEG/RAD Toggle**: Switch between degrees and radians for trigonometric functions
- Clear visual indication of current mode

#### Expression History
- Stores last 15 calculations
- Click on any history item to reuse the expression
- Collapsible history panel to save space

#### Keyboard Support
- **Numbers (0-9)**: Direct number input
- **Basic Operations (+, -, *, /)**: Arithmetic operations
- **Enter/Return**: Calculate result (equals)
- **Escape**: Clear all
- **Backspace**: Delete last character
- **Parentheses ( )**: Grouping operations
- **Function Shortcuts**:
  - `s` → sin
  - `c` → cos
  - `t` → tan
  - `l` → log
  - `n` → ln
  - `r` → √ (square root)
  - `p` → π (pi)

### User Interface

#### Design Features
- **Modern Dark Theme**: Professional appearance with gradient background
- **Color-Coded Buttons**: Different colors for numbers, operations, functions, and memory
- **Responsive Design**: Adapts to mobile, tablet, and desktop screens
- **Smooth Animations**: Button press effects and hover states
- **Visual Feedback**: Active state indicators and status displays

#### Display
- **Expression Line**: Shows current mathematical expression
- **Result Line**: Large, clear result display
- **Status Indicators**: Shows angle mode (DEG/RAD) and memory status (M)
- **Error Handling**: Clear error messages for invalid operations

## Usage Examples

### Basic Calculations
```
15 + 25 × 3 = 90
(5 + 3) × 2 = 16
100 ÷ 4 = 25
```

### Scientific Functions
```
sin(30°) = 0.5
cos(π) = -1
log(100) = 2
ln(e) = 1
√(144) = 12
5! = 120
```

### Complex Expressions
```
sin(π/2) + cos(0) × log(10) = 3
((2 + 3) × 4) - (10 ÷ 2) = 15
2^3 + √(16) = 12
```

### Memory Operations
```
25 [MS] → Store 25 in memory
15 [M+] → Add 15 to memory (now 40)
[MR] → Recall 40 from memory
```

## Error Handling

The calculator handles various error conditions gracefully:

- **Division by Zero**: "Cannot divide by zero"
- **Invalid Square Root**: "Invalid input for square root" (for negative numbers)
- **Invalid Logarithm**: "Invalid input for logarithm" (for zero or negative numbers)
- **Invalid Trigonometric Input**: Domain errors for inverse functions
- **Factorial Limits**: Prevents calculation of factorial for very large numbers
- **Overflow/Underflow**: Automatic scientific notation for very large/small numbers

## Technical Implementation

### Architecture
- **React Functional Components**: Modern React with hooks
- **State Management**: useState and useCallback for optimal performance
- **Mathematical Engine**: Custom expression parser with shunting yard algorithm
- **Precision Handling**: Floating-point precision management to avoid JavaScript math errors

### Mathematical Parser
- **Order of Operations**: Proper PEMDAS/BODMAS implementation
- **Function Precedence**: Correct handling of mathematical function precedence
- **Implicit Multiplication**: Smart handling of expressions like "2π" or "3(4+5)"
- **Parentheses Support**: Nested parentheses with proper evaluation

### Performance Optimizations
- **React.memo**: Prevents unnecessary re-renders
- **useMemo**: Optimizes expensive calculations
- **Debounced Input**: Efficient handling of rapid button presses
- **Minimal Bundle**: Uses CDN React for smaller initial load

## Browser Compatibility

- **Modern Browsers**: Chrome, Firefox, Safari, Edge (latest versions)
- **Mobile Support**: iOS Safari, Chrome Mobile, Samsung Internet
- **Features Used**: ES6+, CSS Grid, Flexbox, CSS Custom Properties

## Installation & Usage

1. **Download**: Save the `index.html` file to your computer
2. **Open**: Double-click the file or open it in any modern web browser
3. **Use**: Start calculating immediately - no installation required!

### Local Development
```bash
# Simply open the HTML file in a browser
# No build process or dependencies required
```

## File Structure
```
scientific-calculator/
├── index.html          # Complete calculator application
└── README.md           # This documentation file
```

## Features Comparison

| Feature | Basic Calculator | This Scientific Calculator |
|---------|------------------|---------------------------|
| Basic Arithmetic | ✅ | ✅ |
| Scientific Functions | ❌ | ✅ |
| Memory Operations | ❌ | ✅ |
| History | ❌ | ✅ |
| Keyboard Support | ❌ | ✅ |
| Angle Modes | ❌ | ✅ |
| Error Handling | Basic | Comprehensive |
| Responsive Design | ❌ | ✅ |
| Professional UI | ❌ | ✅ |

## Future Enhancements

Potential features for future versions:
- **Unit Converter**: Length, weight, temperature conversions
- **Graphing**: Simple function plotting capability
- **Themes**: Light/dark mode toggle
- **Export/Import**: Save and load calculation history
- **Scientific Notation Input**: Direct scientific notation entry
- **Custom Functions**: User-defined mathematical functions

## License

This project is open source and available under the MIT License.

## Support

For issues, questions, or feature requests, please refer to the keyboard shortcuts guide built into the calculator interface.

---

**Built with ❤️ using React, modern CSS, and advanced mathematical algorithms.**
