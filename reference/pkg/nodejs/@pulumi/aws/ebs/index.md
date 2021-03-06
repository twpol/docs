---
title: Module ebs
---

<a href="../index.html">@pulumi/aws</a> &gt; ebs

<h2 class="pdoc-module-header">Index</h2>

* <a href="#Snapshot">class Snapshot</a>
* <a href="#Volume">class Volume</a>
* <a href="#getSnapshot">function getSnapshot</a>
* <a href="#getSnapshotIds">function getSnapshotIds</a>
* <a href="#getVolume">function getVolume</a>
* <a href="#GetSnapshotArgs">interface GetSnapshotArgs</a>
* <a href="#GetSnapshotIdsArgs">interface GetSnapshotIdsArgs</a>
* <a href="#GetSnapshotIdsResult">interface GetSnapshotIdsResult</a>
* <a href="#GetSnapshotResult">interface GetSnapshotResult</a>
* <a href="#GetVolumeArgs">interface GetVolumeArgs</a>
* <a href="#GetVolumeResult">interface GetVolumeResult</a>
* <a href="#SnapshotArgs">interface SnapshotArgs</a>
* <a href="#SnapshotState">interface SnapshotState</a>
* <a href="#VolumeArgs">interface VolumeArgs</a>
* <a href="#VolumeState">interface VolumeState</a>

<a href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getSnapshot.ts">ebs/getSnapshot.ts</a> <a href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getSnapshotIds.ts">ebs/getSnapshotIds.ts</a> <a href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getVolume.ts">ebs/getVolume.ts</a> <a href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/snapshot.ts">ebs/snapshot.ts</a> <a href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/volume.ts">ebs/volume.ts</a> 


<h2 class="pdoc-module-header" id="Snapshot">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/snapshot.ts#L9">class Snapshot</a>
</h2>

Creates a Snapshot of an EBS Volume.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/snapshot.ts#L57">constructor</a>
</h3>

```typescript
new Snapshot(name: string, args: SnapshotArgs, opts?: pulumi.ResourceOptions)
```


Create a Snapshot resource with the given unique name, arguments, and options.

* `name` The _unique_ name of the resource.
* `args` The arguments to use to populate this resource&#39;s properties.
* `opts` A bag of options that control this resource&#39;s behavior.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/snapshot.ts#L18">method get</a>
</h3>

```typescript
public static get(name: string, id: pulumi.Input<pulumi.ID>, state?: SnapshotState): Snapshot
```


Get an existing Snapshot resource's state with the given name, ID, and optional extra
properties used to qualify the lookup.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L64">method isInstance</a>
</h3>

```typescript
static isInstance(obj: any): boolean
```


Returns true if the given object is an instance of CustomResource.  This is designed to work even when
multiple copies of the Pulumi SDK have been loaded into the same process.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/snapshot.ts#L25">property dataEncryptionKeyId</a>
</h3>

```typescript
public dataEncryptionKeyId: pulumi.Output<string>;
```


The data encryption key identifier for the snapshot.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/snapshot.ts#L29">property description</a>
</h3>

```typescript
public description: pulumi.Output<string | undefined>;
```


A description of what the snapshot is.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/snapshot.ts#L33">property encrypted</a>
</h3>

```typescript
public encrypted: pulumi.Output<boolean>;
```


Whether the snapshot is encrypted.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L59">property id</a>
</h3>

```typescript
id: Output<ID>;
```


id is the provider-assigned unique ID for this managed resource.  It is set during
deployments and may be missing (undefined) during planning phases.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/snapshot.ts#L37">property kmsKeyId</a>
</h3>

```typescript
public kmsKeyId: pulumi.Output<string>;
```


The ARN for the KMS encryption key.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/snapshot.ts#L41">property ownerAlias</a>
</h3>

```typescript
public ownerAlias: pulumi.Output<string>;
```


Value from an Amazon-maintained list (`amazon`, `aws-marketplace`, `microsoft`) of snapshot owners.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/snapshot.ts#L45">property ownerId</a>
</h3>

```typescript
public ownerId: pulumi.Output<string>;
```


The AWS account ID of the EBS snapshot owner.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/snapshot.ts#L49">property tags</a>
</h3>

```typescript
public tags: pulumi.Output<{ ... } | undefined>;
```


A mapping of tags to assign to the snapshot

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L11">property urn</a>
</h3>

```typescript
urn: Output<URN>;
```


