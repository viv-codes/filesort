# filesort

![Build](https://img.shields.io/github/workflow/status/viv-codes/autosort/Lint?style=for-the-badge)
![Python](https://img.shields.io/badge/Made%20with-Python-yellow?style=for-the-badge)
![Black](https://img.shields.io/badge/Code%20Style-Black-black?style=for-the-badge)

A utility that automatically organizes files based on metadata within the linux filesystem. Currently can sort by day, month, or year. Future functionality will include options to sort by file extension or only sort files that have a certain extension

Install filesort:
```
pip install filesort
```

Example input directory prior to sorting:
```
-rw-rw-r--. 1 vivi vivi 854K Feb 18 10:51 'Screenshot from 2022-02-18 10-51-43.png'
-rw-r--r--. 1 vivi vivi  15K Feb 18 12:22 'Screenshot from 2022-02-18 12-22-31.png'
-rw-rw-r--. 1 vivi vivi 1.1M Feb 19 18:00 'Screenshot from 2022-02-19 18-00-18.png'
-rw-rw-r--. 1 vivi vivi 553K Feb 23 10:01 'Screenshot from 2022-02-23 10-01-19.png'

```
Example output directory after sort by day:
```
testfilesort/
└── 2022
    └── Feb
        ├── 18
        │   ├── Screenshot from 2022-02-18 10-51-43.png
        │   └── Screenshot from 2022-02-18 12-22-31.png
        ├── 19
        │   └── Screenshot from 2022-02-19 18-00-18.png
        └── 23
            └── Screenshot from 2022-02-23 10-01-19.png

```
