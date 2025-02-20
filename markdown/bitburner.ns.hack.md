<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [bitburner](./bitburner.md) &gt; [NS](./bitburner.ns.md) &gt; [hack](./bitburner.ns.hack.md)

## NS.hack() method

Steal a servers money.

<b>Signature:</b>

```typescript
hack(host: string, opts?: BasicHGWOptions): Promise<number>;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  host | string | Hostname of the target server to hack. |
|  opts | [BasicHGWOptions](./bitburner.basichgwoptions.md) | Optional parameters for configuring function behavior. |

<b>Returns:</b>

Promise&lt;number&gt;

The amount of money stolen if the hack is successful, and zero otherwise.

## Remarks

RAM cost: 0.1 GB

Function that is used to try and hack servers to steal money and gain hacking experience. The runtime for this command depends on your hacking level and the target server’s security level. In order to hack a server you must first gain root access to that server and also have the required hacking level.

A script can hack a server from anywhere. It does not need to be running on the same server to hack that server. For example, you can create a script that hacks the `foodnstuff` server and run that script on any server in the game.

A successful `hack()` on a server will raise that server’s security level by 0.002.

## Example


```ts
hack("foodnstuff");
hack("foodnstuff", { threads: 5 }); // Only use 5 threads to hack
```

