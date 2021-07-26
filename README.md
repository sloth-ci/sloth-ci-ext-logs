# File Logging for Sloth CI

You can customize your logging in a number of ways: set the output dir and filename, set log level and format, toggle and configure log rotation.


## Installation

    $ pip install sloth-ci-ext-logs


## Usage

    extensions:
        logs:
            # Use the module sloth_ci_ext_logs.
            module: logs

            # Set the log path. Default is the current dir.
            path: debug_logs

            # Log filename. If not given, the app's listen point is used.
            filename: test_debug.log

            # Log level (number or valid Python logging level name).
            level: DEBUG

            # Log format (refer to the https://docs.python.org/3/library/logging.html#logrecord-attributes).
            # By default, this format is used: 
            # format: '%(asctime)s | %(name)30s | %(levelname)10s | %(message)s'

            # Make logs rotating. Default is false.
            # rotating: true

            # If rotating, maximum size of a log file in bytes.
            # max_bytes: 500

            # If rotating, maximum number or log files to keep.
            # backup_count: 10

