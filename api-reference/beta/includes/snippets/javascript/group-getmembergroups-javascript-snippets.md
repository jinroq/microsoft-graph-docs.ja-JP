---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 365bbe4f3540f4b46a96d605d3fbb1bf34853276
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705472"
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
    .version('beta')
    .post(String);

```