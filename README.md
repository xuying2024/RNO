# RNO

Below are some qualitative samples from testing. Notice that RNO prediction has smaller magnitude than $\delta u$, indicating RNO have learned and reduced the difference between GT query $u_q$ and pushforward of reference $u_r$.  

Figure 1. Results and visualization of Airfoil-Euler. The deformation for this dataset is easy to get since there is a 1-on-1 mapping of mesh grids between cases. The result is updated to
|    Model    |  l2 Error   |
| ----------- | ----------- |
|    CORAL    |    0.081    |
|    NU-FNO   |    0.147    |   
|   Geo-FNO   |    0.079    | 
|    GNOT     |   *0.04*    |
|  RNO (Ours) |  **0.034**  | 

![fig1](./fig/airfoil2d_euler_y_component_0.png)
![fig1.1](./fig/Airfoil-euler-phi.png)

Figure 2. Results and visualization of Airfoil-RANS, turbulent viscosity $\mu_t$, and an example of constructing deformation $\varphi$ with irregular mesh.
|    Model    |     $u$     |     $v$     |     $p$     |   $\mu_t$   |
| ----------- | ----------- | ----------- | ----------- | ----------- |
|     GNOT    |   0.51      |    0.44     |    0.61     |    0.31     |
|    R-GNOT   |  **0.3**    |  **0.19**   |   *0.11*    |  **0.19**   |
|  RNO (Ours) |   *0.32*    |   *0.32*    |  **0.096**  |   *0.22*    |

![fig2](./fig/airfoil2d_rans_y_component_3.png)
![fig2.1](./fig/Airfoil-RANS-phi.png)

Figure 3. Visualization of NS2d-circle, pressure $p$. 
![fig3](./fig/ns2d_y_component_2.png)

Figure 4. Visualization of NS2d-square, velocity component $v$. 
![fig4](./fig/ns2dsq_y_component_1.png)