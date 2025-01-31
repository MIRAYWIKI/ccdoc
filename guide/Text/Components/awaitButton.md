# $awaitButton
Wait a button to be pressed and return its button Id, or `undefined` in case of no button pressed until the timeout.
::: tip This function supports message curl format
That way, you can send a message with buttons by using `{button:label:style/url:emoji:id:newline(yes/no)}`
:::

#### Usage: `$awaitButton[Message (optional);user id (optional, default:author);timeout (optional, default:15s);button id1 (optional);button id2...]`
<br/>
::: details Examples

(Simple response)

![](https://cdn.discordapp.com/attachments/914682255346118687/938556903116652594/Screenshot_20220202190956.jpg)

(Usage example)
```
$let[PressedButton;$awaitbutton[Which color is my favorite?
{button:Green:GREEN::green}
{button:Blue:BLUE::blue}
{button:Red:RED::red};$authorid;15s;red;blue;green]]
/* Saves the pressed button id in a temporary var, so you can retrieve later */

$if[$get[PressedButton]!=red]
Wrong!
$else
Correct!
$endif
/* If the button id is different from red, which is the right answer, them incorrect. Else, correct. */
```
choosing something other them red, or nothing.
![](https://cdn.discordapp.com/attachments/914682255346118687/938559970293714984/Screenshot_20220202191954.jpg)

choosing red.

![](https://cdn.discordapp.com/attachments/914682255346118687/938559970792845312/Screenshot_20220202191947.jpg)
:::


##### Function Difficultly: <Badge type="warning" text="Medium" vertical="middle" /> 
###### Tags: <Badge type="tip" text="await" vertical="middle" /> <Badge type="tip" text="button" vertical="middle" /> <Badge type="tip" text="interaction" vertical="middle" /> <Badge type="tip" text="click" vertical="middle" />
