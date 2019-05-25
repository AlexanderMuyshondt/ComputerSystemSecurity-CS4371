all: enc ssh

enc: enc1 enc2 dec2

enc1: enc1.c
	gcc -g -Wall -o enc1 enc1.c

enc2: enc2.c
	gcc -lssl -lcrypto -g -Wall -o enc2 enc2.c

dec2: dec2.c
	gcc -lssl -lcrypto -g -Wall -o dec2 dec2.c

ssh: sshpass.c
	gcc -lssh2 -g -o sshpass sshpass.c

clean:
	rm -rf enc1 enc2 dec2 sshpass

