---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ec3369f82fe89f9b3ee2eb92583c903d0ae5ceb4
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34468803"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getYammerDeviceUsageUserDetail(period='D7')')
    .get();

```