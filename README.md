# ERD/ERS Analysis Pipeline

This notebook provides a reusable pipeline to process EEG data for a simple ERD/ERS analysis. It served as a guiding framework for a thesis project for EEG analysis in a sequential motor learning task.

It:
- Loads pre-processed EEG data for a participant.
- Creates and merges events from annotations.
- Segments the data into epochs (for pre-set conditions).
- Computes time–frequency representations (TFRs) with Morlet wavelets.
- Processes the TFR output to compute ERD/ERS values using baseline normalization,
  including averaging across regions of interest (ROIs).
- Exports and/or plots the final results.
