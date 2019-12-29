# Problem
We are interested in computing a linear optimal control law to stabilize the cart pole system when subjected to small
deviations from the rest position (when ![equation](https://latex.codecogs.com/svg.latex?x&space;=&space;0,&space;v&space;=&space;0,&space;\theta&space;=&space;\pi,&space;\omega&space;=&space;0))

<img src="https://danielpiedrahita.files.wordpress.com/2017/02/cart-pole.png" alt="drawing" width="400"/>

## The dynamic equations of the Cart-Pole model are written as

![equation](https://latex.codecogs.com/svg.latex?\begin{array}{rcl}&space;\dot{x}&space;&=&&space;v&space;\\&space;\dot{v}&space;&=&&space;\frac{f&space;&plus;&space;m_p&space;\sin\theta&space;(l&space;\omega^2&space;&plus;&space;g&space;\cos&space;\theta)}{m_c&space;&plus;&space;m_p&space;\sin^2&space;\theta}&space;\\&space;\dot{\theta}&space;&=&&space;\omega\\&space;\dot{\omega}&space;&=&&space;\frac{-f\cos\theta&space;-m_p&space;l&space;\omega^2&space;\cos\theta\sin\theta&space;-&space;(m_c&space;&plus;&space;m_p)g&space;\sin\theta}{l(m_c&space;&plus;&space;m_p&space;\sin^2&space;\theta)}&space;\end{array})
