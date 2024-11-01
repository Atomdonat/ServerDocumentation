# Subnets

![[Network_Layout_dark.png]]

| Subnet                                         | VLAN | Name  | Purpose                                 | Involved Parties                                                  | Colour                                      | Notes |
|-----------------------------------------------:|:----:|:------|:----------------------------------------|:------------------------------------------------------------------|:--------------------------------------------|:------|
| <span style="color:#666666">0.0.0.0/0</span>   |      | Web   | Internet                                | DMZ Router, Proxy, Public Devices                                 | <span style="color:#666666">\#666666</span> |       |
| <span style="color:#7d32a8">10.1.0.0/24</span> |  10  | Home  | Home Network                            | Router, Home Devices                                              | <span style="color:#7d32a8">\#7d32a8</span> |       |
| <span style="color:#00cccc">10.1.1.0/24</span> |  11  | Guest | Guest Network                           | Router, Guest Devices                                             | <span style="color:#00cccc">\#00cccc</span> |       |
| <span style="color:#e8b71a">10.2.0.0/24</span> |  20  | MGMT  | Management and Backups                  | DMZ Router, Backup Server, MGMT Server, TrueNAS, AMP Server       | <span style="color:#e8b71a">\#e8b71a</span> |       |
| <span style="color:#166ee5">10.3.0.0/24</span> |  30  | NAS   | Routing between TrueNAS and Internet    | TrueNAS, DMZ-Router, Proxy                                        | <span style="color:#166ee5">\#166ee5</span> |       |
| <span style="color:#2aa02c">10.3.1.0/24</span> |  30  | AMP   | Routing between AMP Server and Internet | AMP Server, DMZ-Router, Proxy                                     | <span style="color:#2aa02c">\#2aa02c</span> |       |
| <span style="color:#c22525">10.3.2.0/24</span> |  30  | VPN   | Routing between VPN Server and Clients  | TrueNAS, AMP Server, DMZ-Router, Proxy, Authorized Public Devices | <span style="color:#c22525">\#c22525</span> |       |

Inspired by: [[Network_Images.canvas|IP Ranges and Subnets]]

##  IP Lookup table
- [ ] extract Hostname and current IP from DMZ Router config
- [ ] extract Hostname and current IP from Router config

# DMZ Router Config

## Forward Proxy
### Wireguard VPN
#### if ping not working
[![](https://mermaid.ink/img/pako:eNpdks1ugzAQhF9l5UsvARKpJ6RWakJ-Lj21N6gqyzZgATY1dlGU5N27wKpVasnWzux3mLV9YcJKxVJWtnYUNXce3rPCAK6XvNemAmnVYB48jNY1H0tnmwvuIemdFclwHhKjfKL770c8PkvrRu4kkVk-BGkBIeFbiEZANJ7Q-A992hC8W-CxIr3Pxyr6Clo0EHq01-Qf8sHrtgVjl1SYkjrHXLgz1Sei_uWn2SCKnmFL48ziChvch3trjZuuI5st6h9msaPcBGvjlSu5UOkUNo5j9E73CEaup0u9wp5mnBtEnWZxXARbsU65jmuJr3OZvIL5WnWqYCmWkrumYIW5IceDt29nI1jqXVAr5myoapaWvB1QhV5yrzLNK8e7X1dJ7a17XR5__gO3H7Vunws?type=png)](https://mermaid.live/edit#pako:eNpdks1ugzAQhF9l5UsvARKpJ6RWakJ-Lj21N6gqyzZgATY1dlGU5N27wKpVasnWzux3mLV9YcJKxVJWtnYUNXce3rPCAK6XvNemAmnVYB48jNY1H0tnmwvuIemdFclwHhKjfKL770c8PkvrRu4kkVk-BGkBIeFbiEZANJ7Q-A992hC8W-CxIr3Pxyr6Clo0EHq01-Qf8sHrtgVjl1SYkjrHXLgz1Sei_uWn2SCKnmFL48ziChvch3trjZuuI5st6h9msaPcBGvjlSu5UOkUNo5j9E73CEaup0u9wp5mnBtEnWZxXARbsU65jmuJr3OZvIL5WnWqYCmWkrumYIW5IceDt29nI1jqXVAr5myoapaWvB1QhV5yrzLNK8e7X1dJ7a17XR5__gO3H7Vunws)

## Reverse Proxy

# Router Config

# Switch Config


