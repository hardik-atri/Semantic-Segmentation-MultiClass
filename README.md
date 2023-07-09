\documentclass{article}
\usepackage{enumitem}

\begin{document}

\title{Semantic Segmentation Project}
\author{Your Name}
\date{\today}
\maketitle

\section{Overview}
This project focuses on semantic segmentation using a U-net model with the ResNet34 architecture. The goal is to label each pixel in an image with a corresponding class label.

\section{Dataset}
\begin{itemize}
  \item The dataset is obtained from the Cityscapes website.
  \item It contains 2400 images, totaling approximately 17 GB.
  \item The images and corresponding masks are used for training the model.
\end{itemize}

\section{Preprocessing}
\begin{enumerate}[label=\arabic*.]
  \item Load the images and masks from the dataset.
  \item Store the paths of the images and masks in a data frame.
  \item Perform preprocessing on the images and masks.
\end{enumerate}

\section{Data Normalization}
\begin{itemize}
  \item Normalize the input images to ensure consistent and standardized input for the model.
\end{itemize}

\section{Model Building}
\begin{itemize}
  \item Utilize the U-net model architecture with ResNet34 as the backbone.
  \item Compile the model using the Adam optimizer.
  \item Use Dice Loss as the loss function for training the model.
  \item Evaluate the model using the IOU (Intersection over Union) score.
\end{itemize}

\section{Training}
\begin{itemize}
  \item Fit the compiled model on the input images and their corresponding masks.
  \item Train the model to learn pixel-wise semantic labels.
\end{itemize}

\section{Results}
\begin{itemize}
  \item After training, the model achieved an IOU score of 43\%.
  \item Evaluate and analyze the performance of the model based on the IOU score.
\end{itemize}

\section{Future Improvements}
\begin{itemize}
  \item Experiment with different model architectures and backbones.
  \item Explore advanced data augmentation techniques to improve performance.
  \item Increase the dataset size for better generalization.
\end{itemize}

\end{document}
