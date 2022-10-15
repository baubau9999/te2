@shift /0
@echo off
mode 80,25
title Baubau
color b
set load=
set/a loadnum=

:loading
set load=%load%Û
cls
echo.
echo  [! baubau.pro !]
timeout 2 >nul
echo  [! LOADING !]
timeout 2 >nul
ping localhost -n 3 >nul
set/a loadnum=%loadnum% +1
if %loadnum%==1 goto done

goto loading
:done
echo.
echo loading complete
:login
cls
mode 80,27
color b 
title Baubau
chcp 65001
cls
color b                                               
echo.        __         __  __          __        
echo        / /   /\ /\ \ \/ / /\ /\   /__\ /\_/\ 
echo       / /   / / \ \ \  / / / \ \ / \// \_ _/ 
echo      / /___ \ \_/ / /  \ \ \_/ // _  \  / \  
echo      \____/  \___/ /_/\_\ \___/ \/ \_/  \_/  
echo                 __    ___    _        __
echo      /\ /\   /\ \ \  / __\  /_\    /\ \ \
echo     / / \ \ /  \/ / /__\// //_\\  /  \/ /
echo     \ \_/ // /\  / / \/  \/  _  \/ /\  / 
echo      \___/ \_\ \/  \_____/\_/ \_/\_\ \/  
echo.
echo    ____________________________________________
echo     Cảm ơn bạn đã sử dụng
echo     Nếu bạn có bất kỳ câu hỏi hoặc lỗi nào
echo     hãy mở ticket!
echo    ____________________________________________
echo.
echo [?] Đăng nhập tài khoản
set /p user=Username : 
echo.                                                                                                                        
set /p pass=Password : 
if %user% == baubau if %pass% == tntv2007 goto main
if %user% == 1 if %pass% == 1 goto main

echo Sai mật khẩu hoặc tài khoản
timeout 5 >nul
goto login
echo Version 2
:main
cls
echo welcome %Luxury%
cls
mode 80,27
title Baubau
color b



echo         ________________________________________
echo        [________________________________________]
echo        [       [!] BAUBAU.PRO [!]               ]
echo        [________________________________________]
echo        [                                        ]
echo        [       [1] Config     [2] Client        ]
echo        [                [3] Other               ]
echo        [        [4] LINK DISCORD                ]
echo        [________________________________________]
echo.
echo.
set /p key=Select : 
if %key%==1 goto config                            
if %key%==2 goto xbox
if %key%==3 goto other
if %key%==4 goto discord
echo.
echo.   


:test
cls
echo.
echo [!] Vui lòng đợi 3s  
timeout 3>nul
xcopy "C:\Users\bau\Desktop\test\cc\copy\1.txt" "C:\Users\bau\Desktop\test\cc\1" /y
cls
echo done
timeout 3>nul
goto main

:xbox
cls 
echo.
echo ccc
del /q /s /f "C:\Users\bau\Desktop\test\cc\ccc"
cls


:config
cls
echo         ________________________________________
echo        [________________________________________]
echo        [       [!] BAUBAU.PRO [!]               ]
echo        [________________________________________]
echo        [                                        ]
echo        [ [1] bed                                ]
echo        [ [2] sky                                ]
echo        [ [1] the                                ]
echo        [ [999] back                            ]
echo        [________________________________________]
echo.
echo.
set /p key=Select : 
if %key%==1 goto bed                            
if %key%==2 goto xbox
if %key%==3 goto discord
if %key%==999 goto main
echo.
echo.  


:bed
start https://baubau.pro











:other
cls
echo         ________________________________________
echo        [________________________________________]
echo        [       [!] BAUBAU.PRO [!]               ]
echo        [________________________________________]
echo        [                                        ]
echo        [ [1] unfollow                           ]
echo        [ [999] back                             ]
echo        [________________________________________]
echo.
echo.
set /p key=Select : 
if %key%==1 goto unfollow                            
if %key%==999 goto main
echo.
echo.  


:unfollow
start https://tinyurl.com/2gq485b8







