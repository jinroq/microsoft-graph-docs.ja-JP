---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: cf73b72bfb1628f6a9ff1249a66f986edc6c31b4
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35471367"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  displayName: "displayName-value"
};

let res = await client.api('/me/mailFolders')
    .post({mailFolder : mailFolder});

```