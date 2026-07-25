# tic-tictoe
this is a game
XOX (Tic-Tac-Toe) Game - 10x10 Board Edition
A two-player Tic-Tac-Toe game played on a 10x10 grid.
Win condition: 5 marks in a row (horizontally, vertically, or diagonally).

Run with:  python xox_game.py
Requires:  Python 3 with Tkinter (usually included by default)
"""

import tkinter as tk
from tkinter import messagebox

BOARD_SIZE = 10
WIN_LENGTH = 5
CELL_SIZE = 45


class XOXGame:
    def _init_(self, root):
        self.root = root
        self.root.title("XOX - 10x10 Tic-Tac-Toe")
        self.root.resizable(False, False)

        self.board = [["" for _ in range(BOARD_SIZE)] for _ in range(BOARD_SIZE)]
        self.current_player = "X"
        self.buttons = [[None for _ in range(BOARD_SIZE)] for _ in range(BOARD_SIZE)]
        self.game_over = F…
