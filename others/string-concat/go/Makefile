.SUFFIXES: .go .6

N=100000
C=3

.go.6:
	6g $<

.6.out:
	6l -o $@ $<

all:	bench_strcat.out
	N=$(N) C=$(C) ./bench_strcat.out

clean:
	rm -f *.out
