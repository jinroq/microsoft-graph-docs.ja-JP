---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f967ac07ded10f92892dbec3926a8532c86aa745
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459301"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryRoles/{id}/members/{id}/$ref')
    .delete();

```