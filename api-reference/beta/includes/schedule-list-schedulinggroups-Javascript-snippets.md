---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fca735f841ba58d39cfc875bdbf30f6754c53c7c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34462219"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{teamId}/schedule/schedulingGroups')
    .version('beta')
    .get();

```