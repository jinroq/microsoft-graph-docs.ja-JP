---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 206c2622e8de196934258fd85bc5eef4658106e8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883937"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/contactFolders/{id}/childFolders')
    .get();

```