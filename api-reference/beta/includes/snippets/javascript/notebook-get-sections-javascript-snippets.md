---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: b390af7b25f445c7d8d3755d3973181ca0b284dd
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879094"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/notebooks/{id}/sections')
    .version('beta')
    .get();

```