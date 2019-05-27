---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 92ad3b87cf1e8cdf9c46be28df8bdec6086bfc13
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34454293"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365ActiveUserDetail(period='D7')')
    .get();

```