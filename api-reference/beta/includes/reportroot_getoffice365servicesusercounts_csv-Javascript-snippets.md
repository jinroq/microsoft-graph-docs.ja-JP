---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 362a7841c68cc5b5ceb38e1b93a9d4e48fd75a18
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34441312"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365ServicesUserCounts(period='D7')')
    .version('beta')
    .get();

```