---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: e6b8a72e7e058e6de0fdcd35ca83cbbf23aad17e
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35931763"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/installedApps/{id}/upgrade')
    .version('beta')
    .post();

```