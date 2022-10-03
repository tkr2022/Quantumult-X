# Quantumult X懒人配置

[general]
dns_exclusion_list=*.cmpassport.com, *.jegotrip.com.cn, *.icitymobile.mobi, id6.me, *.pingan.com.cn
geo_location_checker=http://ip-api.com/json/?lang=zh-CN, https://github.com/KOP-XIAO/QuantumultX/raw/master/Scripts/IP_API.js
resource_parser_url= https://raw.githubusercontent.com/KOP-XIAO/QuantumultX/master/Scripts/resource-parser.js
profile_img_url= https://raw.githubusercontent.com/KOP-XIAO/QuantumultX/master/img/dragonball/1.PNG
server_check_url=http://www.gstatic.com/generate_204
#第一个filter为4g模式开启规则分流，第二个filter为其他wifi下开启规则分流，第三个wifi1修改成你路由器翻墙的wifi名开启直连模式，第四个wifi2为你公司或者其他有路由器翻墙的WiFi名走直连）
#默认关闭根据wifi切换模式，如需开启，删除下方的“#”即可！
#running_mode_trigger=filter, filter, wifi1:all_direct, wifi2: all_direct

[dns]
server=223.5.5.5
server=114.114.114.114
server=119.29.29.29
server=8.8.8.8
address=/raw.githubusercontent.com/185.199.110.133


[policy]

static=Global, 香港, 台湾, 日本, 韩国, 狮城, 美国, proxy, img-url=https://raw.githubusercontent.com/Koolson/Qure/master/IconSet/Color/Quantumult_X.png
static=YouTube, 香港, 台湾, 日本, 狮城, 韩国, 美国, img-url=https://raw.githubusercontent.com/Koolson/Qure/master/IconSet/Color/YouTube.png 
static=Telegram, 香港, 台湾, 韩国, 日本, 狮城, 美国, img-url=https://raw.githubusercontent.com/Koolson/Qure/master/IconSet/Color/Telegram.png
static=Twitch, 香港, 台湾, 韩国, 日本, 狮城, img-url=https://raw.githubusercontent.com/Koolson/Qure/master/IconSet/Color/Twitch.png
static=Twitter, 香港, 台湾, 韩国, 日本, 狮城, 美国, img-url=https://raw.githubusercontent.com/Koolson/Qure/master/IconSet/Color/Twitter.png
static=TikTok, 台湾, 日本, 韩国, 狮城, 美国, img-url=https://raw.githubusercontent.com/Koolson/Qure/master/IconSet/Color/TikTok_2.png
static=Netflix, 台湾, 日本, 狮城, img-url=https://raw.githubusercontent.com/Koolson/Qure/master/IconSet/Color/Netflix_Letter.png
static=GlobalTV, 香港, 台湾, 韩国, 日本, 狮城, 美国, img-url=https://raw.githubusercontent.com/Koolson/Qure/master/IconSet/Color/Google_Search.png
static=Spotify, 台湾, 日本, 狮城, img-url=https://raw.githubusercontent.com/Koolson/Qure/master/IconSet/Color/Spotify.png
static=FINAL, 香港, 台湾, 日本, 韩国, 狮城, 美国, img-url=https://raw.githubusercontent.com/Koolson/Qure/master/IconSet/Color/Siri.png
static=Apple, direct, img-url=https://raw.githubusercontent.com/Koolson/Qure/master/IconSet/Color/Apple.png
url-latency-benchmark=香港, server-tag-regex=(?i)(港|HK|Hong), check-interval=600, tolerance=0, alive-checking=false, img-url=https://raw.githubusercontent.com/Koolson/Qure/master/IconSet/Color/HK.png
url-latency-benchmark=台湾, server-tag-regex=(?i)(台|TW|Tai), check-interval=600, tolerance=0, alive-checking=false, img-url=https://raw.githubusercontent.com/Koolson/Qure/master/IconSet/Color/TW.png
url-latency-benchmark=韩国, server-tag-regex=(?i)(韩|KR|Korea), check-interval=600, tolerance=0, alive-checking=false, img-url=https://raw.githubusercontent.com/Koolson/Qure/master/IconSet/Color/KR.png
url-latency-benchmark=日本, server-tag-regex=(?i)(日本|川日|东京|大阪|泉日|埼玉|沪日|日|深日|JP|Japan), check-interval=600, tolerance=0, alive-checking=false, img-url=https://raw.githubusercontent.com/Koolson/Qure/master/IconSet/Color/JP.png
url-latency-benchmark=狮城, server-tag-regex=(?i)(新加坡|坡|狮城|SG|Singapore), check-interval=600, tolerance=0, alive-checking=false, img-url=https://raw.githubusercontent.com/Koolson/Qure/master/IconSet/Color/SG.png
url-latency-benchmark=美国, server-tag-regex=(?i)(美|United States), check-interval=600, tolerance=0, alive-checking=false, img-url=https://raw.githubusercontent.com/Koolson/Qure/master/IconSet/Color/US.png
[server_remote]

