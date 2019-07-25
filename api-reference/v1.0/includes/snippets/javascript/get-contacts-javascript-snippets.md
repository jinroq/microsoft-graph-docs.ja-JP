---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 5e013d191f751ae21c4f4f9fbfc50312c52ef68c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35895097"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/contacts')
    .get();

```