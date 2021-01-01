 .model small
.stack 100h
.data
.code
Main proc
 mov ah,1
 int   21h
mov bl,2
mov cl,1
sub bl,cl   ;subtract value in cl register  from value in bl register
mov dl,bl
add dl,48      
mov ah,2
int 21h
mov ah, 4ch
int 21h
	
main endp
end main
