---
ID: 334
post_title: Test Latex Support
author: admin
post_excerpt: ""
layout: post
permalink: http://en.mekesim.com/article/334
published: true
post_date: 2016-08-16 13:40:03
---
\section{Bar-Cohen and Rohsennow Solution}

Finned surfaces of various shapes, called heat sinks, are frequently used in the cooling of electronic devices. Energy dissipated by these devices is transferred to the heat sinks by conduction and from the heat sinks to the ambient air by natural or forced convection, depending on the power dissipation requirements. Natural convection is the preferred mode of heat transfer since it involves no moving parts, like the electronic components themselves. However, in the natural convection mode, the components are more likely to run at a higher temperature and thus undermine reliability. A properly selected heat sink may considerably lower the operation temperature of the components and thus reduce the risk of failure.

Natural convection from vertical finned surfaces of rectangular shape has been the subject of numerous studies, mostly experimental. 

\begin{figure}[htp]	
	\centering
	\includegraphics[width=3cm]{flow.eps}
	\caption{Natural convection flow through a channel between two isothermal vertical plates.}
	\label{flow}
\end{figure}

Natural convection flow through a channel formed by two parallel plates as shown in Fig \ref{flow} is commonly encountered in practice. When the plates are hot ($T_s > T_{\infty}$), the ambient fluid at $T_{\infty}$ enters the channel from the lower end, rises as it is heated under the effect of buoyancy, and the heated fluid leaves the channel from the upper end. The plates can be approximated as being isothermal ($T_s = constant$) in this case.

Boundary layers start to develop at the lower ends of opposing surfaces, and eventually merge at the midplane if the plates are vertical and sufficiently long. In this case, we will have fully developed channel flow after the merger of the boundary layers, and the natural convection flow is analyzed as channel flow. But when the plates are short or the spacing is large, the boundary layers of opposing surfaces never reach each other, and the natural convection flow on a surface is not affected by the presence of the opposing surface. In that case, the problem should be analyzed as natural convection from two in- dependent plates in a quiescent medium, using the relations given for surfaces, rather than natural convection flow through a channel.

\begin{figure}[htp]	
	\centering
	\includegraphics[width=4cm]{fin.eps}
	\caption{Various dimensions of a finned surface	oriented vertically.}
	\label{fin}
\end{figure}
\subsection{Heat Flow Transfer by Fin}
Bar-Cohen and Rohsenow (1984) \cite{Bar} have compiled the available data under various boundary conditions, and developed correlations for the Nusselt number and optimum spacing. The characteristic length for vertical parallel plates used as fins is usually taken to be the spacing between adjacent fins $S$, although the fin height $L$ could also be used. The Rayleigh number is expressed as

\begin{equation}\label{eq:ra}
Ra_S=\dfrac{g\beta (T_S-T_{\infty})S^3}{\nu^2}Pr
\end{equation}

\begin{equation}\label{eq:nu}
Nu=\left[ \dfrac{576}{(Ra_SS/L)^2}+\dfrac{2.873}{(Ra_SS/L)^{0.5}}\right] ^{-0.5}
\end{equation}

\begin{equation}\label{eq:h}
h=Nuk/S
\end{equation}

\begin{equation}\label{eq:q}
\dot{Q}=hA(T_s-T_{\infty})
\end{equation}
\subsection{Optimum Fin Spacing}
A question that often arises in the selection of a heat sink is whether to select one with closely packed fins or widely spaced fins for a given base area. A heat sink with closely packed fins will have greater surface area for heat transfer but a smaller heat transfer coefficient because of the extra resistance the additional fins introduce to fluid flow through the interfin passages. A heat sink with widely spaced fins, on the other hand, will have a higher heat transfer coefficient but a smaller surface area. Therefore, there must be an optimum spacing that maximizes the natural convection heat transfer from the heat sink for a given base area $WL$, where $W$ and $L$ are the width and height of the base of the heat sink, respectively, as shown in Fig. \ref{fin}. When the fins are essentially isothermal and the fin thickness t is small relative to the fin spacing S, the optimum fin spacing for a vertical heat sink is determined by Bar-Cohen and Rohsenow to be

\begin{equation}\label{eq:optS}
S_{opt}=2.714\frac{L}{Ra_L^{0.25}}
\end{equation}

