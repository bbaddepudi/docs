---
title: PSUBSCRIBE
linkTitle: PSUBSCRIBE
description: PSUBSCRIBE
menu:
  latest:
    parent: api-yedis
    weight: 2554
aliases:
  - /latest/api/redis/psubscribe
  - /latest/api/yedis/psubscribe
isTocNested: true
showAsideToc: true
---
`PSUBSCRIBE` 

## Synopsis
<b>`PSUBSCRIBE pattern [pattern ...]`</b><br>
This command subscribes the client to the specified pattern(s). The client will receive a message whenever a publisher sends a message to a channel that matches any of the patterns that it has subscribed to.

## See Also
[`keys`](../keys/), 
[`pubsub`](../pubsub/), 
[`publish`](../publish/), 
[`subscribe`](../subscribe/), 
[`unsubscribe`](../unsubscribe/), 
[`psubscribe`](../psubscribe/), 
[`punsubscribe`](../punsubscribe/)
