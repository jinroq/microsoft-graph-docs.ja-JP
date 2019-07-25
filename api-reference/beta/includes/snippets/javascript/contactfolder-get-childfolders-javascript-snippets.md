---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e7c6b96fa5e4380f8eb40a6191efd1692b0968cc
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863266"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/contactFolders/{id}/childFolders')
    .version('beta')
    .get();

```