---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 285d4b8200b5135959a1aabb17c0d469987ee118
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734063"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const String = {
  securityEnabledOnly: true
};

let res = await client.api('/directoryObjects/{object-id}/getMemberObjects')
    .post(String);

```