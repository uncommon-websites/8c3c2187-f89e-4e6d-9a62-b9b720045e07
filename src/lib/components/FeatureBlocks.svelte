<script lang="ts">
	import FeatureBlock from './FeatureBlock.svelte';
</script>

<!-- Block 1: Virtual Compute Acceleration -->
<FeatureBlock 
	title="Virtual Compute Acceleration" 
	description="Hardware-agnostic virtualization layer that delivers 3x AI throughput on any processor through algebraic memory optimization."
	buttons={[
		{ text: "TRY THE PLATFORM", icon: true },
		{ text: "READ TECHNICAL DOCS" }
	]}
>
	<div class="w-full h-full bg-white border border-border rounded shadow-sm p-4 font-mono text-xs">
		<div class="flex items-center gap-2 border-b border-border pb-2 mb-4">
			<span class="text-accent">○</span>
			<span class="text-muted">Virtual Compute Layer</span>
			<span class="w-2 h-4 bg-accent animate-pulse"></span>
		</div>
		<div class="space-y-3">
			<div class="flex items-center gap-2">
				<div class="w-16 text-[10px] text-muted">CPU</div>
				<div class="flex-1 h-2 bg-gray-100 rounded overflow-hidden">
					<div class="h-full bg-accent w-[90%]"></div>
				</div>
				<span class="text-[10px] text-accent">3x</span>
			</div>
			<div class="flex items-center gap-2">
				<div class="w-16 text-[10px] text-muted">Memory</div>
				<div class="flex-1 h-2 bg-gray-100 rounded overflow-hidden">
					<div class="h-full bg-primary-400 w-[60%]"></div>
				</div>
				<span class="text-[10px] text-muted">-40%</span>
			</div>
			<div class="flex items-center gap-2">
				<div class="w-16 text-[10px] text-muted">Energy</div>
				<div class="flex-1 h-2 bg-gray-100 rounded overflow-hidden">
					<div class="h-full bg-green-500 w-[33%]"></div>
				</div>
				<span class="text-[10px] text-green-600">-66%</span>
			</div>
		</div>
	</div>
</FeatureBlock>

<!-- Block 2: Atlas Mathematical Framework -->
<FeatureBlock 
	title="Atlas Mathematical Framework" 
	description="Breakthrough algebraic system converting byte-level operations into precomputed, constant-time memory lookups for O(1) computation."
	buttons={[
		{ text: "EXPLORE FRAMEWORK", icon: true }
	]}
	alignRight={true}
>
	<div class="w-full max-w-md bg-white border border-border rounded shadow-sm p-6 flex flex-col gap-4">
		<div class="flex items-center gap-2 text-xs font-mono text-muted">
			<div class="w-4 h-4 border border-current rounded-sm flex items-center justify-center">
				<div class="w-2 h-2 bg-current rounded-[1px]"></div>
			</div>
			Constant-time computation
		</div>
		<div class="grid grid-cols-3 gap-2 text-center text-[10px] font-mono">
			<div class="border border-border p-2 rounded">
				<div class="text-muted mb-1">Traditional</div>
				<div class="text-lg font-bold">O(n)</div>
			</div>
			<div class="border border-accent bg-accent/5 p-2 rounded">
				<div class="text-accent mb-1">Atlas</div>
				<div class="text-lg font-bold text-accent">O(1)</div>
			</div>
			<div class="border border-border p-2 rounded">
				<div class="text-muted mb-1">Speedup</div>
				<div class="text-lg font-bold text-green-600">3x</div>
			</div>
		</div>
		<div class="flex gap-1 mt-2">
			{#each Array(20) as _, i}
				<div class="w-1 h-3 {i < 7 ? 'bg-accent' : 'bg-gray-200'}"></div>
			{/each}
		</div>
		<div class="mt-2 flex items-center gap-2 text-[10px] text-accent font-mono uppercase">
			<span class="w-3 h-3 border border-current rounded-full flex items-center justify-center">✓</span>
			MATHEMATICAL PROOF VERIFIED
		</div>
	</div>
</FeatureBlock>

<!-- Block 3: Cross-Platform Deployment -->
<FeatureBlock 
	title="Cross-Platform Deployment" 
	description="Universal compute layer runs on Windows, Linux, macOS, Android, iOS, and edge devices—no hardware upgrades needed."
	buttons={[
		{ text: "VIEW COMPATIBILITY", icon: true }
	]}
>
	<div class="w-full h-full bg-white border border-border rounded shadow-sm overflow-hidden font-mono text-[10px]">
		<div class="grid grid-cols-4 gap-2 p-2 border-b border-border bg-gray-50 text-muted">
			<div>PLATFORM</div>
			<div>STATUS</div>
			<div>THROUGHPUT</div>
			<div>ENERGY</div>
		</div>
		{#each [
			{ name: 'Linux x86', status: 'active' },
			{ name: 'Windows', status: 'active' },
			{ name: 'macOS ARM', status: 'active' },
			{ name: 'Android', status: 'active' },
			{ name: 'iOS', status: 'active' },
			{ name: 'Edge Device', status: 'active' }
		] as platform, i}
			<div class="grid grid-cols-4 gap-2 p-2 border-b border-border/50 items-center">
				<div class="flex items-center gap-2">
					<div class="w-2 h-2 rounded-full bg-green-500"></div>
					<span>{platform.name}</span>
				</div>
				<div class="text-green-600">Ready</div>
				<div class="text-accent">+3x</div>
				<div class="text-green-600">-66%</div>
			</div>
		{/each}
	</div>
