<script>
	export let id;
	export let lines;
	export let noescape;
</script>

<pre data-id={id}>
<code data-trim data-line-number={lines || null} data-noescape={noescape || null}>
    <slot />
</code>
</pre>
