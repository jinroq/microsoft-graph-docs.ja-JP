---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 29d1bc5ebf589956b98125d981f50131affe226e
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932406"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/installedApps/{id}/upgrade')
    .post();

```