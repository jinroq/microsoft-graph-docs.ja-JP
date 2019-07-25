---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: dd13612a9e39d620b897c5d63d2ca748427d60b6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729229"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const notebook = {
  displayName: "Notebook name"
};

let res = await client.api('/me/onenote/notebooks')
    .version('beta')
    .post({notebook : notebook});

```