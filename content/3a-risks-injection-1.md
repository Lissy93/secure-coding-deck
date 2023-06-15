This is where a user input is not sanitized before being sent to the server, or appended to the database. This allows an attacker to insert malicious code, which is then executed, leading to unexpected or harmful results.

<img style="margin: 0 auto; display: flex;" src="/assets/pictures/sql-injection.svg" />

<aside class="notes">
  Injection has been number 1 on the OWASP top 10 list since 2010. It should still not be considered a "solved" problem.

  The 2011 Sony Playstation breach was caused by a simple SQL injection.
  It resulted in 77 million user accounts being compromised, and cost Sony
  $171 million, along with nearly a month of downtime.
</aside>
