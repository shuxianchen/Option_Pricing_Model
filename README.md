# Option Pricing Model
This is a model that calculates option values by using the Black-Scholes formulas and binomial pricing model.

If you have basic understanding of options, using the calculator should be very simple. It does not require any particular Excel skills, other that entering values in cells and selecting items in dropdown boxes.

### Supported Options
   - European calls and puts
   - American calls and puts
   - Compound calls and puts
   - Chooser options
### Workbook Structure
There are ten sheets: 			

Yellow tabs are the user interfaces, where you enter inputs, view results, and compare differences.
- Standard Option: calculate standard european option price using either black scholes or binomial prcing up to 100 steps. 					
- Exotic Option: calculate standard compoun option and chooser option price using binomial prcing up to 100 steps.	
  

Blue tabs are the internal implementation of the binomial pricing model.			
- Stock Price: is the underlying pricing tree. Each step is in one column. Moving horizontally from left to right, underlying price goes up; moving diagonally    one cell to the right and one cell down, underlying price goes down.					
- Option Price: is the option pricing tree.The last step shows option payoff at expiration for different levels of underlying price (the price in the same cell in StockPrice sheet).Step zero (cell B2 in Option Price) is the calculated current option price.	
  
### Example Usage							
- Pick either standard option or exotic option workbook.   						

- Enter all the paramaters required in the input table as shown below. Yellow cells are for inputs. Overwrite the values in yellow cells to change inputs or preference.

  ![example_input](https://github.com/shuxianchen/Option_Pricing_Model/blob/main/Supporting%20Files/example_input.jpg)

- The option price and greeks will be reflected instantly in the output table. Do not change any cells in output or intermediate table. They usually contain formulas and that value will be changed by the calculator,not the user.
 
  ![example_output](https://github.com/shuxianchen/Option_Pricing_Model/blob/main/Supporting%20Files/example_output.jpg)
 
- Click on the corresponding blue tab to see bionimal lattic for underlying stock pirce and option price.

### Excel Techniques I Used
 - Complex logic in formulas to implement binomial pricing model.
 - Separating of input, calculation, and output during model design for clear and maintainable spreadsheet.
 - Naming cells and ranges to make formulas more readable and less error-prone.
 - Data validation,such as creating drop-down lists, to restrict the type of data that users enter into a cell.						
