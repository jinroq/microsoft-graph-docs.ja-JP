---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 38e8b0f9b98119eca9c1bd617d27d74b6c99d888
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/11/2019
ms.locfileid: "36838845"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const reject = {
  reason: "busy"
};

let res = await client.api('/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/reject')
    .version('beta')
    .post(reject);

```