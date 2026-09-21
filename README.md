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

## Notes

- `run.sh` clears the Linux filesystem cache before each run. Remove the `drop_cache` calls if cache clearing is unnecessary or unavailable.
- The timing labeled “Interpolation time” measures an array copy retained as a placeholder, rather than interpolation. So can ignore it. 
