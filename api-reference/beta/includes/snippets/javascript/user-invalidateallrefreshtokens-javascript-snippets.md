---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: bf753b660ca48e00f98b8de2d0ad6ab2d3630216
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35486025"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/invalidateAllRefreshTokens')
    .version('beta')
    .post();

```