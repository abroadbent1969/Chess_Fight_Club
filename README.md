
# Advanced Chess AI Self-Play with Castling & Checkmate

This is a web-based chess game featuring an AI that plays against itself using a minimax algorithm with a configurable depth. The game supports castling, checkmate detection, pawn promotion, and various custom board setups. It is built as a single HTML file with embedded CSS and JavaScript.

## Features
- **AI Self-Play**: Two AI instances play against each other with a search depth of 3.
- **Custom Setups**: Includes standard chess setup and unique configurations like "All Pawns," "Bishops Vs Knights," "Rooks Vs Queens," and "No Pawns."
- **Castling**: Supports king-side and queen-side castling with proper legality checks.
- **Checkmate & Stalemate**: Detects game-ending conditions, including checkmate and threefold repetition.
- **Pawn Promotion**: Pawns automatically promote to queens when reaching the opponent's back rank.
- **Visuals**: Renders a chessboard with piece images (if available) or Unicode symbols as a fallback, with move highlighting.
- **Controls**: Start, stop, and switch between different board setups via buttons.

## Prerequisites
- A modern web browser (e.g., Chrome, Firefox, Safari).
- Optional: Image files for chess pieces (`pieces/wp.png`, `pieces/wr.png`, etc.) in the same directory for visual rendering. If images are missing, text symbols are used.

## Setup
1. Save the code as `index.html`.
2. (Optional) Place chess piece images in a `pieces` folder alongside `index.html` (e.g., `pieces/wp.png` for white pawn).
3. Open `index.html` in a web browser.

## Usage
- **Start the Game**: Click "Start AI Game" to begin the AI self-play with the current setup.
- **Select Setup**: Use buttons like "Standard Setup," "All Pawns," etc., to load different board configurations.
- **Stop the Game**: Click "Stop Game" to halt the AI play.
- **Game Status**: The status is displayed above the board, updating with moves, checks, and game outcomes.

## Code Structure
- **HTML**: Defines the canvas for the board and control buttons.
- **CSS**: Styles the board, buttons, and status display with a dark theme.
- **JavaScript**:
  - **Game State**: Manages the 8x8 board, player turns, king positions, and castling rights.
  - **Move Logic**: Handles piece movement, legality checks, and pawn promotion.
  - **AI**: Implements a minimax algorithm for move selection with piece-square tables for evaluation.
  - **Rendering**: Draws the board and pieces, highlighting last moves.

## Custom Setups
- **Standard Setup**: Classic chess starting position.
- **All Pawns**: Boards filled with pawns and kings.
- **Bishops Vs Knights**: One side has bishops, the other knights.
- **Rooks Vs Queens**: One side has rooks, the other queens.
- **No Pawns**: A mix of bishops, rooks, knights, and queens, excluding pawns.

## Limitations
- **AI Depth**: Fixed at 3, which may limit strategic depth. Increasing depth could slow performance.
- **Promotion**: Pawns only promote to queens; other promotions (e.g., to knights) are not supported.
- **No Human Play**: Designed for AI self-play only, with no manual move input.
- **Image Dependency**: Requires piece images for full visual effect; missing images fall back to text.

## Contributing
Feel free to fork this repository and submit pull requests for enhancements, such as:
- Adding human player mode.
- Supporting multiple promotion options.
- Improving AI with deeper search or alternative algorithms.

## License
This project is open-source. Use it as you wish, but consider giving credit if you adapt it!

## Created
Developed on September 29, 2025, by Alex Broadbent.