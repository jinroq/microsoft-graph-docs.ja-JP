---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 99084435a33a45c51edbc87d8dc5f4d34a7b6707
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730679"
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
    .update({driveItem : driveItem});

```