# Matlab Note
### create matrix
A = [1 2 3 ; 4 5 6]
A =

     1     2     3
     4     5     6
### concat matrix
B = [ones(2,1),A]
B =

     1     1     2     3
     1     4     5     6
C = [ones(1,2);A]
C =

     1     1
     0     0
     0     0
     0     0
### take part of matrix
D = B(:,2:end)
D =

     1     2     3
     4     5     6

### Specialized Matrix Functions
A = zeros(3,2)
A =

     0     0
     0     0
     0     0

B = ones(2,4)
B =

     1     1     1     1
     1     1     1     1

I = eye(4)
I =

     1     0     0     0
     0     1     0     0
     0     0     1     0
     0     0     0     1

#### turn numbered label into vectorized label
Y = eye(K)(y, :)      
% K- label_nums y-label vector
