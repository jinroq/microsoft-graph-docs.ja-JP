---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a1a2b65c182ae0ef09898e64518e3496e69c6e79
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35485709"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getEmailAppUsageAppsUserCounts(period='D7')')
    .version('beta')
    .get();

```