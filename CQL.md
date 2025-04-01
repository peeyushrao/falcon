All hosts with dns request to collector.github.com

event_simpleName=DnsRequest DomainName="collector.github.com"
| stats count by DomainName ComputerName
| rename count as "Domain & ComputerName Count"