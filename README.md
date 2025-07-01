# jQuery-with-XSS
jQuery with XSS, Testing and Secure Version

# jQuery versions with known weaknesses
- Bug 9521 (CVE-2011-4969) - $("#`<img src=x onerror=...>`")
- Bug 11290 (CVE-2012-6708) - $("element[attribute='`<img src=x onerror=...>`'")
- issue 2432 (CVE-2015-9251) - 3rd party $.get() auto executes if content type is text/javascript
- issue 11974 (CVE-2015-9251) - parseHTML executes inline scripts like event handlers
- issue 4333 (CVE-2019-11358) - prototype pollution for $.extend()
- issue 4642 (CVE-2020-11022) - htmlPrefilter unwraps things it shouldn't
- issue 4647 (CVE-2020-11023/CVE-2020-23064) - select/option wrapping unwraps can cause XSS
- CVE-2020-7656 - XSS - The load method fails to recognize and remove "<script>" HTML tags that contain a whitespace character, i.e: "</script >"

## Bug list:
- [#4969](https://bugs.jquery.com/ticket/4969)
- [#6708](https://bugs.jquery.com/ticket/6708)
- [#9251](https://bugs.jquery.com/ticket/9251)
- [#9521](https://bugs.jquery.com/ticket/9521)
- [#11290](https://bugs.jquery.com/ticket/11290)
- [#11974](https://bugs.jquery.com/ticket/11974)
- [#11358](https://bugs.jquery.com/ticket/11358)
- [#11022](https://bugs.jquery.com/ticket/11022)
- [#11023](https://bugs.jquery.com/ticket/11023)

## Test version:
- [test](http://research.insecurelabs.org/jquery/test/)

## Safe version：
- 3.5.0，3.5.1
- 3.6.0，3.6.1，3.6.2，3.6.3
- 3.7.0，3.7.1

