# AIM:
To implement error control coding schemes with linear block codes using MATLAB.

# SOFTWARE REQUIRED: 
  MATLAB

# PROGRAM:
# ERROR CODING
# ENCODING:
clc;
close all;
n = 7;
k = 4;
msg = [1 0 0 1;
       1 0 1 0;
       1 0 1 1];
code = encode(msg, n, k, 'cyclic');
msg
code
# ENCODING OUTPUT:
<img width="432" height="346" alt="Screenshot 2026-08-27 133457" src="https://github.com/user-attachments/assets/a87282df-03ba-474d-af40-3526ade52646" />


# DECODING PROGRAM:
clc;

clear all;

close all;

q = 3;

n = 2^q - 1;
k = n - q;

parmat = hammgen(q);
trt = syndtable(parmat);

recd = [1 0 1 1 1 1 0];

syndrome = rem(recd * parmat', 2);
syndrome_de = bi2de(syndrome, 'left-msb');

disp(['syndrome = ', num2str(syndrome_de), ' (decimal) ', ...
      num2str(syndrome), ' (binary)']);

corrvect = trt(1 + syndrome_de, :);

correctedcode = rem(corrvect + recd, 2);

parmat
corrvect
correctedcode

# DECODING OUTPUT:
<img width="437" height="257" alt="Screenshot 2026-08-27 143558" src="https://github.com/user-attachments/assets/1977c083-8389-4ffb-9132-e03389bb12ea" />


# RESULT:
Thus encoding and decoding of block codes are performed using MATLAB.

