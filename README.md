# SetError
Func _IsInternetConnected()     Local $aReturn = DllCall('connect.dll', 'long', 'IsInternetConnected')     If @error Then         Return SetError(1, 0, False)     EndIf     Return $aReturn[0] = 0
