# wazuh-pflog
Decoder and rule example for using Wazuh XDR with pflog

The input generated for the decoder has to be created with _tcpdump -nettr /var/log/pflog_

You can add this to your crontab to update every two minutes the pflogtcpdump.log file:

    */2 * * * * /usr/sbin/tcpdump -nettr /var/log/pflog > /var/log/pflogtcpdump.log 2>&1
