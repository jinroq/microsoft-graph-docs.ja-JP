---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 579d70e82cf18190a8e77a39a900b0f152c4e410
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720816"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const CommsOperation = {
  participants: [
    ""
  ],
  clientContext: "clientContext-value"
};

let res = await client.api('/app/calls/{id}/participants/muteAll')
    .version('beta')
    .post(CommsOperation);

```