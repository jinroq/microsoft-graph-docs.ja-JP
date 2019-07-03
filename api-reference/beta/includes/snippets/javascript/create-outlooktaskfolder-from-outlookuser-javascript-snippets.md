---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: fd5f436d26cb3d60c492d089ba8c32204e8c8833
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35486416"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookTaskFolder = {
  name: "Volunteer"
};

let res = await client.api('/me/outlook/taskfolders')
    .version('beta')
    .post({outlookTaskFolder : outlookTaskFolder});

```