---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cc71407e30ba0bf8342b4f4023e5ddeba3179644
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730156"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onenoteSection = {
  displayName: "Section name"
};

let res = await client.api('/me/onenote/notebooks/{id}/sections')
    .post({onenoteSection : onenoteSection});

```