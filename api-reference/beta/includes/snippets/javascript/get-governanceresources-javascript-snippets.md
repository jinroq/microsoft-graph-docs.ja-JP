---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f046101bd48b2e49f4f8e93abac16eb03bedb176
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713935"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/privilegedAccess/azureResources/resources')
    .version('beta')
    .get();

```