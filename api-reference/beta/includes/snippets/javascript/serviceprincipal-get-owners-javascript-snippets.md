---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1019b5f98da729e015d392932685c9a09a0b2cca
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869987"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/owners')
    .version('beta')
    .get();

```