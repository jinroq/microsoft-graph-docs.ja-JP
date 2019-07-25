---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 398ab8439e89bb308cd275f7f09b5833a4b84a37
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887991"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/sections')
    .get();

```