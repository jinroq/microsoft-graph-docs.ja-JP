---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fa15631a4aa622a455a65cba257fc0a65aa7678c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887705"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/schools/{school-id}/users')
    .get();

```