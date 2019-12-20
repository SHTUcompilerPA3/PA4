FILE=test.cl
CORR=_corr_answer.out
ME=_your_answer.out
compare:
	./lexer ${FILE} |./parser |./semant |./cgen_right > ${CORR}
	./lexer ${FILE} |./parser |./semant |./cgen > ${ME}
	diff ${CORR} ${ME}
corr:
	./lexer ${FILE} |./parser |./semant |./cgen_right > ${CORR}
you:
	./lexer ${FILE} |./parser |./semant |./cgen > ${ME}
sample:
	./lexer ${FILE} |./parser |./semant |./cgen_sample > _sample_answer.out