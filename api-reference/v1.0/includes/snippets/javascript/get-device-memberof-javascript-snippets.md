---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 770166e1fe7c3766b01188de60e3623f6a6acc13
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883483"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/devices/{id}/memberOf')
    .get();

```