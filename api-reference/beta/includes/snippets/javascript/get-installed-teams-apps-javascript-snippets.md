---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: d9cfb3a771aea60d9dd0cf22fa9286f553ff3fb0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35868319"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/installedApps')
    .version('beta')
    .get();

```