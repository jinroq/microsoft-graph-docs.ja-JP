---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: dd352fde8fe949c91067edef4f63a8939c0bcc5e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723120"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/dataBodyRange')
    .post();

```