---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: 96dff4c3c89320bef9febde72aed0432a3504434
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881387"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/{id}/childFolders')
    .get();

```