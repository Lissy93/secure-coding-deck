### There are several types of injection

- Allowing an attacker to execute operating system calls on a target machine
- Allowing an attacker to compromise backend data stores
- Allowing an attacker to compromise or hijack sessions of other users
- Allowing an attacker to force actions on behalf of other users or services

<aside class="notes">
Demo:
1. Go to login screen
2. Type: test’ OR 1=1;- -

Because the original query was: **`SELECT * from user_table WHERE user = ‘test’ AND pass = ‘pass’`**

But it was modified to be **`SELECT * from user_table WHERE user = ‘test’ OR 1=1;- — AND pass = ‘test’`**
</aside>
