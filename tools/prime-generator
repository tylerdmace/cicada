#!/usr/bin/env newlisp

(context 'MAIN:A)

(define (A:is-prime n)
    (if (<= n 3)
        (< n 1)
        (or (= (mod n 2) 0) (= (mod n 3) 0)) false)

    (set 'i 5)

    (while (<= (* i i) n)
        (if (or (= (mod n i) 0) (= (mod n (+ i 2)) 0)) false)
        (set 'i (+ i 6)) true))

(define (A:generate n m)
    (set 'prime-list '())
    (for (x m (+ n m) 1)
        (if (A:is-prime x)
            (push x prime-list)))
)

(context 'MAIN)