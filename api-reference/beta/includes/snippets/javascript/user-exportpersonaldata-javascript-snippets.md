---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b711f61baefc94a59a130e487fffe364c7250fd3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724267"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const exportPersonalData = {
  storageLocation: "storageLocation-value"
};

let res = await client.api('/users/{id}/exportPersonalData')
    .version('beta')
    .post(exportPersonalData);

```