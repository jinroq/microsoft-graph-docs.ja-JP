---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a523035e3b4778a6529fb35a785c3579d4c4ec54
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708924"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/app/calls/57DAB8B1894C409AB240BD8BEAE78896/participants')
    .version('beta')
    .header('Authorization','Bearer <TOKEN>')
    .get();

```