---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: a9e00c07b8f657f4d3319a7ec62d1d52ac2eefe2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35471326"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/{id}')
    .delete();

```