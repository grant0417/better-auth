<script lang="ts">
import { Button as ButtonPrimitive } from "bits-ui";
import { buttonVariants, type Events, type Props } from "./index.js";
import { cn } from "$lib/utils.js";

type $$Props = Props;
type $$Events = Events;

let className: $$Props["class"] = undefined;
export let variant: $$Props["variant"] = "default";
export let size: $$Props["size"] = "default";
export let builders: $$Props["builders"] = [];
export { className as class };
</script>

<ButtonPrimitive.Root
	{builders}
	class={cn(buttonVariants({ variant, size, className }))}
	type="button"
	{...$$restProps}
	on:click
	on:keydown
>
	<slot />
</ButtonPrimitive.Root>
