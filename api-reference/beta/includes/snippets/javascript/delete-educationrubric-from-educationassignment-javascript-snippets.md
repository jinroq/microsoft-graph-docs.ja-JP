---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 8c33ee9ebacf0b75c52efffde6d1ca83a09e19f0
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461215"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/me/assignments/{id}/rubric/$ref')
    .version('beta')
    .delete();

```