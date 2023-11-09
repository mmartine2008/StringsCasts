unit StringsCasts;

interface

function CastAnsiCharArrayToWideChar(const AnsiArray: array of AnsiChar): PWideChar;
function CastWideCharToAnsiChar(const wideStr: PWideChar): PAnsiChar;

implementation

function CastAnsiCharArrayToWideChar(const AnsiArray: array of AnsiChar): PWideChar;
var
  AnsiStr: AnsiString;
  WideStr: WideString;
begin
  // Convert the array of AnsiChar to an AnsiString
  AnsiStr := AnsiString(AnsiArray);

  // Convert the AnsiString to WideString
  WideStr := WideString(AnsiStr);

  // Get the PWideChar from the WideString
  Result := PWideChar(WideStr);
end;


function CastWideCharToAnsiChar(const wideStr: PWideChar): PAnsiChar;
var
  ansiStr: AnsiString;
begin
  // Convert the PWideChar to an AnsiString
  ansiStr := AnsiString(wideStr);

  // Convert the AnsiString to PAnsiChar
  Result := PAnsiChar(ansiStr);
end;

end.
