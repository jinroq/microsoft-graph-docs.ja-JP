---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0a63fbb6408eb33cdf14df9d705bef95789a9df0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35495885"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const String = {
  securityEnabledOnly: false
};

let res = await client.api('/groups/{id}/getMemberGroups')
    .post(String);

```