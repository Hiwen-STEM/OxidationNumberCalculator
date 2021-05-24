# Oxidation Number Calculator - Beta Version - (Still Needs Optimizing and Bug Removal): The oxidation number Calculator takes in a chemical equation
or individual compound and returns the oxidation numbers of each element involved (in the case of a chemical equation, several lists of oxidation numbers
for each compound will be returned). This module has yet to be fully optimized and cleaned of potential bugs; more testing is to come in the following
week along with updates.

#Overview
Documentation for the Oxidation Number Calculator:

# 1. Core Functions:

  How to use: <br/>
      from OxidationNumberCalculator import processI

  ## def processI(StringI, Peroxide)
      +For individual elements, it returns the original string input (StringI) and a list of corresponding oxidation numbers...
      	   +StringI: A compound (DON'T INCLUDE PARENTHESES) or chemical equation (WITH NO SPACES): Cu+NO3[-1]->Cu[+2]+NO
	   	   +Peroxide is an index value that indicates a compound is a peroxide or an element/compound within an equation is a peroxide...
	   	     	       +Let peroxide = 0 for any peroxide compounds give; Let peroxide = COMPOUND_POSITION of equation...
		     	       	    	     +For instance, if StringI = H2O2, let peroxide = 0...
			  		     +For instance, if StringI = H2+O2->H2O2, let peroxide = 2 (index value of the third element/compound in the equation)
	   +When inputting a chemical equation, the original input will be returned along with four separate dictionaries that are one of two types...
	   	     +The first type consists of lists of elements that are accessible via compound name...
		     +The second type consists of lists of oxidation numbers that are accessible via compound name...