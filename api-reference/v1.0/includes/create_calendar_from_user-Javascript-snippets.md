---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 37650ae1350c964754526280a77fe12a4361f946
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34455920"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendar = {
  name: "Volunteer"
};

let res = await client.api('/me/calendars')
    .post({calendar : calendar});

```