---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 92f8968614463785718ffd20c05950781a25445d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876862"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/places/3162F1E1-C4C0-604B-51D8-91DA78989EB1')
    .version('beta')
    .get();

```