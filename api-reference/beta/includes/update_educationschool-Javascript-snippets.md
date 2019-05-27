---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 9aee84a3a1bbd8bc8e4ae2597b3f40983d4ed3cd
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2019
ms.locfileid: "34461245"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationSchool = {
  displayName: "Fabrikam Arts High School",
  description: "Magnate school for the arts. Los Angeles School District"
};

let res = await client.api('/education/schools/10002')
    .version('beta')
    .update({educationSchool : educationSchool});

```