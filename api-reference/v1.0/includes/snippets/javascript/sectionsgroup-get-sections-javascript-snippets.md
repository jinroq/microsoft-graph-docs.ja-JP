---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: f4d57e0ce0f0210092173ca75c376745112e4b77
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883022"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/sectionGroups/{id}/sections')
    .get();

```