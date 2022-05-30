# experiment2

## For 62256 memory chips

Addr19 = 0
Addr18 $\sim$ 16 = 000 $\sim$ 111 ($Y_{0}\sim Y_{7}$)
Addr15 $\sim$ 0 = 0000H $\sim$ 1111H


$$
\begin{array}{|c|c|}
        \hline \text { Memory Chip } & \text { Address range } \\
        \hline Y_{0} & \mathrm{00000h}\sim\mathrm{0FFFFh} \\
        Y_{1} & \mathrm{10000h}\sim\mathrm{1FFFFh} \\
        Y_{2} & \mathrm{20000h}\sim\mathrm{2FFFFh} \\
        Y_{3} & \mathrm{30000h}\sim\mathrm{3FFFFh} \\
        Y_{4} & \mathrm{40000h}\sim\mathrm{4FFFFh} \\
        Y_{5} & \mathrm{50000h}\sim\mathrm{5FFFFh} \\
        Y_{6} & \mathrm{60000h}\sim\mathrm{6FFFFh} \\
        Y_{7} & \mathrm{70000h}\sim\mathrm{7FFFFh} \\
\hline
\end{array}
$$

If the address range of U10 and U11 starts from 80000h, we need to modify Addr19 to 1 and use $Y_{0}$.

## For four registers of 8255 chip

Addr7 = 1
Addr6 = 0
Addr5 $\sim$ 3 = 000 $\sim$ 111 ($Y_{0}\sim Y_{7}$)
Addr2 $\sim$ 0 = 000 $\sim$ 111

Since 8255 is $Y_{2}$, its address range is 90H~97H. 


$$
\begin{array}{|c|c|c|c|c|}
        \hline \text { Register } & \text { $A_{1}$ } & \text { $A_{0}$ } & \text { Addr }(D_{0}\sim D_{7}) & \text { Addr }(D_{8}\sim D_{15})\\
        \hline \mathrm{PortA} & \mathrm{0} & \mathrm{0} & \mathrm{90H} & \mathrm{91H}\\
        \mathrm{PortB} & \mathrm{0} & \mathrm{1} & \mathrm{92H} & \mathrm{93H}\\
        \mathrm{PortC} & \mathrm{1} & \mathrm{0} & \mathrm{94H} & \mathrm{95H}\\
        \mathrm{CtrlPT} & \mathrm{1} & \mathrm{1} & \mathrm{96H} & \mathrm{97H}\\
\hline
\end{array}
$$

## For PA, PB and PC ports


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

