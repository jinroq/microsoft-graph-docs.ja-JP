---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9b5ec9a3a26a6eaef217cf9ccffedb8707d5fc45
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855265"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/applications/{id}/owners')
    .version('beta')
    .get();

```