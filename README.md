# TRABAJO-DE-LIBRO
EJERCICIOS DEL LIBRO
{
 "cells": [
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "# CAPITULO 1"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 6,
   "metadata": {},
   "outputs": [],
   "source": [
    "users = [\n",
    "{ \"id\": 0, \"name\": \"Hero\" },\n",
    "{ \"id\": 1, \"name\": \"Dunn\" },\n",
    "{ \"id\": 2, \"name\": \"Sue\" },\n",
    "{ \"id\": 3, \"name\": \"Chi\" },\n",
    "{ \"id\": 4, \"name\": \"Thor\" },\n",
    "{ \"id\": 5, \"name\": \"Clive\" },\n",
    "{ \"id\": 6, \"name\": \"Hicks\" },\n",
    "{ \"id\": 7, \"name\": \"Devin\" },\n",
    "{ \"id\": 8, \"name\": \"Kate\" },\n",
    "{ \"id\": 9, \"name\": \"Klein\" }\n",
    "]"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 8,
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "[{'id': 0, 'name': 'Hero'},\n",
       " {'id': 1, 'name': 'Dunn'},\n",
       " {'id': 2, 'name': 'Sue'},\n",
       " {'id': 3, 'name': 'Chi'},\n",
       " {'id': 4, 'name': 'Thor'},\n",
       " {'id': 5, 'name': 'Clive'},\n",
       " {'id': 6, 'name': 'Hicks'},\n",
       " {'id': 7, 'name': 'Devin'},\n",
       " {'id': 8, 'name': 'Kate'},\n",
       " {'id': 9, 'name': 'Klein'}]"
      ]
     },
     "execution_count": 8,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "users"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 9,
   "metadata": {},
   "outputs": [],
   "source": [
    "friendships = [(0, 1), (0, 2), (1, 2), (1, 3), (2, 3), (3, 4),\n",
    "(4, 5), (5, 6), (5, 7), (6, 8), (7, 8), (8, 9)]"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 10,
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "[(0, 1),\n",
       " (0, 2),\n",
       " (1, 2),\n",
       " (1, 3),\n",
       " (2, 3),\n",
       " (3, 4),\n",
       " (4, 5),\n",
       " (5, 6),\n",
       " (5, 7),\n",
       " (6, 8),\n",
       " (7, 8),\n",
       " (8, 9)]"
      ]
     },
     "execution_count": 10,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "friendships"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 14,
   "metadata": {},
   "outputs": [
    {
     "ename": "IndentationError",
     "evalue": "expected an indented block (<ipython-input-14-508a03cf9a2a>, line 2)",
     "output_type": "error",
     "traceback": [
      "\u001b[1;36m  File \u001b[1;32m\"<ipython-input-14-508a03cf9a2a>\"\u001b[1;36m, line \u001b[1;32m2\u001b[0m\n\u001b[1;33m    user[\"friends\"]\u001b[0m\n\u001b[1;37m       ^\u001b[0m\n\u001b[1;31mIndentationError\u001b[0m\u001b[1;31m:\u001b[0m expected an indented block\n"
     ]
    }
   ],
   "source": [
    "for user in users:\n",
    "user[\"friends\"]"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 15,
   "metadata": {},
   "outputs": [
    {
     "ename": "IndentationError",
     "evalue": "expected an indented block (<ipython-input-15-bb015def8cf9>, line 3)",
     "output_type": "error",
     "traceback": [
      "\u001b[1;36m  File \u001b[1;32m\"<ipython-input-15-bb015def8cf9>\"\u001b[1;36m, line \u001b[1;32m3\u001b[0m\n\u001b[1;33m    users[i][\"friends\"].append(users[j]) # add i as a friend of j\u001b[0m\n\u001b[1;37m        ^\u001b[0m\n\u001b[1;31mIndentationError\u001b[0m\u001b[1;31m:\u001b[0m expected an indented block\n"
     ]
    }
   ],
   "source": [
    "for i, j in friendships:\n",
    "# this works because users[i] is the user whose id is i\n",
    "users[i][\"friends\"].append(users[j]) # add i as a friend of j\n",
    "users[j][\"friends\"].append(users[i]) # add j as a friend of i"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "# CAPITULO 2"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 19,
   "metadata": {},
   "outputs": [],
   "source": [
    "list_of_lists = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]\n",
    "easier_to_read_list_of_lists = [ [1, 2, 3],\n",
    "[4, 5, 6],\n",
    "[7, 8, 9] ]\n"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 21,
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "[[1, 2, 3], [4, 5, 6], [7, 8, 9]]"
      ]
     },
     "execution_count": 21,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "list_of_lists"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 23,
   "metadata": {},
   "outputs": [
    {
     "ename": "IndentationError",
     "evalue": "expected an indented block (<ipython-input-23-6d9e20415740>, line 2)",
     "output_type": "error",
     "traceback": [
      "\u001b[1;36m  File \u001b[1;32m\"<ipython-input-23-6d9e20415740>\"\u001b[1;36m, line \u001b[1;32m2\u001b[0m\n\u001b[1;33m    return x * 2\u001b[0m\n\u001b[1;37m         ^\u001b[0m\n\u001b[1;31mIndentationError\u001b[0m\u001b[1;31m:\u001b[0m expected an indented block\n"
     ]
    }
   ],
   "source": [
    "def double(x):\n",
    "return x * 2"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": []
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    " # CAPITULO 4"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 1,
   "metadata": {},
   "outputs": [],
   "source": [
    "height_weight_age = [70, # inches,\n",
    "170, # pounds,\n",
    "40 ] # years"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 3,
   "metadata": {},
   "outputs": [
    {
     "data": {
      "text/plain": [
       "[70, 170, 40]"
      ]
     },
     "execution_count": 3,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "height_weight_age"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 4,
   "metadata": {},
   "outputs": [],
   "source": [
    "grades = [95, # exam1\n",
    "80, # exam2\n",
    "75, # exam3\n",
    "62 ] # exam4"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 5,
   "metadata": {
    "scrolled": true
   },
   "outputs": [
    {
     "data": {
      "text/plain": [
       "[95, 80, 75, 62]"
      ]
     },
     "execution_count": 5,
     "metadata": {},
     "output_type": "execute_result"
    }
   ],
   "source": [
    "grades"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "# CAPITULO 8"
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 25,
   "metadata": {},
   "outputs": [
    {
     "ename": "IndentationError",
     "evalue": "expected an indented block (<ipython-input-25-d93367f3754a>, line 2)",
     "output_type": "error",
     "traceback": [
      "\u001b[1;36m  File \u001b[1;32m\"<ipython-input-25-d93367f3754a>\"\u001b[1;36m, line \u001b[1;32m2\u001b[0m\n\u001b[1;33m    \"returns the probability that a uniform random variable is <= x\"\u001b[0m\n\u001b[1;37m                                                                   ^\u001b[0m\n\u001b[1;31mIndentationError\u001b[0m\u001b[1;31m:\u001b[0m expected an indented block\n"
     ]
    }
   ],
   "source": [
    "def uniform_cdf(x):\n",
    "\"returns the probability that a uniform random variable is <= x\"\n",
    "if x < 0: return 0 # uniform random is never less than 0\n",
    "elif x < 1: return x # e.g. P(X <= 0.4) = 0.4\n",
    "else: return 1 # uniform random is always less than 1"
   ]
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python 3",
   "language": "python",
   "name": "python3"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.7.0"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 2
}
