# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: abenamar <abenamar@student.42.fr>          +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2024/05/13 15:26:20 by abenamar          #+#    #+#              #
#    Updated: 2024/05/13 15:26:25 by abenamar         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME := a.out

INCLUDES := -I $(CURDIR)

SRCS := main.cpp

OBJS := $(SRCS:.cpp=.o)

CC := c++

CFLAGS := -Wall
CFLAGS += -Wextra
CFLAGS += -Werror
CFLAGS += -std=c++98

RM := rm -f

%.o: %.cpp
	$(CC) $(CFLAGS) -c $< -o $@ $(INCLUDES)

$(NAME): $(OBJS)
	$(CC) $(CFLAGS) -o $(NAME) $(OBJS) $(INCLUDES)

all: $(NAME)

clean:
	$(RM) $(OBJS)

fclean: clean
	$(RM) $(NAME)

re: fclean all

.PHONY: re fclean clean all