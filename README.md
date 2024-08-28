# Tinkoff_finteck_2024

%-----------------------------------------------------------------------------------------------------------------------------------------------%
%	The MIT License (MIT)
%
%	Copyright (c) 2021 Jitin Nair
%
%	Permission is hereby granted, free of charge, to any person obtaining a copy
%	of this software and associated documentation files (the "Software"), to deal
%	in the Software without restriction, including without limitation the rights
%	to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
%	copies of the Software, and to permit persons to whom the Software is
%	furnished to do so, subject to the following conditions:
%	
%	THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
%	IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
%	FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
%	AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
%	LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
%	OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
%	THE SOFTWARE.
%	
%
%-----------------------------------------------------------------------------------------------------------------------------------------------%

%----------------------------------------------------------------------------------------
%	DOCUMENT DEFINITION
%----------------------------------------------------------------------------------------

% article class because we want to fully customize the page and not use a cv template
\documentclass[a4paper,12pt]{article}

%----------------------------------------------------------------------------------------
%	FONT
%----------------------------------------------------------------------------------------

% % fontspec allows you to use TTF/OTF fonts directly
% \usepackage{fontspec}
% \defaultfontfeatures{Ligatures=TeX}

% % modified for ShareLaTeX use
% \setmainfont[
% SmallCapsFont = Fontin-SmallCaps.otf,
% BoldFont = Fontin-Bold.otf,
% ItalicFont = Fontin-Italic.otf
% ]
% {Fontin.otf}

%----------------------------------------------------------------------------------------
%	PACKAGES
%----------------------------------------------------------------------------------------
\usepackage{url}
\usepackage{parskip} 	
%other packages for formatting
\RequirePackage{color}
\RequirePackage{graphicx}
\usepackage[usenames,dvipsnames]{xcolor}
\usepackage[scale=0.9]{geometry}

%%% Работа с русским языком
\usepackage{cmap}					% поиск в PDF
\usepackage{mathtext} 				% русские буквы в формулах
\usepackage[T2A]{fontenc}			% кодировка
\usepackage[utf8]{inputenc}			% кодировка исходного текста
\usepackage[english,russian]{babel}	% локализация и переносы
\usepackage{indentfirst}
\frenchspacing

%tabularx environment
\usepackage{tabularx}

%for lists within experience section
\usepackage{enumitem}

% centered version of 'X' col. type
\newcolumntype{C}{>{\centering\arraybackslash}X} 

%to prevent spillover of tabular into next pages
\usepackage{supertabular}
\usepackage{tabularx}
\newlength{\fullcollw}
\setlength{\fullcollw}{0.47\textwidth}

%custom \section
\usepackage{titlesec}				
\usepackage{multicol}
\usepackage{multirow}

%CV Sections inspired by: 
%http://stefano.italians.nl/archives/26
\titleformat{\section}{\Large\scshape\raggedright}{}{0em}{}[\titlerule]
\titlespacing{\section}{0pt}{10pt}{10pt}

%for publications
\usepackage[style=authoryear,sorting=ynt, maxbibnames=2]{biblatex}

%Setup hyperref package, and colours for links
\usepackage[unicode, draft=false]{hyperref}
\definecolor{linkcolour}{rgb}{0,0.2,0.6}
\hypersetup{colorlinks,breaklinks,urlcolor=linkcolour,linkcolor=linkcolour}
\addbibresource{citations.bib}
\setlength\bibitemsep{1em}
%for social icons
\usepackage{fontawesome5}


%debug page outer frames
%\usepackage{showframe}

%----------------------------------------------------------------------------------------
%	BEGIN DOCUMENT
%----------------------------------------------------------------------------------------
\begin{document}

% non-numbered pages
\pagestyle{empty} 

%----------------------------------------------------------------------------------------
%	TITLE
%----------------------------------------------------------------------------------------

% \begin{tabularx}{\linewidth}{ @{}X X@{} }
% \huge{Your Name}\vspace{2pt} & \hfill \emoji{incoming-envelope} email@email.com \\
% \raisebox{-0.05\height}\faGithub\ username \ | \
% \raisebox{-0.00\height}\faLinkedin\ username \ | \ \raisebox{-0.05\height}\faGlobe \ mysite.com  & \hfill \emoji{calling} number
% \end{tabularx}

\begin{tabularx}{\linewidth}{@{} C @{}}
\Huge{Крейс Алексей} \\[7.5pt]
\href{https://github.com/IT-Schnitzel}{\raisebox{-0.05\height}\faGithub\ https://github.com/IT-Schnitzel} \ $|$ \ 
\href{mailto:oficealex@mail.ru}{\raisebox{-0.05\height}\faEnvelope \ oficealex@mail.ru} \ $|$ \ 
\href{tel:+79651583031}{\raisebox{-0.05\height}\faMobile \ +7.965.158.30.31} \\
\end{tabularx}

%----------------------------------------------------------------------------------------
% EXPERIENCE SECTIONS
%----------------------------------------------------------------------------------------

%Interests/ Keywords/ Summary
\section{О себе}
Я энергичный и мотивированный студент интересующийся программированием и новыми технологиям. Стараюсь постоянно совершенствовать навыки в программировании и участвовать в интересных и перспективных проектах.



\section{Образование}
\begin{tabularx}{\linewidth}{@{}l X@{}}	
2023 - н.в & Учусь на направлении "Программная инженерия” в \textbf{РТУ МИРЭА} \hfill \\
2021 - 2022 & 	Диплом о неоконченном высшем образовании, Факультет компьютерных наук (Программная инженерия) (\textbf{НИУ ВШЭ})   \\
2021 & Получил аттестат о среднем общем образовании с отличием \textbf{"Школа 58"} \\ 


\end{tabularx}

%Experience
\section{Достижения}

\begin{tabularx}{\linewidth}{ @{}l r@{} }
\multicolumn{2}{@{}X@{}}{Победитель олимпиады "Ломоносов" по математике}  \\
\multicolumn{2}{@{}X@{}}{Докладчик национальной научно-технической конференции с международным участием «Перспективные материалы и технологии»-2024}  \\
\multicolumn{2}{@{}X@{}}{Медаль "за особые успехи в обучении"}  \\
\end{tabularx}



%Experience
\section{Опыт работы}

\begin{tabularx}{\linewidth}{ @{}l r@{} }
\textbf{стартап AiCraft} & \hfill сентябрь 2021 - февраль 2022 \\[3.75pt]
\multicolumn{2}{@{}X@{}}{Участвовал в разработке продукта AimBox, в частности, отвечал за первичную обработку приходящих с камер данных, сравнение получаемой информации с отображением в WMS, полностью разработал алгоритм декодирование штрихкодов}  \\
\end{tabularx}


\section{Навыки}
\begin{tabularx}{\linewidth}{@{}l X@{}}
Языки программирования: Java, Python, C++, С
\cr Spring Framework: Boot, Web MVC, Data JPA, Security, Cloud; RestTemplate, WebClient
\cr PostgreSQL, MongoDB, SQLite
\cr Docker, Kubernetes, Kafka
\cr Vue.JS, HTML, CSS, JavaScript, TypeScript
\cr Maven, Gradle 
\end{tabularx}

\vfill
\end{document}
