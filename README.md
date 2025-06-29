HP Warranty Scraper
A simple Python-based web scraper that captures the serial number of an HP machine, queries the HP Warranty Check site, and writes the warranty end date to the Windows Registry.
Perfect for feeding warranty info into RMM tools or UDFs via PowerShell scripts.

HP's public warranty API hasn’t been maintained in years, and there’s no reliable way to automate warranty lookups anymore. This tool fills that gap by scraping directly from the HP site using the device's serial number.

Features
- Automatically reads HP device serial from WMI.
- Scrapes warranty end date from HP's support site.
- Writes the result to the Windows Registry.
- Easy integration with your RMM via follow-up PowerShell scripts.
- Lightweight.

Compile
Make sure Python is installed, then run:

pyinstaller --onefile --windowed .\your_script.py

Disclaimer
I'm not a professional developer — just an MSP frustrated by the lack of support from HP’s APIs. This tool is stitched together with online research and late nights. If you find bugs, inefficiencies, or have ideas, feel free to open an issue or PR. Feedback is welcome!
