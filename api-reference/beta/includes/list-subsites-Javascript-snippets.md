---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6c03eb6eed82af5d6f44020a364f3ae1650d9f9f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444385"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/sites')
    .version('beta')
    .get();

```