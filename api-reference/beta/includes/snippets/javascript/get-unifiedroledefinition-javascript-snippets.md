---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 72f1fa0da2e3577834443f8e3cf1dd2f8816fb05
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461657"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/roleManagement/directory/roleDefinitions/f189965f-f560-4c59-9101-933d4c87a91a')
    .version('beta')
    .get();

```