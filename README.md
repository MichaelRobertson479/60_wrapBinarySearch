# implement List.indexOf

2.	y = log2(x)
	means
	2^y = x

	The graph looks like 2^x, but reflected across y=x.

3.	Given a list and a element
	Return any index of that element in the list
	Or -1 if the element isn't in the list

	Repeat the instructions
	For the list from index 0 to the-one-we-checked minus 1
	Or the list from index the-one-we-checked plus 1 to the end
	Depending on the comparison

	Conditionals: if (low > high)
		      if (comparison == 0)

	Base Cases: return -1;
		    return mid;

	Recursive Case:

		Leftover Processing: comparison = list.get(mid).compareTo(find);

		Combining: if statements for comparison

		Recursive Abstraction:	
			return brec(list,find,mid+1,high);
      			return brec(list,find,low,mid-1);


`while`-style and recursive implementations at the top of
OrderedList_inArraySlots.java

[Java API on the `indexOf` method](https://docs.oracle.com/javase/10/docs/api/java/util/List.html#indexOf(java.lang.Object))

based on [solutionsHolmes/5D_genericTypes/OrderedList_inArraySlots_v2/](https://github.com/stuyvesant-cs/solutionsHolmes/tree/master/5D_genericTypes/OrderedList_inArraySlots_v2)
as of 2019-04-10 04:48