urn is the stable logical URN used to distinctly address a resource, both before and after
deployments.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/snapshot.ts#L53">property volumeId</a>
</h3>

```typescript
public volumeId: pulumi.Output<string>;
```


The Volume ID of which to make a snapshot.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/snapshot.ts#L57">property volumeSize</a>
</h3>

```typescript
public volumeSize: pulumi.Output<number>;
```


The size of the drive in GiBs.

<h2 class="pdoc-module-header" id="Volume">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/volume.ts#L9">class Volume</a>
</h2>

Manages a single EBS volume.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/volume.ts#L57">constructor</a>
</h3>

```typescript
new Volume(name: string, args: VolumeArgs, opts?: pulumi.ResourceOptions)
```


Create a Volume resource with the given unique name, arguments, and options.

* `name` The _unique_ name of the resource.
* `args` The arguments to use to populate this resource&#39;s properties.
* `opts` A bag of options that control this resource&#39;s behavior.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/volume.ts#L18">method get</a>
</h3>

```typescript
public static get(name: string, id: pulumi.Input<pulumi.ID>, state?: VolumeState): Volume
```


Get an existing Volume resource's state with the given name, ID, and optional extra
properties used to qualify the lookup.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L64">method isInstance</a>
</h3>

```typescript
static isInstance(obj: any): boolean
```


Returns true if the given object is an instance of CustomResource.  This is designed to work even when
multiple copies of the Pulumi SDK have been loaded into the same process.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/volume.ts#L25">property arn</a>
</h3>

```typescript
public arn: pulumi.Output<string>;
```


The volume ARN (e.g. arn:aws:ec2:us-east-1:0123456789012:volume/vol-59fcb34e).

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/volume.ts#L29">property availabilityZone</a>
</h3>

```typescript
public availabilityZone: pulumi.Output<string>;
```


The AZ where the EBS volume will exist.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/volume.ts#L33">property encrypted</a>
</h3>

```typescript
public encrypted: pulumi.Output<boolean>;
```


If true, the disk will be encrypted.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L59">property id</a>
</h3>

```typescript
id: Output<ID>;
```


id is the provider-assigned unique ID for this managed resource.  It is set during
deployments and may be missing (undefined) during planning phases.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/volume.ts#L37">property iops</a>
</h3>

```typescript
public iops: pulumi.Output<number>;
```


The amount of IOPS to provision for the disk.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/volume.ts#L41">property kmsKeyId</a>
</h3>

```typescript
public kmsKeyId: pulumi.Output<string>;
```


The ARN for the KMS encryption key. When specifying `kms_key_id`, `encrypted` needs to be set to true.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/volume.ts#L45">property size</a>
</h3>

```typescript
public size: pulumi.Output<number>;
```


The size of the drive in GiBs.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/volume.ts#L49">property snapshotId</a>
</h3>

```typescript
public snapshotId: pulumi.Output<string>;
```


A snapshot to base the EBS volume off of.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/volume.ts#L53">property tags</a>
</h3>

```typescript
public tags: pulumi.Output<{ ... } | undefined>;
```


A mapping of tags to assign to the resource.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/volume.ts#L57">property type</a>
</h3>

```typescript
public type: pulumi.Output<string>;
```


The type of EBS volume. Can be "standard", "gp2", "io1", "sc1" or "st1" (Default: "standard").

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/node_modules/@pulumi/pulumi/resource.d.ts#L11">property urn</a>
</h3>

```typescript
urn: Output<URN>;
```


urn is the stable logical URN used to distinctly address a resource, both before and after
deployments.

<h2 class="pdoc-module-header" id="getSnapshot">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getSnapshot.ts#L9">function getSnapshot</a>
</h2>

```typescript
getSnapshot(args?: GetSnapshotArgs): Promise<GetSnapshotResult>
```


Use this data source to get information about an EBS Snapshot for use when provisioning EBS Volumes

<h2 class="pdoc-module-header" id="getSnapshotIds">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getSnapshotIds.ts#L10">function getSnapshotIds</a>
</h2>

```typescript
getSnapshotIds(args?: GetSnapshotIdsArgs): Promise<GetSnapshotIdsResult>
```


Use this data source to get a list of EBS Snapshot IDs matching the specified
criteria.

<h2 class="pdoc-module-header" id="getVolume">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getVolume.ts#L10">function getVolume</a>
</h2>

```typescript
getVolume(args?: GetVolumeArgs): Promise<GetVolumeResult>
```


