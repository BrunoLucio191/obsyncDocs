---
title: Gene
kind: class
longname: module:backend/Server/Gene.Gene
description: The gene file is responsible for tracking the changes inside the vault. UpdateGene controls the whole flux when it comes to deal with the gene file generation - How many times the vault has changes. bytes - How many bytes the vault has. fileCount - The number of files inside the vault. lastModification - the date and hour from the last modification in ISO format Reads and updates go through their own queue, so an update never reads the file while another one is writing it, and initSync never gets a half-written gene.
---

# Gene

<SourceLink href="/source/backend/server/gene-ts/#L37" label="Gene.ts:37" />

The gene file is responsible for tracking the changes inside the vault. UpdateGene controls the whole flux when it comes to deal with the gene file

- `generation` - How many times the vault has changes.
- `bytes` - How many bytes the vault has.
- `fileCount` - The number of files inside the vault.
- `lastModification` - the date and hour from the last modification in ISO format

Reads and updates go through their own queue, so an update never reads the file while another one is writing it, and initSync never gets a half-written gene.

---

## Constructors

<MemberHeading
  id="constructor"
  depth="3"
  name="constructor"
  sig="new Gene(
	vaultDirectory: string,
	genePath: string,
	queueManager: QueueManager,
): Gene"
/>

**Parameters**

- `vaultDirectory` (string) — A valid vault directory
- `genePath` (string) — Path for the gene file
- `queueManager` (QueueManager) — Queue manager built with the server's shared KeyedLock

**Returns**

`Gene`

---

## Methods

<MemberHeading
  id="getbytesandnumoffiles"
  depth="3"
  name="getBytesAndNumOfFiles"
  sig="getBytesAndNumOfFiles(
	vaultDirectory: string,
): Promise<{ bytes: number; filesCount: number }>"
/>

<MemberMeta badges="async" sourceHref="/source/backend/server/gene-ts/#L130" sourceLabel="Gene.ts:130" />

returns the number of files and the byteSize from the whole vault, doesn't count empty files neither empty folders.

**Parameters**

- `vaultDirectory` (string)

**Returns**

- `Promise<{ bytes: number; filesCount: number }>`

<MemberHeading
  id="mutatevaultgene"
  depth="3"
  name="mutateVaultGene"
  sig="mutateVaultGene(
	directory: string,
	genePath: string,
): Promise<void>"
/>

<MemberMeta badges="async" sourceHref="/source/backend/server/gene-ts/#L162" sourceLabel="Gene.ts:162" />

update the gene file in a specific directory

**Parameters**

- `directory` (string, default: "...") — A valid directory
- `genePath` (string, default: "...") — Path for the gene file

**Returns**

- `Promise<void>`

<MemberHeading id="readgene" depth="3" name="readGene" sig="readGene(genePath: string): Promise<string>" />

<MemberMeta badges="async" sourceHref="/source/backend/server/gene-ts/#L197" sourceLabel="Gene.ts:197" />

Read in the gene queue, so it's never caught mid-update. `null` if missing or invalid.

**Parameters**

- `genePath` (string, default: "...")

**Returns**

- `Promise<string>`
