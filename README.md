# v8-running-ng-configs

# Getting Started

1. Checkout v8
2. Apply the harness hook patch: `cd /path/to/v8 && git apply /path/to/harness-20230828.patch`
3. Build v8
4. Update _https://github.com/wenyuzhao/v8-running-ng-configs/blob/main/configs/common.yml#L7-L8_ to your cloned octane.
3. Update _./configs/example.yml_ and point the d8 executable to your d8 binary.
3. Run benchmark: `running runbms ./results ./configs/example.yml 8 3`
