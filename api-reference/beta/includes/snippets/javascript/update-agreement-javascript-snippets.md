---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8ef82992ac250e01586344e4435f49be0202dd92
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637856"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const agreement = {
  displayName: "displayName-value",
  isViewingBeforeAcceptanceRequired: true
};

let res = await client.api('/agreements/{id}')
    .version('beta')
    .update(agreement);

```