---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: aaa61709abac9fd45f9a16c8bde0057cecd56eff
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35504712"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  name: "new-file-name.docx"
};

let res = await client.api('/me/drive/items/{item-id}')
    .version('beta')
    .update({driveItem : driveItem});

```