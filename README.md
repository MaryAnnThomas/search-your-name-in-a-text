# search-your-name-in-a-text
var text = "Hey,how are you \
doing ?My name is emily.";
var myName = "emily";
var hits = [];
for(var i=0;i<text.length;i++)
{
    if(text[i] === "e")
    {
        for(var j=i;j<(myName.length +i);j++)
        {
           hits.push(text[j]); 
        }
    }
}
if(hits.length === 0)
{
    console.log("Your name not found");
}
else
{
    console.log(hits);
}
