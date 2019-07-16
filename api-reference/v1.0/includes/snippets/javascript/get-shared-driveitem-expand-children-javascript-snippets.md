---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 077fc33ed89ca63455291b710a27ff5a60420761
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736879"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/shares/{shareIdOrUrl}/driveItem')
    .expand('children')
    .get();

```