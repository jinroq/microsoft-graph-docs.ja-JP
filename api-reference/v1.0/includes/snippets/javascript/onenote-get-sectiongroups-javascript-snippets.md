---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 931bc628555e4d51f4dc041e446c4dc3a439bb47
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855140"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/sectionGroups')
    .get();

```