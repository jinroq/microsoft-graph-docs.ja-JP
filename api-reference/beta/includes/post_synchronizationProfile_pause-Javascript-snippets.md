---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9bb947fd3c07efffe7bbe25e68ace2b12b82e423
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443258"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/synchronizationProfiles/{id}/pause')
    .version('beta')
    .post();

```