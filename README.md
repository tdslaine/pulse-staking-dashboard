# PLS staking dashboard Adjustd for Mainnet

Based by Yoldark's + raskitoma work.

<img src=preview.PNG>

# Requirement
* Grafana 8
* Prometheus with more than 30 days of data retention
* Cryptowat (optional) << I don't know how to configure this.  Any help will be appreciated!
* Nodes: Execution, Consensus and Validator with metrics on.

# Features
* Handle lot of keys
* Display annualized % (kind of)
* ~Support currency conversion thanks cryptowat~  << This have not been implemented yet!
* Displays PLS gains
* Display status of validators (was very hard to do)
* Built in alerts
* Display attestation, aggregate and proposed count per validators
* Keep tracks of daily and monthly income

# TODO
* ~Add aggregated and proposed blocks in the validator table (there is only attestation right now)~

# Issues
* ~Cpu usage can't be displayed as it is not provided~ Load avg added which should be a suitable solution.
* ~Process starting time is an educated guess as not provided, it should be enough~ Metrics implemented in Tony release, i use them now
* The bottom node graph is supposed to display global balance for exited and withdrawable validators. This is not the case as lighthouse do not provide this info.
* ~Log types counter are merged, need warning and error counter~ It is because there is no error logs

eth + prc : `0xCB00d822323B6f38d13A1f951d7e31D9dfDED4AA` (Mine)

eth donation : `0x945DF808617bDD3753237eCF0d5D2A8EEedE76d2` (Yoldark's)

eth donation : `0x21A7D66C1f1089b78a2A530580295939Cdf2a0eD` (raskitoma)
