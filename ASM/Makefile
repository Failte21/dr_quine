# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: lsimon <lsimon@student.42.fr>              +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2019/10/10 12:55:55 by lsimon            #+#    #+#              #
#    Updated: 2019/10/10 12:58:51 by lsimon           ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

COLLEEN = Colleen
GRACE = Grace
SULLY = Sully

AS = nasm

COLLEEN_SRC	 = Colleen.s
GRACE_SRC	 = Grace.s
SULLY_SRC	 = Sully.s

COLLEEN_OBJ	 = Colleen.o
GRACE_OBJ	 = Grace.o
SULLY_OBJ	 = Sully.o

all: $(COLLEEN) $(GRACE) $(SULLY)

$(COLLEEN): $(COLLEEN_OBJ)
	@ar -r $@ $^
	@ranlib $@

$(GRACE): $(GRACE_OBJ)
	@ar -r $@ $^
	@ranlib $@

$(SULLY): $(SULLY_OBJ)
	@ar -r $@ $^
	@ranlib $@

%.o: %.s
	$(AS) -f macho64 $^ -o $@

clean:
	rm -f $(COLLEEN_OBJ) $(GRACE_OBJ) $(SULLY_OBJ)

fclean: clean
	rm -f $(COLLEEN) $(GRACE) $(SULLY)

re: fclean all
