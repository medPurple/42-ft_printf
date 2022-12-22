# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: wmessmer <wmessmer@student.42.fr>          +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2022/11/24 10:12:21 by wmessmer          #+#    #+#              #
#    Updated: 2022/11/28 15:16:36 by wmessmer         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME = libftprintf.a

HEADER = include/ft_printf.h

CC	= gcc

FLAGS = -Wall -Wextra -Werror

SRCS =	srcs/ft_nbr.c \
		srcs/ft_printf.c \
		srcs/ft_putchar_fd.c \
		srcs/ft_putstr_fd.c \
		srcs/ft_strlen.c \
		srcs/ft_hexa.c \
		srcs/ft_hexavoid.c\
		srcs/ft_itoa.c \

OBJS	= ${SRCS:.c=.o}

$(NAME) : ${OBJS}
	ar rc ${NAME} ${OBJS}

all:	${NAME}

clean :
	/bin/rm -f ${OBJS}

fclean : clean
	/bin/rm -f ${NAME}

re : fclean all

.o .c:
	$(CC) $(FLAGS)  -c $< -o ${<:.c = .o}
