---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 06f8c4ac11665a9d7e5e03e696d3472e18a83b39
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35718438"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getYammerDeviceUsageUserDetail(period='D7')')
    .version('beta')
    .get();

```