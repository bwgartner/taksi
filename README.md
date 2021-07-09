# taksi

Assess/Evaluate collected support data

For a given data locale, when new support data is deposited, provide a means to:
- implement a next stage, simple data pipeline process
  - look for certain collection scenarios, unpack the respective bundle
  - launch respective analysis tool, collecting resulting output
    - sca-L0
    - sca-server-report
  - WIP
    - if previous runs are available, summarize trend status
    - provide guidance on next steps
    - manage content for longer-term retention structure

## Usage

From this source code repo:

    git clone "this repo"
    cd taksi
      adjust taski.conf to match your context
    sudo ./bin/taksi
        and review the content in the "archiveDir" and runtime "logFile"
	then setup cron/systemd timer to regularly perform this assessment

Or for packaged-based (RPM) for openSUSE/SUSE, see OBS(https://build.opensuse.org/package/show/home:bwgartner:SCA/taksi)

    this has suggested package dependencies
	aludo
        supportutils
	sca-L0
	sca-server-report

