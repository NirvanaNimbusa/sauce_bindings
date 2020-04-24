---
id: create-session
title: Creating a Session
sidebar_label: Create Session
---

Sauce Bindings allows you to configure numerous capabilities, but it also provides reasonable defaults.
If you want to start and stop a session on a Windows 10 machine with the latest version of Chrome, 
this is all you need to do:

<!--DOCUSAURUS_CODE_TABS-->
<!--Java-->

```java
import com.saucelabs.saucebindings.session;

public class HelloSauce {
    public static void main(String[] args) {
        SauceSession sauceSession = new SauceSession();
        RemoteWebDriver driver = sauceSession.start();

        // use the driver to drive the browser as desired

        sauceSession.stop(True);
    }
}
```

<!--Python-->
```python
from saucebindings.session import SauceSession

sauceSession = SauceSession()
driver = sauceSession.start()

# use the driver to drive the browser as desired

session.stop(True)
```
<!--Ruby-->
```ruby
require 'sauce_bindings'

sauceSession = SauceSession.new
driver = sauceSession.start

# use the driver to drive the browser as desired

sauceSession.stop(true)
```
<!--C#-->
<br />

**C# bindings are coming soon...**

<!--END_DOCUSAURUS_CODE_TABS-->

___