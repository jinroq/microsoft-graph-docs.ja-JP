---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5f35c328a415de6839e85ffa44f41302c9c26edf
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728773"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onenoteOperation = {
  id: "id-value",
  groupId: "groupId-value"
};

let res = await client.api('/me/onenote/pages/{id}/copyToSection')
    .version('beta')
    .post(onenoteOperation);

```