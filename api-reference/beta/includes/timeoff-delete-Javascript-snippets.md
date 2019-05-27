---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 88c8ef62b3ccbd9ae5fac1950f0b3340097f671f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34469259"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{teamId}/schedule/timesOff/{timeOffId}')
    .version('beta')
    .delete();

```