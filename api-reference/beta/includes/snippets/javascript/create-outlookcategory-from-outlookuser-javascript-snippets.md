---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f8f88da12bb483022e1c4399d52fbb490dcdb01d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728804"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookCategory = {
      displayName:"Project expenses",
      color:"preset9"
};

let res = await client.api('/me/outlook/masterCategories')
    .version('beta')
    .post({outlookCategory : outlookCategory});

```