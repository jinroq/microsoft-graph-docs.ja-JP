---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 86add7d946d8f1d5614d3a246ef39e82fb924cf4
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713692"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/conversations')
    .version('beta')
    .get();

```