---
layout: docLayout
---

<script>
	import { Textarea, Toolbar, ToolbarGroup, ToolbarButton, Button, Heading } from 'flowbite-svelte';
	import { MapPin, CodeBracket, PaperClip, Photo, FaceSmile, PaperAirplane } from 'svelte-heros-v2';
	import ExampleDiv from '../ExampleDiv.svelte';
</script>

<Heading class="mb-2" tag="h1" customSize="text-3xl">Textarea</Heading>

<ExampleDiv>
<form class="w-full">
	<label for="editor" class="sr-only">Publish post</label>
	<Textarea id="editor" rows="8" class="mb-4" placeholder="Write a comment">
		<Toolbar slot="header" embedded>
			<ToolbarGroup>
				<ToolbarButton name="Attach file">
					<PaperClip />
				</ToolbarButton>
				<ToolbarButton name="Embed map">
					<MapPin />
				</ToolbarButton>
				<ToolbarButton name="Upload image">
					<Photo />
				</ToolbarButton>
			</ToolbarGroup>
			<ToolbarGroup>
				<ToolbarButton name="Format code">
					<CodeBracket />
				</ToolbarButton>
				<ToolbarButton name="Add emoji">
					<FaceSmile />
				</ToolbarButton>
			</ToolbarGroup>
			<ToolbarButton name="send" slot="end">
				<PaperAirplane />
			</ToolbarButton>
		</Toolbar>
	</Textarea>
	<Button>Publish post</Button>
</form>
</ExampleDiv>

```html
<form class="w-full">
	<label for="editor" class="sr-only">Publish post</label>
	<Textarea id="editor" rows="8" class="mb-4" placeholder="Write a comment">
		<Toolbar slot="header" embedded>
			<ToolbarGroup>
				<ToolbarButton name="Attach file">
					<PaperClip />
				</ToolbarButton>
				<ToolbarButton name="Embed map">
					<MapPin />
				</ToolbarButton>
				<ToolbarButton name="Upload image">
					<Photo />
				</ToolbarButton>
			</ToolbarGroup>
			<ToolbarGroup>
				<ToolbarButton name="Format code">
					<CodeBracket />
				</ToolbarButton>
				<ToolbarButton name="Add emoji">
					<FaceSmile />
				</ToolbarButton>
			</ToolbarGroup>
			<ToolbarButton name="send" slot="end">
				<PaperAirplane />
			</ToolbarButton>
		</Toolbar>
	</Textarea>
	<Button>Publish post</Button>
</form>
```