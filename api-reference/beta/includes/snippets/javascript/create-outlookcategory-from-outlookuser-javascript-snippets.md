---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f8f88da12bb483022e1c4399d52fbb490dcdb01d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35486419"
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