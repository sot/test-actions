name: Test runner cleanup
on:
  repository_dispatch:
    types:
      - test-cleanup

jobs:
  conda-test:
    runs-on: fido
    name: Testing Runner Cleanup
    steps:
      - name: Create and activate
        run: |
          echo PATH $PATH
          conda list
        env:
          CONDA_PASSWORD: ${{ secrets.CONDA_PASSWORD }}
          SKA: /proj/sot/ska
          SYBASE_OCS: OCS-16_0
          SYBASE: /soft/SYBASE16.0
          LD_LIBRARY_PATH: /soft/SYBASE16.0/OCS-16_0/lib
