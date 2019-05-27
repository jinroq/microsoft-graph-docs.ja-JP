---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: ebfca6a4001f3be672ee174065d6395f59997c3f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463334"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365ActivationCounts')
    .get();

```