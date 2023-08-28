# v8-running-ng-configs

# Getting Started

1. Checkout v8
2. Apply the harness hook patch: `cd /path/to/v8 && git apply /path/to/harness-20230828.patch`
3. Build v8
4. Build harness library: `cd harness && make libharness.so`
5. Update [_configs/common.yml#L7_](https://github.com/wenyuzhao/v8-running-ng-configs/blob/main/configs/common.yml#L7) to the path of your locally cloned octane.
6. Update [_configs/common.yml#L8_](https://github.com/wenyuzhao/v8-running-ng-configs/blob/main/configs/common.yml#L8) to _path/to/this/repo/harness/octane.js_.
6. Update [_configs/common.yml#L70_](https://github.com/wenyuzhao/v8-running-ng-configs/blob/main/configs/common.yml#L70) to _path/to/this/repo/harness/libharness.so_.
3. Update [_configs/example.yml#L11_](https://github.com/wenyuzhao/v8-running-ng-configs/blob/main/configs/example.yml#L11) to _path/to/v8/out/x64.release/d8_.
3. Run the benchmark suite: `running runbms ./results ./configs/example.yml 8 3`