Use this data source to get information about an EBS volume for use in other
resources.

<h2 class="pdoc-module-header" id="GetSnapshotArgs">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getSnapshot.ts#L24">interface GetSnapshotArgs</a>
</h2>

A collection of arguments for invoking getSnapshot.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getSnapshot.ts#L30">property filters</a>
</h3>

```typescript
filters?: pulumi.Input<{ ... }[]>;
```


One or more name/value pairs to filter off of. There are
several valid keys, for a full reference, check out
[describe-snapshots in the AWS CLI reference][1].

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getSnapshot.ts#L34">property mostRecent</a>
</h3>

```typescript
mostRecent?: pulumi.Input<boolean>;
```


If more than one result is returned, use the most recent snapshot.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getSnapshot.ts#L38">property owners</a>
</h3>

```typescript
owners?: pulumi.Input<pulumi.Input<string>[]>;
```


Returns the snapshots owned by the specified owner id. Multiple owners can be specified.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getSnapshot.ts#L42">property restorableByUserIds</a>
</h3>

```typescript
restorableByUserIds?: pulumi.Input<pulumi.Input<string>[]>;
```


One or more AWS accounts IDs that can create volumes from the snapshot.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getSnapshot.ts#L46">property snapshotIds</a>
</h3>

```typescript
snapshotIds?: pulumi.Input<pulumi.Input<string>[]>;
```


Returns information on a specific snapshot_id.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getSnapshot.ts#L47">property tags</a>
</h3>

```typescript
tags?: pulumi.Input<{ ... }>;
```

<h2 class="pdoc-module-header" id="GetSnapshotIdsArgs">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getSnapshotIds.ts#L22">interface GetSnapshotIdsArgs</a>
</h2>

A collection of arguments for invoking getSnapshotIds.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getSnapshotIds.ts#L28">property filters</a>
</h3>

```typescript
filters?: pulumi.Input<{ ... }[]>;
```


One or more name/value pairs to filter off of. There are
several valid keys, for a full reference, check out
[describe-volumes in the AWS CLI reference][1].

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getSnapshotIds.ts#L32">property owners</a>
</h3>

```typescript
owners?: pulumi.Input<pulumi.Input<string>[]>;
```


Returns the snapshots owned by the specified owner id. Multiple owners can be specified.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getSnapshotIds.ts#L36">property restorableByUserIds</a>
</h3>

```typescript
restorableByUserIds?: pulumi.Input<pulumi.Input<string>[]>;
```


One or more AWS accounts IDs that can create volumes from the snapshot.

<h2 class="pdoc-module-header" id="GetSnapshotIdsResult">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getSnapshotIds.ts#L42">interface GetSnapshotIdsResult</a>
</h2>

A collection of values returned by getSnapshotIds.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getSnapshotIds.ts#L43">property ids</a>
</h3>

```typescript
ids: string[];
```

<h2 class="pdoc-module-header" id="GetSnapshotResult">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getSnapshot.ts#L53">interface GetSnapshotResult</a>
</h2>

A collection of values returned by getSnapshot.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getSnapshot.ts#L57">property dataEncryptionKeyId</a>
</h3>

```typescript
dataEncryptionKeyId: string;
```


The data encryption key identifier for the snapshot.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getSnapshot.ts#L61">property description</a>
</h3>

```typescript
description: string;
```


A description for the snapshot

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getSnapshot.ts#L65">property encrypted</a>
</h3>

```typescript
encrypted: boolean;
```


Whether the snapshot is encrypted.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getSnapshot.ts#L69">property kmsKeyId</a>
</h3>

```typescript
kmsKeyId: string;
```


The ARN for the KMS encryption key.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getSnapshot.ts#L73">property ownerAlias</a>
</h3>

```typescript
ownerAlias: string;
```


Value from an Amazon-maintained list (`amazon`, `aws-marketplace`, `microsoft`) of snapshot owners.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getSnapshot.ts#L77">property ownerId</a>
</h3>

```typescript
ownerId: string;
```


The AWS account ID of the EBS snapshot owner.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getSnapshot.ts#L81">property snapshotId</a>
</h3>

```typescript
snapshotId: string;
```


The snapshot ID (e.g. snap-59fcb34e).

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getSnapshot.ts#L85">property state</a>
</h3>

```typescript
state: string;
```


The snapshot state.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getSnapshot.ts#L89">property tags</a>
</h3>

```typescript
tags: { ... };
```


