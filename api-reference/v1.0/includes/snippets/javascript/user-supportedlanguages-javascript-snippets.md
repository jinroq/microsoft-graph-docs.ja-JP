---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 0175722425643281be38475b34c70a6b0e26b78f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35513175"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/outlook/supportedLanguages')
    .get();

```