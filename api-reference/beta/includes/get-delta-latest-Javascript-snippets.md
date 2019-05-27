---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 6c403b06cb89d6daaf5d9d023820d825e46032e9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436356"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/delta')
    .version('beta')
    .get();

```