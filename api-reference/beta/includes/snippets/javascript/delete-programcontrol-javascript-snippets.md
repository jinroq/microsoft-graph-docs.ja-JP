---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 1ce43fdd45559b3369b9b06f9d1550d419bf24a5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35503774"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/programControls/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213')
    .version('beta')
    .delete();

```