---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b261ac6554656669f8dac5511a9aaf45a42892a2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35722738"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  @odata.id: "https://graph.microsoft.com/v1.0/users/{id}"
};

let res = await client.api('/users/{id}/manager/$ref')
    .put({directoryObject : directoryObject});

```