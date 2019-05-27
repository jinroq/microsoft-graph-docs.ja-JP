---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 20e4730849f6c8a217f07ee05276a64a7082f08f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34472491"
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