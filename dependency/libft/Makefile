NAME		= libft.a

SRCSBONUS	= ./ft_lstadd_back.c\
			  ./ft_lstadd_front.c\
			  ./ft_lstclear.c\
			  ./ft_lstdelone.c\
			  ./ft_lstiter.c\
			  ./ft_lstlast.c\
			  ./ft_lstmap.c\
			  ./ft_lstnew.c\
			  ./ft_lstsize.c\

SRCS		= ./ft_atoi.c\
			  ./ternaire.c\
			  ./ft_bzero.c\
			  ./ft_calloc.c\
			  ./ft_isalnum.c\
			  ./ft_isalpha.c\
			  ./ft_isascii.c\
			  ./ft_isdigit.c\
			  ./ft_isprint.c\
			  ./ft_itoa.c\
			  ./ft_memccpy.c\
			  ./ft_memchr.c\
			  ./ft_memcmp.c\
			  ./ft_memcpy.c\
			  ./ft_memmove.c\
			  ./ft_memset.c\
			  ./ft_putchar_fd.c\
			  ./ft_putendl_fd.c\
			  ./ft_putnbr_fd.c\
			  ./ft_putstr_fd.c\
			  ./ft_split.c\
			  ./ft_strchr.c\
			  ./ft_strdup.c\
			  ./ft_strjoin.c\
			  ./ft_strlcat.c\
			  ./ft_strlcpy.c\
			  ./ft_strlen.c\
			  ./ft_strncmp.c\
			  ./ft_strnstr.c\
			  ./ft_strrchr.c\
			  ./ft_strtrim.c\
			  ./ft_tolower.c\
			  ./ft_toupper.c\
			  ./ft_putstr.c\
			  ./ft_putnbr.c\
			  ./new_malloc.c

INC			= libft.h

CFLAGS		= -Wall -Wextra -Werror

OBJS		= $(SRCS:.c=.o)

OBJSBONUS	= $(SRCSBONUS:.c=.o) $(SRCS:.c=.o)


CC			= gcc

%.o:		%.c		$(INC)
			$(CC) $(CFLAGS) -c -o $@ $<

all			:	$(NAME)

$(NAME)		:			$(OBJS) $(INC)
			ar rc $(NAME) $(OBJS)

bonus		:		$(OBJSBONUS)
			ar rc $(NAME) $? 

clean		:
			rm -rf $(OBJS) $(OBJSBONUS)

fclean		:	clean
			rm -rf $(NAME)

re 			:	fclean all

.PHONY		:	 all clean fclean re bonus
