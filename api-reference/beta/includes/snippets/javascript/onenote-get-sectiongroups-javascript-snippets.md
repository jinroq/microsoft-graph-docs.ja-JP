---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fb1e009475830b217b754945b2bf2033ced65d7e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878873"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/sectionGroups')
    .version('beta')
    .get();

```