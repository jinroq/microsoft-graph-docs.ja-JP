---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 41158f1324ff15fcb515cf1f1c8799fa92175ca6
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932832"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  name: "Shared legal agreements"
};

let res = await client.api('/drive/items/{bundle-id}')
    .version('beta')
    .update({driveItem : driveItem});

```