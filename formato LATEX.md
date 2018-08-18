# Github
Informe de Github


\documentclass[letterpaper,12pt]{report}
\usepackage[right=2cm,left=3cm,top=2cm,bottom=2cm,footskip=1.4cm]{geometry}%margenes de la pagina
\usepackage{fancyhdr}
\pagestyle{fancy}
\usepackage{tikz}
%\pagestyle{fancyplain}

% \fancyhead[C]{ }
% \fancyhead[R]{\thepage}
% \fancyhead[L]{}
% \fancyfoot[C]{}
\pagestyle{headings} %Se puede seleccionar esta opción o todas las anteriores.
\renewcommand{\headrulewidth}{0pt} % grosor de la línea de la cabecera

\usepackage{ucs}
\usepackage[utf8x]{inputenc}
\usepackage[spanish, es-tabla]{babel}
\usepackage[T1]{fontenc}
\usepackage{graphicx}
\usepackage{multicol} %multicolumnas
\usepackage{subfigure} %incluir multiples imágenes en una figura
% \usepackage[vlined, lined, linesnumbered, algosection]{algorithm2e} %paquete para los algoritmos en pseudocódigo
\usepackage{enumerate} %permite cambiar el item de la enumeracion mas facilmente: \begin{enumerate}[(a)] %for small alpha-characters within brackets.
						%Otra opcion renombrar el item: \renewcommand{\labelenumi}{\Alph{enumi}.}
\RequirePackage{hyperref}
\RequirePackage{url} %citacion de URL
\usepackage{hyperref}
\linespread{1.5} %interlineado

\usepackage{listings}
\lstset{language=C, numbers=left, numberstyle=\small, tabsize=2, captionpos=b, frame=single, breaklines=true, basicstyle=\normalsize, showstringspaces=false}
\renewcommand\lstlistingname{Código}

