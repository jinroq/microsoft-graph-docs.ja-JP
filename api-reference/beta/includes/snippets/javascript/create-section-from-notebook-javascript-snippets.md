---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6d9e70ededb5507a7c61f24898dc33aad3925f0b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729219"
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
    .version('beta')
    .post({onenoteSection : onenoteSection});

```