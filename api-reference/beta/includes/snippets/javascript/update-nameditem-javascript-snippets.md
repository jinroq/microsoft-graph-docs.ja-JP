---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: c0dd5b28dbdfc672556aa0af2e57b8e5ecffac98
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637983"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookNamedItem = {
  type: "type-value",
  scope: "scope-value",
  comment: "comment-value",
  value: {
  },
  visible: true
};

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}')
    .version('beta')
    .update(workbookNamedItem);

```