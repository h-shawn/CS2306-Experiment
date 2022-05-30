# experiment3

## For 8255 chip

Addr8 = 1
Addr7 = 0
Addr6 $\sim$ 4 = 000 $\sim$ 111 ($Y_{0}\sim Y_{7}$)
Addr3 $\sim$ 0 = 0000 $\sim$ 1111

Since 8255 is $Y_{2}$, its address range is 120H~127H. 
$$
\begin{array}{|c|c|c|c|c|}
        \hline \text { Register } & \text { $A_{1}$ } & \text { $A_{0}$ } & \text { Addr }(D_{0}\sim D_{7}) & \text { Addr }(D_{8}\sim D_{15})\\
        \hline \mathrm{PortA} & \mathrm{0} & \mathrm{0} & \mathrm{120H} & \mathrm{121H}\\
        \mathrm{PortB} & \mathrm{0} & \mathrm{1} & \mathrm{122H} & \mathrm{123H}\\
        \mathrm{PortC} & \mathrm{1} & \mathrm{0} & \mathrm{124H} & \mathrm{125H}\\
        \mathrm{CtrlPT} & \mathrm{1} & \mathrm{1} & \mathrm{126H} & \mathrm{127H}\\
\hline
\end{array}
$$

$$
\begin{array}{|c|c|}
        \hline \text { Register } & \text { Usage } \\
        \hline \mathrm{PA_{0}\sim PA_{3}} &  \text{control which digit to display}\\
        \mathrm{PA_{4}\sim PA_{7}} &  \text{control four LED lights }\\
        \mathrm{PB_{0}\sim PB_{7}} &  \text{control which number to display}\\
        \mathrm{PC_{0}\sim PC_{7}} &  \text{correspond to switches}\\
\hline
\end{array}
$$

## For 8253 chip

Since 8253 is $Y_{0}$, its address range is 100H~107H. 
$$
\begin{array}{|c|c|c|c|c|}
        \hline \text { Register } & \text { $A_{1}$ } & \text { $A_{0}$ } & \text { Addr }(D_{0}\sim D_{7}) & \text { Addr }(D_{8}\sim D_{15})\\
        \hline \mathrm{Timer0} & \mathrm{0} & \mathrm{0} & \mathrm{100H} & \mathrm{101H}\\
        \mathrm{Timer1} & \mathrm{0} & \mathrm{1} & \mathrm{102H} & \mathrm{103H}\\
        \mathrm{Timer2} & \mathrm{1} & \mathrm{0} & \mathrm{104H} & \mathrm{105H}\\
        \mathrm{CtrlRegister} & \mathrm{1} & \mathrm{1} & \mathrm{106H} & \mathrm{107H}\\
\hline
\end{array}
$$

