---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 81a8c6be7627fdb048e997e452f111ef6798c170
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35895563"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/AAMkAGVmMDEzM/childFolders')
    .version('beta')
    .get();

```