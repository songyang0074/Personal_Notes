# Personal_Notes
记录一些个人的笔记，便于随时察看，主要是Markdown笔记
###谐振控制器的传递函数：
$$
H(s)=\frac{2K_r \omega_cs}{s^2 + 2\omega_cs + \omega_0^2}
$$

使用双线性变换，进行离散化处理
$$
H(z) = \frac{A_0+A_1z^{-1}+A_2z^{-2}}{1+B_1z^{-1}+B_2z^{-2}} = \frac{A_0z^2+A_1z+A_2z}{z^2+B_1z+B_2}
$$

$$
\begin{array}{l}
C = 2 / T \\ \\
R = \omega_0^2 + 2\omega_cC + C^2
\end{array}
$$

分子系数
$$ \begin{array}{l}
A_0 = \frac{2K_i\omega_cC}{R}\\ \\
A_1 = 0 \\ \\
A_2 = -A_0
\end{array} $$

分母系数
$$ \begin{array}{l}
B_0 = 1 \\ \\
B_1 = \frac {2\omega_0^2 - 2C^2} {R} \\
\\
B_2 = \frac {\omega_0^2 - 2\omega_cC + C^2} {R} 
\end{array} $$

带通滤波器就是把$K_r$设为1

###低通滤波器传递函数：
$$
H(s)=\frac{\omega_0^2}{s^2 + 2\zeta\omega_0s + \omega_0^2}
$$

使用双线性变换，进行离散化处理
$$
H(z) = \frac{A_0+A_1z^{-1}+A_2z^{-2}}{1+B_1z^{-1}+B_2z^{-2}} = \frac{A_0z^2+A_1z^+A_2z}{z^2+B_1z+B_2}
$$

$$
\begin{array}{l}
C = 2 / T \\ \\
R = \omega_0^2 + 2\zeta\omega_0C + C^2
\end{array}
$$

分子系数
$$ \begin{array}{l}
A_0 = \frac{\omega_0^2}{R}\\ \\
A_1 = \frac{2\omega_0^2}{R} \\ \\
A_2 = \frac{\omega_0^2}{R}
\end{array} $$

分母系数
$$ \begin{array}{l}
B_0 = 1 \\ \\
B_1 = \frac {2\omega_0^2 - 2C^2} {R} \\
\\
B_2 = \frac{\omega_0^2 - 2\zeta\omega_0C + C^2}{R}
\end{array} $$

###高通滤波器传递函数：
$$
H(s)=\frac{s^2}{s^2 + 2\zeta\omega_0s + \omega_0^2}
$$

使用双线性变换，进行离散化处理
$$
H(z) = \frac{A_0+A_1z^{-1}+A_2z^{-2}}{1+B_1z^{-1}+B_2z^{-2}} = \frac{A_0z^2+A_1z^+A_2z}{z^2+B_1z+B_2}
$$

$$
\begin{array}{l}
C = 2 / T \\ \\
R = \omega_0^2 + 2\zeta\omega_0C + C^2
\end{array}
$$

分子系数
$$ \begin{array}{l}
A_0 = \frac{C^2}{R}\\ \\
A_1 = \frac{-2C^2}{R} \\ \\
A_2 = \frac{C^2}{R}
\end{array} $$

分母系数
$$ \begin{array}{l}
B_0 = 1 \\ \\
B_1 = \frac {2\omega_0^2 - 2C^2} {R} \\
\\
B_2 = \frac{\omega_0^2 - 2\zeta\omega_0C + C^2}{R}
\end{array} $$
###带阻滤波器传递函数：
$$
H(s)=\frac{s^2+\omega_0^2}{s^2 + 2\zeta\omega_0s + \omega_0^2}
$$

使用双线性变换，进行离散化处理
$$
H(z) = \frac{A_0+A_1z^{-1}+A_2z^{-2}}{1+B_1z^{-1}+B_2z^{-2}} = \frac{A_0z^2+A_1z^+A_2z}{z^2+B_1z+B_2}
$$

$$
\begin{array}{l}
C = 2 / T \\ \\
R = \omega_0^2 + 2\zeta\omega_0C + C^2
\end{array}
$$

分子系数
$$ \begin{array}{l}
A_0 = \frac{\omega_0^2 + C^2}{R}\\ \\
A_1 = \frac{2\omega_0^2 - 2C^2}{R} \\ \\
A_2 = \frac{\omega_0^2 + C^2}{R}
\end{array} $$

分母系数
$$ \begin{array}{l}
B_0 = 1 \\ \\
B_1 = \frac {2\omega_0^2 - 2C^2} {R} \\
\\
B_2 = \frac{\omega_0^2 - 2\zeta\omega_0C + C^2}{R}
\end{array} $$
