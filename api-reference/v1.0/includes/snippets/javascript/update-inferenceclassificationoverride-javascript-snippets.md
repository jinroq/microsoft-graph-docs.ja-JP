---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 48154e70c2aef726068d740131ea7093fddee78e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35738927"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const inferenceClassificationOverride = {
  classifyAs: "focused"
};

let res = await client.api('/me/inferenceClassification/overrides/{id}')
    .update({inferenceClassificationOverride : inferenceClassificationOverride});

```