% Para algoritmos
\usepackage{algorithmic}
\usepackage{algorithm}
\floatname{algorithm}{Algoritmo}
\renewcommand{\listalgorithmname}{Lista de algoritmos}
\renewcommand{\algorithmicrequire}{\textbf{Entrada:}}
\renewcommand{\algorithmicensure}{\textbf{Retorna:}}
\renewcommand{\algorithmicprint}{\textbf{ESCRIBIR}}
\newcommand{\READ}[1]{\STATE \textbf{LEER} (#1)}
\renewcommand{\algorithmicif}{\textbf{si}}
\renewcommand{\algorithmicthen}{\textbf{entonces}}
\renewcommand{\algorithmicelse}{\textbf{sino}}
\renewcommand{\algorithmicfor}{\textbf{para}}
\renewcommand{\algorithmicforall}{\textbf{para todo}}
\renewcommand{\algorithmicdo}{\textbf{hacer}}
\renewcommand{\algorithmicrepeat}{\textbf{repetir}}
\renewcommand{\algorithmicreturn}{\textbf{retornar}}
\renewcommand{\algorithmictrue}{\textbf{verdadero}}
\renewcommand{\algorithmicfalse}{\textbf{falso}}
\renewcommand{\algorithmicend}{\textbf{fin}}
\renewcommand{\algorithmicwhile}{\textbf{mientras}}
\renewcommand{\algorithmiccomment}[1]{//#1}
\renewcommand{\algorithmicendloop}{\algorithmicend\ \algorithmicloop}
\renewcommand{\algorithmicendwhile}{\algorithmicend\ \algorithmicwhile}
\renewcommand{\algorithmicendfor}{\algorithmicend\ \algorithmicfor}
\renewcommand{\algorithmicelsif}{\algorithmicelse,\ \algorithmicif}
\renewcommand{\algorithmicendif}{\algorithmicend\ \algorithmicif}

\begin{document}
\renewcommand{\contentsname}{Tabla de Contenido}
\begin{titlepage}
\begin{center}
\vspace*{0.5in}
UNIVERSIDAD PRIVADA DE TACNAO\\
FACULTAD DE INGENIERÍA\\
ESCUELA PROFESIONAL DE INGENIERIA DE SISTEMAS\\
INGENIERÍA DE SISTEMAS

\vspace*{0.5in}
\begin{figure}[htb]
\begin{center}
	\includegraphics[width=8.5cm, height=4cm]{color-836x732.png}
	% color-836x732.png: 836x732 pixel, 72dpi, 29.50x25.83 cm, bb=0 0 836 732
\end{center}
\end{figure}



\vspace*{0.5in}
\begin{Large}
\textbf{GitHub} \\
\end{Large}
\vspace*{1in}


\end{center}
\begin{flushright}

\begin{tabular}{lll}
Integrantes & : & Brandon Dennis Mamani Ayala\\
          &   & 2015052715\\ 
Profesor & : & Ing. Patrick Cuadros Quiroga\\
Curso & : & Base de Datos II\\
Fecha & : & \today
\end{tabular}
\end{flushright}
\end{titlepage}

\tableofcontents

\chapter{¿Qu\'e es Github?}\label{cap:1}
Github es una plataforma creada para facilitar el desarrollo colaborativo de software, nos permite alojar proyectos en la web gratuitamente, por lo general de forma pública, aunque podemos alojar los proyectos de modo privado, si pagamos una pequeña suscripción mensual.

\section{¿Qu\'e nos ofrece?}\label{sec:1}
%\chapter{¿Qu\'e nos ofrece?}\label{cap:2}
Github ofrece al desarrollador toda la potencia y agilidad del sistema de control de versiones Git, más un interesante set de herramientas añadidas:\\
 \begin{itemize}
         \item Wiki.
         \item Sistema de seguimiento de incidencias.
          \item Interfaz gráfica para revisión/comparación de código.
           \item Visor de ramas de desarrollo.
    \end{itemize}
    
\section{¿C\'omo funciona Github?}\label{sec:2}

Lo primero que debemos hacer es crear una cuenta en https://github.com. La activamos por mail y ya podemos crear nuestros repositorios. Los repositorios de Github son el almacén que utilizamos para guardar nuestro código. Github nos ofrece la opción de crear un repositorio vacío, recomendable cuando vamos a iniciar un nuevo desarrollo, o la opción de importar un proyecto ya existente, elegimos la que más nos convenga y mediante unos pocos comandos de consola configuramos la rama principal de nuestro repositorio, que por defecto se llamará "master". Cada programador puede crear sus propias ramas de desarrollo, donde tiene que llevar a cabo sus modificaciones, sin interferir en el trabajo de sus compañeros. Cuando terminamos y validamos un desarrollo paralelo, lo unimos con la rama principal y todos los miembros del equipo pueden descargar las nuevas modificaciones, sin alterar los desarrollos que estén llevando cabo en ese momento. Después de alojar el repositorio público en Github.com, cualquier usuario de la comunidad podrá aportar ideas, hacer un seguimiento del proyecto, incluso copiarlo y modificarlo a su gusto bajo la misma licencia.




\chapter{Crear un nuevo repositorio}\label{cap:2}
Un repositorio generalmente se usa para organizar un solo proyecto. Los repositorios pueden contener carpetas y archivos, imágenes, videos, hojas de cálculo y conjuntos de datos, cualquier cosa que su proyecto necesite. Se recomienda incluir un archivo README o un archivo con información sobre su proyecto.

\section{¿C\'omo crear un repositorio?}\label{sec:1}

\begin{enumerate}[1.]
    \item En la esquina superior derecha, al lado de tu avatar o identicon, haz clic en + (m\'as) y luego seleccione \textbf{Nuevo repositorio}.
    \item Nombra tu repositorio .
    \item Escribe una breve descripción.
    \item Seleccione Inicializar este repositorio con un README.
    \item Finalmente haga click en \textbf{Crear repositorio}.
    
\end{enumerate}

\begin{figure}[htb]
\begin{center}
	\includegraphics[scale=0.8]{crear-repositorio.png}
	% color-836x732.png: 836x732 pixel, 72dpi, 29.50x25.83 cm, bb=0 0 836 732
\end{center}
\end{figure}

\end{document}

%AYUDAS:
insertar codigo desde archivo
\lstinputlisting[caption ={DESCRIPCION} , label=cod:pregunta]{SOURCE}

%insertar codigo
\begin{lstlisting}[caption={DESCRIPCION}, label=cod:pregunta]
\end{lstlisting}1
