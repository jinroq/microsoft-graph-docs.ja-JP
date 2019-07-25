---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 4dd6648b0b157f33a707dd0f99c7a9faf32ead57
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728162"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRange = {
  shift: "shift-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/insert')
    .version('beta')
    .post(workbookRange);

```