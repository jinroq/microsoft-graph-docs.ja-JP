---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ac01495e9753a6c380465f505e33a547fb49e9a7
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740230"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookFormatProtection = {
  locked: true,
  formulaHidden: true
};

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/protection')
    .update({workbookFormatProtection : workbookFormatProtection});

```