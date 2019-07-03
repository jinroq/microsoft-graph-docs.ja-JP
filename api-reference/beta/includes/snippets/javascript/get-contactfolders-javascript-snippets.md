---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 20e4730849f6c8a217f07ee05276a64a7082f08f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35526160"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/contactFolders')
    .version('beta')
    .get();

```