A mapping of tags for the resource.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getSnapshot.ts#L93">property volumeId</a>
</h3>

```typescript
volumeId: string;
```


The volume ID (e.g. vol-59fcb34e).

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getSnapshot.ts#L97">property volumeSize</a>
</h3>

```typescript
volumeSize: number;
```


The size of the drive in GiBs.

<h2 class="pdoc-module-header" id="GetVolumeArgs">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getVolume.ts#L22">interface GetVolumeArgs</a>
</h2>

A collection of arguments for invoking getVolume.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getVolume.ts#L28">property filters</a>
</h3>

```typescript
filters?: pulumi.Input<{ ... }[]>;
```


One or more name/value pairs to filter off of. There are
several valid keys, for a full reference, check out
[describe-volumes in the AWS CLI reference][1].

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getVolume.ts#L33">property mostRecent</a>
</h3>

```typescript
mostRecent?: pulumi.Input<boolean>;
```


If more than one result is returned, use the most
recent Volume.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getVolume.ts#L34">property tags</a>
</h3>

```typescript
tags?: pulumi.Input<{ ... }>;
```

<h2 class="pdoc-module-header" id="GetVolumeResult">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getVolume.ts#L40">interface GetVolumeResult</a>
</h2>

A collection of values returned by getVolume.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getVolume.ts#L44">property arn</a>
</h3>

```typescript
arn: string;
```


The volume ARN (e.g. arn:aws:ec2:us-east-1:0123456789012:volume/vol-59fcb34e).

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getVolume.ts#L48">property availabilityZone</a>
</h3>

```typescript
availabilityZone: string;
```


The AZ where the EBS volume exists.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getVolume.ts#L52">property encrypted</a>
</h3>

```typescript
encrypted: boolean;
```


Whether the disk is encrypted.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getVolume.ts#L56">property iops</a>
</h3>

```typescript
iops: number;
```


The amount of IOPS for the disk.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getVolume.ts#L60">property kmsKeyId</a>
</h3>

```typescript
kmsKeyId: string;
```


The ARN for the KMS encryption key.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getVolume.ts#L64">property size</a>
</h3>

```typescript
size: number;
```


The size of the drive in GiBs.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getVolume.ts#L68">property snapshotId</a>
</h3>

```typescript
snapshotId: string;
```


The snapshot_id the EBS volume is based off.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getVolume.ts#L72">property tags</a>
</h3>

```typescript
tags: { ... };
```


A mapping of tags for the resource.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getVolume.ts#L76">property volumeId</a>
</h3>

```typescript
volumeId: string;
```


The volume ID (e.g. vol-59fcb34e).

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/getVolume.ts#L80">property volumeType</a>
</h3>

```typescript
volumeType: string;
```


The type of EBS volume.

<h2 class="pdoc-module-header" id="SnapshotArgs">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/snapshot.ts#L144">interface SnapshotArgs</a>
</h2>

The set of arguments for constructing a Snapshot resource.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/snapshot.ts#L148">property description</a>
</h3>

```typescript
description?: pulumi.Input<string>;
```


A description of what the snapshot is.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/snapshot.ts#L152">property tags</a>
</h3>

```typescript
tags?: pulumi.Input<{ ... }>;
```


A mapping of tags to assign to the snapshot

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/snapshot.ts#L156">property volumeId</a>
</h3>

```typescript
volumeId: pulumi.Input<string>;
```


The Volume ID of which to make a snapshot.

<h2 class="pdoc-module-header" id="SnapshotState">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/snapshot.ts#L102">interface SnapshotState</a>
</h2>

Input properties used for looking up and filtering Snapshot resources.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/snapshot.ts#L106">property dataEncryptionKeyId</a>
</h3>

```typescript
dataEncryptionKeyId?: pulumi.Input<string>;
```


The data encryption key identifier for the snapshot.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/snapshot.ts#L110">property description</a>
</h3>

```typescript
description?: pulumi.Input<string>;
```


A description of what the snapshot is.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/snapshot.ts#L114">property encrypted</a>
</h3>

```typescript
encrypted?: pulumi.Input<boolean>;
```


Whether the snapshot is encrypted.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/snapshot.ts#L118">property kmsKeyId</a>
</h3>

```typescript
kmsKeyId?: pulumi.Input<string>;
```


The ARN for the KMS encryption key.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/snapshot.ts#L122">property ownerAlias</a>
</h3>

