# Flutter code coverage in a single package app

A simple Flutter project demonstrating how code coverage works in Flutter with a single package APP.

Run flutter test with coverage info (root app folder):

```flutter test --coverage```

Coverage will be available in ```/coverage/lcov.info```.

Convert info into html report (```lcov``` needs to be installed):

```genhtml coverage/lcov.info -o coverage/html```

```-o``` = output folder

Coverage report will be available in ```/coverage/html/index.html```.

Remember to add ```/coverage``` folder to the ```.gitignore``` file.

## Additional info

This is the first part of four repositories teaching how to handle code coverage in Flutter APPs:

[Part 1 - Flutter code coverage in a single package app](https://github.com/cantellir/flutter_code_coverage_single_package);

[Part 2 - Flutter code coverage in a multi package app](https://github.com/cantellir/flutter_code_coverage_multi_package);

[Part 3 - Github actions to handle Flutter APP minimum coverage](https://github.com/cantellir/flutter_code_coverage_minimum_github_action);

[Part 4 - Integration with Codecov analysis tool](https://github.com/cantellir/flutter_code_coverage_github_codecov);