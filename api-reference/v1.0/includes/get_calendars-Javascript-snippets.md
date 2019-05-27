---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e717736eb8a63e101f9308f497a77cfc90f4f6a5
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34457088"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendars')
    .get();

```