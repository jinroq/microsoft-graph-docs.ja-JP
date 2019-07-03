---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 077fc33ed89ca63455291b710a27ff5a60420761
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35471645"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/shares/{shareIdOrUrl}/driveItem')
    .expand('children')
    .get();

```