\begin{equation}\label{key}
Ra_L=\dfrac{g\beta(T_s-T_{\infty})L^3}{\nu^2}Pr
\end{equation}

It can be shown by combining the three equations above that when $S = S_{opt}$, the Nusselt number is a constant and its value is 1.307,
\begin{equation}
Nu=\dfrac{hS_{opt}}{k}=1.307
\end{equation}

\section{Discussion}
if fin distance is very big, that analysis as two independent plate:

\begin{equation}\label{key}
Nu=\left[ 0.825+\dfrac{0.387Ra_L^{1/6}}{[1+(0.492/Pr)^{9/16}]^{8/27}}\right]^2
\end{equation}

\begin{figure}[htp]	
	\centering
	\includegraphics[width=10cm]{compare.eps}
	\caption{Calculation Result compare}
\end{figure}

that shows when space become bigger, Bar-Cohen provide equation result will same as signal plate result. And it has max point.

I use matlab to solve the max flow rate will space change, the result not matched author provided equation \ref{eq:optS} result. use equation \ref{eq:optS} the fin space is
\begin{lstlisting}
Sopt = 9.5070
Nopt = 24.7467
Nuopt = 1.7343
\end{lstlisting}
Noticed the Nu is 1.7343, which not same as it said equal to a fix number 1.307.

But solve equations \ref{eq:ra} - \ref{eq:q} results is
\begin{lstlisting}
Sopt = 10.2079
Nopt = 23.4866
Nuopt = 1.2194
\end{lstlisting}

The optimum of fin space has some error of the original text book, that may cause it calculate the fin number as below:
\begin{equation}\label{key}
N=W/(S+t)\simeq W/S
\end{equation}

But the fin number should be calculate as
\begin{equation}\label{key}
N=(W-t)/(S+t)+1
\end{equation}

\begin{figure}[htp]	
	\centering
	\includegraphics[width=10cm]{Nu.eps}
	\caption{Nu number change with length with two calculation methods}
\end{figure}

Below Matlab code calculate the heat flow with given parameters.

% ----------------------------------------------------------------
\begin{lstlisting}
%Cal Heat Sink Heat Flow
%please input setting parameters:
Ts=87;
Ta=45;
W=300;
L=330;
H=39.6;
N=21;
t=3;
% Air parameters, change them as need.
Pr=0.7177;
nu=0.00001995;
g=9.81;
k=0.02881;

%%The setting fin space is
S=(W-t)/(N-1)-t
A=H*L*2*N*1E-6;
beta=1/((Ts+Ta)/2+273);


%Ra number and Nu number
Ras=g*beta*(Ts-Ta)*(S/1000)^3/nu^2*Pr
RaL=g*beta*(Ts-Ta)*(L/1000)^3/nu^2*Pr
Nu_p=(576/(Ras*S/L)^2+2.873/(Ras*S/L)^0.5)^(-0.5)%Parallel Wall
Nu_s=(0.825+0.387*RaL^(1/6)/(1+(0.492/0.7202)^(9/16))^(8/27))^2%Signal Wall
%Heat transfer coff is

h_p=Nu_p*k/S*1000
h_s=k*Nu_s/L*1000

Q_p=h_p*A*(Ts-Ta)
Q_s=h_s*A*(Ts-Ta)

%Optimized fin space
Sopt=2.714*L/RaL^0.25
Nopt=(W-t)/(t+Sopt)+1
Nuopt=(576/(Ras*Sopt/L)^2+2.873/(Ras*Sopt/L)^0.5)^(-0.5)
\end{lstlisting}

\begin{thebibliography}{99}
	
	\bibliographystyle{amsplain}
	% 英文学术期刊中的文章
	%\bibitem{paper:english} A. Charnes, W. W. Cooper and E. Rhodes. Measuring the efficiency of decision making units. {\it European Journal of Operaional Research}, 2(6), 429--444, 1978.
	\bibitem{Bar}Bar-Cohen AA, Rohsenow WM. Thermally Optimum Spacing of Vertical, Natural Convection Cooled, Parallel Plates. {\it ASME. J. Heat Transfer}. 1984;106(1):116-123. doi:10.1115/1.3246622.
	% 中文学术期刊中的文章
	%\bibitem{paper:chinese} 韩松, 魏权龄. 资源配置的非参数~DEA~模型. {\it 系统工程理论与实践}, 22, 59--64, 2002.
	
\end{thebibliography}