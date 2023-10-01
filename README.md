# AB Test Simulation in MATLAB

This repository contains code to simulate a large number of A/B test iterations in MATLAB. The visual output of the simulation presents the number of visitors on the X-axis and shows the percentage of improvements on the Y-axis. The primary objective of this code is to help those new to A/B testing and statistics understand the importance of significance testing. It demonstrates why we cannot solely trust the numbers in a test without considering the influence of random variation on the measured metrics.

## Features

- Generates random conversion rates for different versions being tested.
- Simulates visitor interactions based on these conversion rates.
- Visualizes observed conversion improvements over time.
- Allows for "AA tests" where all versions are identical, to observe the role of random variation.

## Usage

### MATLAB Version

1. Set the desired parameters at the beginning of the script, such as:
   - `base_conv`: Base conversion rate.
   - `factor`: Factor by which conversion rate can vary.
   - `aa_test`: Set to 1 for AA test, 0 otherwise.
   - `versions`: Number of different versions being tested.
   - `new_vis_per_iter`: Number of new visitors in each iteration.
   - `set_iter`: Number of iterations.
   - `num_sims`: Number of simulations.
2. Run the script in MATLAB.
3. Observe the plotted results, which show the true conversion improvements and the observed conversion improvements over time.

## Dependencies

- MATLAB Version: This code uses the `brewermap` function for generating color maps. Ensure you have this function available in your MATLAB path or replace it with an alternative color map function.

## License

[MIT](LICENSE)

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## Contact

For any questions or feedback, please contact [Erik Malkemus](mailto:erikmalk@gmail.com).

## Note

While the MATLAB version accomplishes similar tasks, there might be slight differences in features and user interface compared to the [python version of this code](https://github.com/erikmalk/AB_Test_Simulation).
