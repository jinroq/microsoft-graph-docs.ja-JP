---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 7d865c644da353d67052ba8f366c77f9692b7b4b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893233"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/installedApps')
    .get();

```