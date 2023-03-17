MPICC = mpicc
CFLAGS = -I.
DEPS = .
OBJ = helloworld.o
EXEC = helloworld

%.o: %.c $(DEPS)
	$(MPICC) -c -o $@ $< $(CFLAGS)

$(EXEC): $(OBJ)
	$(MPICC) -o $@ $^ $(CFLAGS)

.PHONY: clean

clean:
	rm -f $(OBJ) $(EXEC)