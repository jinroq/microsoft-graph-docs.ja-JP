---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 50155f71279f49080af201820d620a51fe875e95
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34457314"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailboxSettings')
    .get();

```