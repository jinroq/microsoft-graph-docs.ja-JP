---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6207450177ab74d72153762b5033eb1aa1e7f986
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637758"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  @odata.id: "https://graph.microsoft.com/beta/directoryObjects/{id}"
};

let res = await client.api('/groups/{id}/members/$ref')
    .version('beta')
    .post(directoryObject);

```