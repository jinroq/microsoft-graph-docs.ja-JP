---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 99084435a33a45c51edbc87d8dc5f4d34a7b6707
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34467031"
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