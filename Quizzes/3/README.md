1) the * operator is a cross product while the .* is a dot product  ex:>> [2,5,3;4,8,6;6,9,2]*[4,6,2;5,6,2;8,4,3]

ans =

    57    54    23
   104    96    42
    85    98    36

>> [2,5,3;4,8,6;6,9,2].*[4,6,2;5,6,2;8,4,3]

ans =

     8    30     6
    20    48    12
    48    36     6
    
    
2) A.*B

3A)
inputstr(s)= input ('enter a string: ');
function BoolAns= testStrings(s)
    if (testStrings(s)=='MATLAB')
        BoolAns='true';
    else
        BoolAns='false';
    end
    disp BoolAns;
end

3B)the == operator will check if 2 values are exuivalent, while the .equals() will check 2 strings directly against each other.

4)the two OR operators | and || are different because || is an exclusive OR which is more efficient in coding.
example - say we have 2 values, true and false, the | will check both values- true|false even though it did not need to check 
the second value. the || would stop after finding true in  true||false.

5) x=(a/b)<10  -- because x results in a true or flase value (0 or 1) and (a/b)=infinity falsifying the statement by saying 
infinity is less than 10 will result in false (aka x=0)

6) the struture array is more efficient... instead of having to call AOS(1).grade + AOS(2).grade+... and dividing by the total
we can loop through all of the students in the structure array adding their grades and dividing by the total number of students 
in order to find the average. Besides this, 10000 students would become way too many lines of code without using a structure 
array

7)
function [x1,x2]=getRoot(a,b,c)
x1=((-b+sqrt((b^2)-(4*a*c)))/(2*a))
x2=((-b-sqrt((b^2)-(4*a*c)))/(2*a))
end

8)function[f]=int(a,b,c)
f=integral(x.^2+c.*x+1, a,b);
end

9)
function [factorial]=getFac(n)
total=0;
for i=1:n-1
    a=(i*(i+1));
    total=total+a;
end
factorial=total;
end

