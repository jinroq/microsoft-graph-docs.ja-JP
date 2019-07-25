---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6a6abdaee2ea42cefdd9f63cbda04b38ecfcb49e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721075"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/contacts/{id}/manager')
    .version('beta')
    .get();

```