```typescript
ownerAlias?: pulumi.Input<string>;
```


Value from an Amazon-maintained list (`amazon`, `aws-marketplace`, `microsoft`) of snapshot owners.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/snapshot.ts#L126">property ownerId</a>
</h3>

```typescript
ownerId?: pulumi.Input<string>;
```


The AWS account ID of the EBS snapshot owner.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/snapshot.ts#L130">property tags</a>
</h3>

```typescript
tags?: pulumi.Input<{ ... }>;
```


A mapping of tags to assign to the snapshot

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/snapshot.ts#L134">property volumeId</a>
</h3>

```typescript
volumeId?: pulumi.Input<string>;
```


The Volume ID of which to make a snapshot.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/snapshot.ts#L138">property volumeSize</a>
</h3>

```typescript
volumeSize?: pulumi.Input<number>;
```


The size of the drive in GiBs.

<h2 class="pdoc-module-header" id="VolumeArgs">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/volume.ts#L144">interface VolumeArgs</a>
</h2>

The set of arguments for constructing a Volume resource.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/volume.ts#L148">property availabilityZone</a>
</h3>

```typescript
availabilityZone: pulumi.Input<string>;
```


The AZ where the EBS volume will exist.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/volume.ts#L152">property encrypted</a>
</h3>

```typescript
encrypted?: pulumi.Input<boolean>;
```


If true, the disk will be encrypted.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/volume.ts#L156">property iops</a>
</h3>

```typescript
iops?: pulumi.Input<number>;
```


The amount of IOPS to provision for the disk.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/volume.ts#L160">property kmsKeyId</a>
</h3>

```typescript
kmsKeyId?: pulumi.Input<string>;
```


The ARN for the KMS encryption key. When specifying `kms_key_id`, `encrypted` needs to be set to true.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/volume.ts#L164">property size</a>
</h3>

```typescript
size?: pulumi.Input<number>;
```


The size of the drive in GiBs.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/volume.ts#L168">property snapshotId</a>
</h3>

```typescript
snapshotId?: pulumi.Input<string>;
```


A snapshot to base the EBS volume off of.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/volume.ts#L172">property tags</a>
</h3>

```typescript
tags?: pulumi.Input<{ ... }>;
```


A mapping of tags to assign to the resource.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/volume.ts#L176">property type</a>
</h3>

```typescript
type?: pulumi.Input<string>;
```


The type of EBS volume. Can be "standard", "gp2", "io1", "sc1" or "st1" (Default: "standard").

<h2 class="pdoc-module-header" id="VolumeState">
<a class="pdoc-member-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/volume.ts#L102">interface VolumeState</a>
</h2>

Input properties used for looking up and filtering Volume resources.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/volume.ts#L106">property arn</a>
</h3>

```typescript
arn?: pulumi.Input<string>;
```


The volume ARN (e.g. arn:aws:ec2:us-east-1:0123456789012:volume/vol-59fcb34e).

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/volume.ts#L110">property availabilityZone</a>
</h3>

```typescript
availabilityZone?: pulumi.Input<string>;
```


The AZ where the EBS volume will exist.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/volume.ts#L114">property encrypted</a>
</h3>

```typescript
encrypted?: pulumi.Input<boolean>;
```


If true, the disk will be encrypted.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/volume.ts#L118">property iops</a>
</h3>

```typescript
iops?: pulumi.Input<number>;
```


The amount of IOPS to provision for the disk.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/volume.ts#L122">property kmsKeyId</a>
</h3>

```typescript
kmsKeyId?: pulumi.Input<string>;
```


The ARN for the KMS encryption key. When specifying `kms_key_id`, `encrypted` needs to be set to true.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/volume.ts#L126">property size</a>
</h3>

```typescript
size?: pulumi.Input<number>;
```


The size of the drive in GiBs.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/volume.ts#L130">property snapshotId</a>
</h3>

```typescript
snapshotId?: pulumi.Input<string>;
```


A snapshot to base the EBS volume off of.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/volume.ts#L134">property tags</a>
</h3>

```typescript
tags?: pulumi.Input<{ ... }>;
```


A mapping of tags to assign to the resource.

<h3 class="pdoc-member-header">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-aws/blob/master/sdk/nodejs/ebs/volume.ts#L138">property type</a>
</h3>

```typescript
type?: pulumi.Input<string>;
```


The type of EBS volume. Can be "standard", "gp2", "io1", "sc1" or "st1" (Default: "standard").

