---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8fde6b9aebf50a0e19fa0205167b44b0f964c573
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863199"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/contactFolders/{id}/contacts')
    .version('beta')
    .get();

```