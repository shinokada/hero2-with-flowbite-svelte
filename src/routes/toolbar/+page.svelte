<script>
	import { Toolbar, ToolbarButton, ToolbarGroup, Textarea, Button } from 'flowbite-svelte';
	import {
		QrCode,
		Envelope,
		Home,
		PaperClip,
		MapPin,
		FaceSmile,
		CodeBracket,
		Photo,
		PaperAirplane
	} from 'svelte-heros-v2';
</script>

<div class="p-8">
	<Toolbar>
		<ToolbarButton><Home /></ToolbarButton>
		<ToolbarButton><QrCode /></ToolbarButton>
		<ToolbarButton><Envelope /></ToolbarButton>
	</Toolbar>
</div>

<div class="p-8">
	<form>
		<label for="editor" class="sr-only">Publish post</label>
		<Textarea id="editor" rows="8" class="mb-4" placeholder="Write a comment">
			<Toolbar slot="header" embedded>
				<ToolbarGroup>
					<ToolbarButton name="Attach file"><PaperClip /></ToolbarButton>
					<ToolbarButton name="Embed map"><MapPin /></ToolbarButton>
					<ToolbarButton name="Upload image"><Photo /></ToolbarButton>
				</ToolbarGroup>
				<ToolbarGroup>
					<ToolbarButton name="Format code"><CodeBracket /></ToolbarButton>
					<ToolbarButton name="Add emoji"><FaceSmile /></ToolbarButton>
				</ToolbarGroup>
				<ToolbarButton name="send" slot="end"><PaperAirplane /></ToolbarButton>
			</Toolbar>
		</Textarea>
		<Button>Publish post</Button>
	</form>
</div>
