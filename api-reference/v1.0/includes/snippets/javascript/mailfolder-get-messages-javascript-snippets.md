---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: 58a23f9b7ec11359d399a6d318eb6655ce7b1de9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856470"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/{id}/messages')
    .get();

```