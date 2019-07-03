---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 48154e70c2aef726068d740131ea7093fddee78e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35471680"
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