[filter_remote]
https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/QuantumultX/Twitch/Twitch.list, tag=Twitch, force-policy=Twitch, update-interval=172800, 
opt-parser=true, enabled=true
https://raw.githubusercontent.com/DivineEngine/Profiles/master/Quantumult/Filter/Extra/Twitter.list, tag=Twitter, force-policy=Twitter, 
update-interval=172800, opt-parser=false, enabled=true
https://raw.githubusercontent.com/Semporia/TikTok-Unlock/master/Quantumult-X/TikTok.list, 
tag=TikTok, force-policy=TikTok, update-interval=86400, opt-parser=false, enabled=true
https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/QuantumultX/TestFlight/TestFlight.list, 
tag=TestFlight, force-policy=Global, update-interval=86400, opt-parser=true, enabled=true
https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/QuantumultX/Apple/Apple.list, tag=Apple, force-policy=Apple, update-interval=86400, 
opt-parser=true, enabled=true
https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/QuantumultX/YouTube/YouTube.list, tag=YouTube, force-policy=YouTube, update-interval=86400, opt-parser=true, enabled=true
https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/QuantumultX/Netflix/Netflix.list, tag=Netflix, force-policy=Netflix, update-
interval=86400, opt-parser=true, enabled=true
https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/QuantumultX/GlobalMedia/GlobalMedia.list, tag=GlobalTV, force-policy=Global, update-interval=86400, opt-parser=true, enabled=true
https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/QuantumultX/Telegram/Telegram.list, tag=Telegram, force-policy=Telegram, update-interval=86400, opt-parser=true, enabled=true
https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/QuantumultX/Advertising/Advertising.list, tag=广告拦截, force-policy=reject, update-
interval=86400, opt-parser=true, enabled=true
https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/QuantumultX/Proxy/Proxy.list, tag=全球规则, 
force-policy=Global, update-interval=86400, opt-parser=true, enabled=true
https://raw.githubusercontent.com/blackmatrix7/ios_rule_script/master/rule/QuantumultX/China/China.list, tag=全球直连, force-policy=DIRECT, update-interval=86400, 
opt-parser=true, enabled=true

[rewrite_remote]
https://raw.githubusercontent.com/chavyleung/scripts/master/box/rewrite/boxjs.rewrite.quanx.tf.conf, tag=Boxjs, update-interval=86400, opt-parser=false, enabled=true
https://raw.githubusercontent.com/w37fhy/QuantumultX/master/QuantumultX_JS.conf, tag=比价等脚本, update-interval=86400, opt-parser=false, enabled=true
https://raw.githubusercontent.com/w37fhy/QuantumultX/master/QuantumultX_Cookie.conf, tag=获取Cookie, update-interval=86400, opt-parser=false, enabled=true

[server_local]

[filter_local]
host-suffix, local, DIRECT
ip-cidr, 192.168.0.0/16, DIRECT
ip-cidr, 10.0.0.0/8, DIRECT
ip-cidr, 172.16.0.0/12, DIRECT
ip-cidr, 127.0.0.0/8, DIRECT
ip-cidr, 100.64.0.0/10, DIRECT
ip-cidr, 224.0.0.0/4, DIRECT
ip6-cidr, fe80::/10, DIRECT
ip-cidr, 203.107.1.1/24, reject
geoip, cn, DIRECT
final, FINAL

[rewrite_local]

[task_local]

[mitm]





