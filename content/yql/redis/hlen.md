---
title: HLEN
---

## SYNOPSIS
<code>HLEN key</code><br>
This command is to fetch the number of fields in the hash that is associated with the given <code>key</code>
<li>If the <code>key</code> does not exist, 0 is returned.</li>
<li>If the <code>key</code> is associated with non-hash data, an error is raised.</li>

## RETURN VALUE
Returns number of fields in the specified hash.

## EXAMPLES
% <code>HSET yugahash area1 "Africa"</code><br>
1<br>
% <code>HSET yugahash area2 "America"</code><br>
1<br>
% <code>HLEN yugahash</code><br>
2<br>

## SEE ALSO