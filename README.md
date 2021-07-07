# Base1

//
// function.yaml:
// spec:
// runtime: dotnetcore

public class test
{
public string reverser(Context context, Event eventBase)
{
var charArray = eventBase.GetBody().ToCharArray();
Array.Reverse(charArray);
return new string(charArray);
}
}
