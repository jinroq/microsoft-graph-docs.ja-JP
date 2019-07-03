---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a23cd922028856979dd7c7226eec4e4b5d18d76e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526689"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/schools/10002')
    .version('beta')
    .delete();

```