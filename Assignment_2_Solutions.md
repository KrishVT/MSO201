# Q1  
B = A ∪ (B-A)  
Now as A and B-A are disjoint  
P(B) = P(A) + P(B-A)  
P(B-A) >= 0  
P(B) >= P(A)  
# Q2  
A ∪ B = (A-B) ∪ (B-A) ∪ (A ∩ B)  
As all the sets on the right hand side of the above equation are mutually disjoint  
P(A ∪ B) = P(A-B) + P(B-A) + P(A ∩ B) ---(1)   
A = (A-B) ∪ (A ∩ B)  
As (A-B) and (A ∩ B) are disjoint  
P(A) = P(A-B) + P(A ∩ B)  
P(A-B) = P(A) - P(A ∩ B) ---(2)  
Similarily, P(B-A) = P(B) - P(A ∩ B) ---(3)  
Using (2) and (3) in (1)  
P(A ∪ B) = P(A) + P(B) - P(A ∩ B)  
# Q3  
Let B ∪ C = M  
Now from Q2 we have P(A ∪ M) = P(A) + P(M) - P(A ∩ M)  
P(A ∪ B ∪ C) = P(A) + P(B ∪ C) - P(A ∩ (B ∪ C))  
P(A ∪ B ∪ C) = P(A) + P(B ∪ C) - P((A ∩ B) ∪ (A ∩ C)) ---(1)  
Now again using Q2 we have, P((A ∩ B) ∪ (A ∩ C)) = P(A ∩ B) + P(A ∩ C) - P((A ∩ B) ∩ (A ∩ C))    
The above equation is same as P((A ∩ B) ∪ (A ∩ C)) = P(A ∩ B) + P(A ∩ C) - P(A ∩ B ∩ C) ---(2)  
Now once again from Q2 we have P(B ∪ C) = P(B) + P(C) - P(B ∩ C) ---(3)  
Now using (2) and (3) in (1) we have  
P(A ∪ B ∪ C) = P(A) + P(B) + P(C) - P(B ∩ C) - P(A ∩ B) - P(A ∩ C) + P(A ∩ B ∩ C)  
# Q4  
I am going to use induction for this problem  
  
Base Case  
For n = 1 it is true as P(A1) = P(A1)  

Assumption  
A1 ⊂ A2 ⊂ A3 ..⊂An  
P(A1 ∪ A2 .... ∪ An) = P(An)  
  
Now Proving for (n+1)  
Let A1 ⊂ A2 ⊂ A3 ..⊂An = M  
As M ⊂ A(n+1)  
A(n+1) = M ∪ (A(n+1) - M) ---(1)  
P(M ∪ A(n+1)) = P(M ∪ M ∪ (A(n+1) - M))  
P(M ∪ A(n+1)) = P(M ∪ (A(n+1) - M))  
Now again using (1)  
P(M ∪ A(n+1)) = P(A(n+1))  
Hence Proved !!  
# Q5  
We can solve this using induction and it is very similar to Q4
