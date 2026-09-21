# WPD Example Code and Data

This repository includes the WPD code and input data.

## Download and run

Git LFS is required when cloning:

```bash
git lfs install
git clone https://github.com/Zqinnn/WPD_test.git
cd WPD_test
tar -xzf Xin_WPD.tar.gz
cd Xin_WPD/Application/Hurricane_WPD
bash run.sh
```


## Versions

- **Uniform:** supports five related QoIs: horizontal wind speed (`q=0`), temperature in kelvin (`q=1`), virtual temperature (`q=2`), air density (`q=3`), and WPD (`q=4`).
- **Sensitive:** uses the final WPD (`q=4`) as the optimization target, selecting one variable's next bitplane at each search step.


## Notes

- `run.sh` clears the Linux filesystem cache before each run. Remove the `drop_cache` calls if cache clearing is unnecessary or unavailable.
- Sampling and linear interpolation components used in *Tango: A Cross-layer Approach to Managing I/O Interference over Local Ephemeral Storage* have been removed from this example.
- The timing labeled “Interpolation time” measures an array copy retained as a placeholder, rather than interpolation. So can ignore it. 
