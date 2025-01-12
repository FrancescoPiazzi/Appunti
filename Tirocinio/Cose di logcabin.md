# Sembra importante ma non capisco
https://github.com/logcabin/logcabin/blob/ee6c55ae9744b82b451becd9707d26c7c1b6bbfb/Server/RaftConsensus.cc#L2516
https://github.com/logcabin/logcabin/blob/ee6c55ae9744b82b451becd9707d26c7c1b6bbfb/Server/RaftConsensus.cc#L2191

# Cose che logcabin fa e io no
- [ ] this is probably a problem in my code as well: 
https://github.com/logcabin/logcabin/blob/ee6c55ae9744b82b451becd9707d26c7c1b6bbfb/Server/RaftConsensus.cc#L1340
- [ ] apparently nodes refuse the vote of a candidate if they have recently heard from a leader, with the idea that the candidate is wrong for starting an election
https://github.com/logcabin/logcabin/blob/ee6c55ae9744b82b451becd9707d26c7c1b6bbfb/Server/RaftConsensus.cc#L1540
