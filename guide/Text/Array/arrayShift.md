# $arrayShift
Remove and return the first element in the splitted array by `$textsplit`

#### Usage: `$arrayShift`
::: warning 
Return element value or undefined if no element in the array
:::

<br/>
<discord-messages>
	<discord-message :bot="false" role-color="#ffcc9a" author="Member">
		!!exec $textSplit[Rake Mido; ] {{ '\n' }} $arrayShift
	</discord-message>
	<discord-message :bot="true" role-color="#0099ff" author="Custom Command" avatar="https://media.discordapp.net/avatars/725721249652670555/781224f90c3b841ba5b40678e032f74a.webp">
		Rake /* Now the array only have Mido */
	</discord-message>
</discord-messages>

##### Function Difficultly: <Badge type="tip" text="Easy" vertical="middle" /> 
###### Tags: <Badge type="tip" text="array" vertical="middle" /> <Badge type="tip" text="shift" vertical="middle" /> <Badge type="tip" text="textsplit" vertical="middle" /> <Badge type="tip" text="remove" vertical="middle" />