</FeatureBlock>

<!-- Block 4: Enterprise-Grade Security -->
<FeatureBlock 
	title="Enterprise-Grade Security" 
	description="Air-gapped deployment, compliance-ready architecture, and verifiable computation with mathematical proofs for regulated industries."
	buttons={[
		{ text: "SECURITY OVERVIEW", icon: true }
	]}
	alignRight={true}
>
	<div class="w-full h-full bg-white border border-border rounded shadow-sm overflow-hidden font-mono text-[10px]">
		<div class="grid grid-cols-4 gap-2 p-2 border-b border-border bg-gray-50 text-muted">
			<div>FEATURE</div>
			<div>STATUS</div>
			<div>COMPLIANCE</div>
			<div>VERIFIED</div>
		</div>
		{#each [
			{ name: 'Air-Gapped', comp: 'DoD' },
			{ name: 'Encrypted', comp: 'NIST' },
			{ name: 'Verifiable', comp: 'SOC 2' },
			{ name: 'Isolated', comp: 'FedRAMP' },
			{ name: 'Auditable', comp: 'ISO 27001' },
			{ name: 'Private', comp: 'GDPR' }
		] as feature, i}
			<div class="grid grid-cols-4 gap-2 p-2 border-b border-border/50 items-center">
				<div class="flex items-center gap-2">
					<div class="w-2 h-2 rounded-sm bg-green-500"></div>
					<span>{feature.name}</span>
				</div>
				<div class="text-green-600">Active</div>
				<div class="text-blue-600">{feature.comp}</div>
				<div class="text-accent">✓</div>
			</div>
		{/each}
	</div>
</FeatureBlock>

<!-- Block 5: Developer Experience -->
<FeatureBlock 
	title="Developer Experience" 
	description="One-click kernel spin-up, one-command compilation from Python/TypeScript to native code. No learning curve required."
	buttons={[
		{ text: "START BUILDING", icon: true }
	]}
>
	<div class="w-full h-full bg-black text-green-400 border border-border rounded shadow-sm p-4 flex flex-col gap-3 font-mono text-[10px]">
		<div class="flex items-center gap-2 text-white/60">
			<span>$</span>
			<span class="text-white">hologram init</span>
		</div>
		
		<div class="space-y-1 text-white/40">
			<div>✓ Initializing virtual compute layer...</div>
			<div>✓ Loading Atlas framework...</div>
			<div>✓ Optimizing memory mappings...</div>
			<div class="text-green-400">✓ Ready for deployment</div>
		</div>

		<div class="mt-2 flex items-center gap-2 text-white/60 border-t border-white/10 pt-3">
			<span>$</span>
			<span class="text-white">hologram compile model.py</span>
		</div>

		<div class="space-y-1 text-white/40">
			<div>→ Compiling to native code...</div>
			<div class="text-accent">→ 3x performance gain detected</div>
			<div class="text-green-400">✓ Build complete: 847ms</div>
		</div>

		<div class="mt-auto flex items-center gap-2 text-[9px] text-white/30">
			<span class="w-2 h-2 bg-green-500 rounded-full animate-pulse"></span>
			Virtual compute active
		</div>
	</div>
</FeatureBlock>
