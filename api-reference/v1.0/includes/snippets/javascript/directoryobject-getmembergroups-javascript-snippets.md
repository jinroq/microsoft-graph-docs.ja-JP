---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8d94193387befabbb8d5724b993c356c5271dae2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715834"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const String = {
  securityEnabledOnly: true
};

let res = await client.api('/directoryObjects/{object-id}/getMemberGroups')
    .post(String);

```