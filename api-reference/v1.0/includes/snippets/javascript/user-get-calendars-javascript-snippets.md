---
description: 自動生成されたファイル。 変更しないでください
ms.openlocfilehash: e717736eb8a63e101f9308f497a77cfc90f4f6a5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880768"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendars')
    .get();

```