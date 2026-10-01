# Game Management System

A Python game rental management system developed for university coursework. The system manages board and video game searches, rentals, returns, subscription checks and customer feedback, with records stored in text files.

The main code and menu are contained in **`menu.ipynb`**.

## Features

- Search for board and video games using case-insensitive matching.
- Check game availability before processing rentals.
- Validate customer subscriptions and enforce concurrent rental limits:
  - Standard: up to 2 games.
  - Premium: up to 7 games.
  - Expired subscriptions cannot rent games.
- Process game returns and collect customer ratings and feedback.
- Analyse rental activity and game ratings.
- Maintain records using text-file storage.

## Repository Files

| File | Description |
|------|-------------|
| `menu.ipynb` | Main notebook containing the core code and menu |
| `Board_Game_info.txt` | Board game records |
| `Video_Game_info.txt` | Video game records |
| `Booking.txt` | Booking records |
| `Rental.txt` | Rental records; `NULL` indicates an unreturned game |
| `Subscription_Info.txt` | Customer subscription records |
| `Game_Feedback.txt` | Game ratings and customer feedback |
| `bgms.jar` | Supporting Java archive supplied with the project |
| `feedbackManager.pyc` | Compiled Python feedback manager module |
| `subscriptionManager.pyc` | Compiled Python subscription manager module |

## Running in Google Colab

1. Download the repository files.
2. Open Google Colab and upload `menu.ipynb`.
3. Use the Files panel to upload the supporting files into the notebook’s working directory.
4. Check any file paths in the notebook and adjust them to match where the files are stored.
5. Run the cells in order.
6. Use the menu to search for games, process rentals and returns, and access analysis features.

If the notebook accesses files through Google Drive, mount your Drive and update the paths to point to your own project folder.

Operations may modify the data files, so keep copies of the original sample records.

## Coursework and Learning

This project applies foundational programming concepts to a practical game rental scenario.

It provided experience in:

- Structuring a program using reusable functions.
- Reading and updating persistent records.
- Validating user input.
- Implementing subscription and rental rules.
- Tracking game availability.
- Analysing rental records and customer feedback.

## Limitations

The system is a coursework prototype using text files for storage. It is intended for a single-user workflow and does not include production account security or concurrent access management.

The `.pyc` files contain compiled Python code and may require a compatible Python version. Their source code is not included in the files shown here.

## Potential Improvements

- Replace text-file storage with a relational database.
- Add automated tests for rental and subscription rules.
- Improve handling of missing or incorrectly formatted files.
- Include Python source files for supporting modules where available.
- Develop a web interface.
