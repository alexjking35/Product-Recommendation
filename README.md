# Product-Recommendation
Finding association rules with highest confidence given previous item browsing history.  

Product Recommendations: The action or practice of selling additional products or services to
existing customers is called cross-selling. Giving product recommendation is one of the
examples of cross-selling that are frequently used by online retailers. One simple method to
give product recommendations is to recommend products that are frequently browsed
together by the customers.  
Suppose we want to recommend new products to the customer based on the products they
have already browsed on the online website. Write a program using the A-priori algorithm to
find products which are frequently browsed together. Fix the support to s = 100 (i.e. product
pairs need to occur together at least 100 times to be considered frequent) and find itemsets of
size 2 and 3.  
Use the provided browsing behavior dataset browsing.txt. Each line represents a browsing
session of a customer. On each line, each string of 8 characters represents the id of an item
browsed during that session. The items are separated by spaces.  

Identify pairs of items (X, Y) such that the support of {X, Y} is at least 100. For all such pairs,
compute the confidence scores of the corresponding association rules: X ⇒ Y, Y ⇒ X. Sort the
rules in decreasing order of confidence scores and list the top 5 rules in the writeup. Break ties,
if any, by lexicographically increasing order on the left hand side of the rule.  

Top 5 pairs by confidence scores   
((A→B)  is ((A,B),Confidence score)    
(('DAI93865', 'FRO40251'), 1.0)  
(('GRO85051', 'FRO40251'), 0.999176276771005)  
(('GRO38636', 'FRO40251'), 0.9906542056074766)  
(('ELE12951', 'FRO40251'), 0.9905660377358491)  
(('DAI88079', 'FRO40251'), 0.9867256637168141)  

Identify item triples (X, Y, Z) such that the support of {X, Y, Z} is at least 100. For all such triples,
compute the confidence scores of the corresponding association rules: (X, Y) ⇒ Z, (X, Z) ⇒ Y,
and (Y, Z) ⇒ X. Sort the rules in decreasing order of confidence scores and list the top 5 rules in
the writeup. Order the left-hand-side pair lexicographically and break ties, if any, by
lexicographical order of the first then the second item in the pair.  

Top 5 triples by confidence scores  
((A,B→C)  is (((A,B),C),Confidence score)  
(('DAI23334', 'ELE92920), 'DAI62779'), 1.0)  
(('DAI31081', 'GRO85051), 'FRO40251'), 1.0)  
(('DAI55911', 'GRO85051), 'FRO40251'), 1.0)  
(('DAI62779', 'DAI88079), 'FRO40251'), 1.0)  
(('DAI75645', 'GRO85051), 'FRO40251'), 1.0)  


