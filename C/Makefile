# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: lsimon <lsimon@student.42.fr>              +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2018/10/17 11:11:59 by lsimon            #+#    #+#              #
#    Updated: 2019/10/10 14:14:18 by lsimon           ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

CC = gcc

CFLAGS = -Werror -Wall -Wextra

COLLEEN = Colleen
GRACE = Grace
SULLY = Sully

COLLEEN_SRC	 = Colleen.s
GRACE_SRC	 = Grace.s
SULLY_SRC	 = Sully.s

COLLEEN_OBJ	 = Colleen.o
GRACE_OBJ	 = Grace.o
SULLY_OBJ	 = Sully.o

all: $(COLLEEN) $(GRACE) $(SULLY)

$(COLLEEN): $(COLLEEN_OBJ)
	$(CC) -o $@ $^

$(GRACE): $(GRACE_OBJ)
	$(CC) -o $@ $^

$(SULLY): $(SULLY_OBJ)
	$(CC) -o $@ $^

clean:
	rm -f $(OBJS)

fclean: clean
	rm -f $(NAME)

re: fclean all