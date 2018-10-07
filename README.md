API Call:
* https://api.apptoken.co

For streaming data:
* Use zeromq: http://zeromq.org/
* tcp://api.apptoken.co:5556

Test
API call:

```
/
```

API respond:

```
Welcome to the Apptoken API!
```

#### All Stamps
API call:

```
/stamps?page=1
```

API respond:

```
{"page_info":
{"has_next_page":true},
"stamps":
[{"author":"theapptokens",
"content":"Lots of exciting new developments in crypto land recently...",
"num_replies":2,
"reply_to":null,
"seq":467012198,
"timestamp":"2018-09-25T02:09:13",
"tips":0,
"transaction_id":"babd309692125d4222fe3b781a824e2ba4d5dd77abd6c7791ce6bcce86da3744"},
{"author":"masteryoshil",
"content":"Wall Street, venture capitalists and crypto companies descend on Capitol Hill to debate regulation: https://www.cnbc.com/2018/09/24/lawmakers-venture-capitalists-and-crypto-companies-descend-on-on-capitol-hill-to-debate-regulation.html",
"num_replies":2,
"reply_to":null,
"seq":466014568,
"timestamp":"2018-09-24T18:36:38",
"tips":40000,
"transaction_id":"bf3f99ad88734668b4bec291f40f259cecdba832c261e57e0cadfe8c373a7235"},
{"author":"masteryoshil",
"content":"Japan Lost $540 Million to Crypto Hacks in First Half of 2018: https://www.coindesk.com/japan-lost-540-million-to-crypto-hacks-in-first-half-of-2018/",
"num_replies":3,
"reply_to":null,
"seq":446538918,
"timestamp":"2018-09-21T00:59:29.5",
"tips":60000,
"transaction_id":"e3988646120490d6b987332c1835319e8634548ca507a4958255b46553b6ca4a"},
{"author":"seyertam1234",
"content":"All green across the board!",
"num_replies":3,
"reply_to":null,
"seq":446487795,
"timestamp":"2018-09-21T00:44:36.5",
"tips":40000,
"transaction_id":"2b0d7e4bbcee4133372cd8c46ce2027429f8a2c93235c133112b90725e0d295e"},
{"author":"masteryoshil",
"content":"Another beautiful day!",
"num_replies":1,
"reply_to":null,
"seq":446323272,
"timestamp":"2018-09-20T23:41:12",
"tips":0,
"transaction_id":"954e453db16ee7fc74b2ce8be0ea035239c8bec04bf608d2367002b25baca6a9"}]}
```

#### Specific Stamp
API call:

```
/stamps/<stamp_id>

/stamps/babd309692125d4222fe3b781a824e2ba4d5dd77abd6c7791ce6bcce86da3744
```

API respond:

```
{"author":"theapptokens",
"content":"Lots of exciting new developments in crypto land recently...",
"num_replies":2,
"reply_to":null,"seq":467012198,
"timestamp":"2018-09-25T02:09:13",
"tips":0,
"transaction_id":"babd309692125d4222fe3b781a824e2ba4d5dd77abd6c7791ce6bcce86da3744"}
```

#### All Replies for a Stamp
API call:

```
/stamps/<stamp_id>/replies

/stamps/babd309692125d4222fe3b781a824e2ba4d5dd77abd6c7791ce6bcce86da3744/replies
```

API respond:

```
{"page_info":
{"has_next_page":false},
"replies":
[{"author":"seyertam1234",
"content":"Yep, very true!",
"num_replies":0,
"reply_to":"babd309692125d4222fe3b781a824e2ba4d5dd77abd6c7791ce6bcce86da3744","seq":467013642,"timestamp":"2018-09-25T02:09:36.5",
"tips":0,
"transaction_id":"8f0714389588c1e5309718c8350b8eff25068d9f9e0daac0d2255c9eba8d24e2"},
{"author":"masteryoshil",
"content":"Good technical developers coming!",
"num_replies":0,
"reply_to":"babd309692125d4222fe3b781a824e2ba4d5dd77abd6c7791ce6bcce86da3744",
"seq":467040081,
"timestamp":"2018-09-25T02:18:00.5",
"tips":0,
"transaction_id":"a505a08177080dc50d0799993fd6f2863f689bb6545a19cd9b4fe1bdde151bd9"}]}
```

#### All Stamps for an Author
API call:

```
/authors/<author>/stamps

/authors/seyertam1234/stamps
```

API respond:

```
{"page_info":
{"has_next_page":false},
"stamps":
[{"author":"seyertam1234",
"content":"All green across the board!",
"num_replies":3,
"reply_to":null,
"seq":446487795,
"timestamp":"2018-09-21T00:44:36.5",
"tips":40000,
"transaction_id":"2b0d7e4bbcee4133372cd8c46ce2027429f8a2c93235c133112b90725e0d295e"},
{"author":"seyertam1234",
"content":"Hey hey hey","num_replies":4,
"reply_to":null,
"seq":442342439,
"timestamp":"2018-09-20T02:31:23.5",
"tips":0,
"transaction_id":"7eb48d92e20e0eef66e75ffe93cd9ba4932e8e1ef6f0a74d8d1200fb6e261887"}]}
```

#### Avatar of an Author
API call:

```
/authors/<author>/avatar

/authors/theapptokens/avatar
```

API respond:

```
{"url":"https://upload.wikimedia.org/wikipedia/en/thumb/8/8b/Avatar_2_logo.jpg/220px-Avatar_2_logo.jpg","username":"theapptokens"}
```



