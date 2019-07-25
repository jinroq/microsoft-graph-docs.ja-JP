---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 594379190675422c4cc4ce3f9409e4e9b5b8e8c2
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870459"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/sectionGroups/{id}/sections')
    .version('beta')
    .get();

```