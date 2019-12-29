# Problem
We are interested in computing a linear optimal control law to stabilize the cart pole system when subjected to small
deviations from the rest position (when ![equation](https://latex.codecogs.com/svg.latex?x&space;=&space;0,&space;v&space;=&space;0,&space;\theta&space;=&space;\pi,&space;\omega&space;=&space;0))

<img src="https://danielpiedrahita.files.wordpress.com/2017/02/cart-pole.png" alt="drawing" width="400"/>

## The dynamic equations of the Cart-Pole model are written as

![equation](https://latex.codecogs.com/svg.latex?%5Cbegin%7Barray%7D%7Brcl%7D%20%5Cdot%7Bx%7D%20%26%3D%26%20v%20%5C%5C%20%5Cdot%7Bv%7D%20%26%3D%26%20%5Cfrac%7Bf%20&plus;%20m_p%20%5Csin%5Ctheta%20%28l%20%5Comega%5E2%20&plus;%20g%20%5Ccos%20%5Ctheta%29%7D%7Bm_c%20&plus;%20m_p%20%5Csin%5E2%20%5Ctheta%7D%20%5C%5C%20%5Cdot%7B%5Ctheta%7D%20%26%3D%26%20%5Comega%5C%5C%20%5Cdot%7B%5Comega%7D%20%26%3D%26%20%5Cfrac%7B-f%5Ccos%5Ctheta%20-m_p%20l%20%5Comega%5E2%20%5Ccos%5Ctheta%5Csin%5Ctheta%20-%20%28m_c%20&plus;%20m_p%29g%20%5Csin%5Ctheta%7D%7Bl%28m_c%20&plus;%20m_p%20%5Csin%5E2%20%5Ctheta%29%7D%20%5Cend%7Barray%7D)

## which we discretize using a time step Δ𝑡

![equation](https://latex.codecogs.com/svg.latex?%24%24%20%5Cbegin%7Barray%7D%7Brcl%7D%20x_%7Bn&plus;1%7D%20%26%3D%26%20x_n%20&plus;%20%5CDelta%20t%5Ccdot%20v_n%20%5C%5C%20v_%7Bn&plus;1%7D%20%26%3D%26%20v_n%20&plus;%20%5CDelta%20t%20%5Ccdot%20%5Cleft%28%20%5Cfrac%7Bf_n%20&plus;%20m_p%20%5Csin%5Ctheta_n%20%28l%20%5Comega_n%5E2%20&plus;%20g%20%5Ccos%20%5Ctheta_n%29%7D%7Bm_c%20&plus;%20m_p%20%5Csin%5E2%20%5Ctheta_n%7D%20%5Cright%29%5C%5C%20%5Ctheta_%7Bn&plus;1%7D%20%26%3D%26%20%5Ctheta_n%20&plus;%20%5CDelta%20t%20%5Ccdot%20%5Comega_n%20%5C%5C%20%5Comega_%7Bn&plus;1%7D%20%26%3D%26%20%5Comega_n%20&plus;%20%5CDelta%20t%20%5Ccdot%20%5Cleft%28%20%5Cfrac%7B-f_n%5Ccos%5Ctheta_n%20-m_p%20l%20%5Comega_n%5E2%20%5Ccos%5Ctheta_n%5Csin%5Ctheta_n%20-%20%28m_c%20&plus;%20m_p%29g%20%5Csin%5Ctheta_n%7D%7Bl%28m_c%20&plus;%20m_p%20%5Csin%5E2%20%5Ctheta_n%29%7D%5Cright%29%20%5Cend%7Barray%7D%24%24)

## Result
![cart](Exercise 2/IP.gif)
