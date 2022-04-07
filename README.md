# pacman
definição de constantes

#lang racket

(require 2htdp/image)
(require 2htdp/universe)

(provide (all-defined-out))


(define ALTURA-CENARIO 600)
(define LARGURA-CENARIO 800)
(define CENARIO (empty-scene LARGURA-CENARIO ALTURA-CENARIO))

(define MEIO-X (/ LARGURA-CENARIO 2))
(define MEIO-Y (/ ALTURA-CENARIO 2))


///////////////////////PACMAN//////////////////////////////

(define IMG-PACMAN (bitmap "pac-man.jpg")
(define LARGURA-PACMAN (image-width IMG-PACMAN))
(define ALTURA-PACMAN (image-height IMG-PACMAN))


//////////////////////AMARELO//////////////////////////////

(define IMG-AMARELO (bitmap "amarelo.png")
(define LARGURA-AMARELO (image-width IMG-AMARELO))
(define ALTURA-AMARELO (image-height IMG-AMARELO))


/////////////////////VERMELHO//////////////////////////////

(define IMG-VERMELHO (bitmap "vermelho.png")
(define LARGURA-VERMELHO (image-width IMG-VERMELHO))
(define ALTURA-VERMELHO (image-height IMG-VERMELHO))


///////////////////////VERDE//////////////////////////////

(define IMG-VERDE (bitmap "verde.png")
(define LARGURA-VERDE (image-width IMG-VERDE))
(define ALTURA-VERDE (image-height IMG-VERDE))


//////////////////////AZUL////////////////////////////////

(define IMG-AZUL (bitmap "azul.png")
(define LARGURA-AZUL (image-width IMG-AZUL))
(define ALTURA-AZUL (image-height IMG-AZUL))




(define METADE-L-PACMAN (/ LARGURA-PACMAN 2))
(define METADE-L-AZUL (/ ALTURA-PACMAN 2))
(define METADE-L-VERDE (/ ALTURA-PACMAN 2))
(define METADE-L-VERMELHO (/ ALTURA-PACMAN 2))
(define METADE-L-AMARELO (/ ALTURA-PACMAN 2))


(define LIMITE_ESQUERDO (+ 0 (/ image-width IMG-PACMAN) 2))
(define LIMITE-DIREITO (- LARGURA-CENARIO (/ (image-width IMG-PACMAN) 2)))
