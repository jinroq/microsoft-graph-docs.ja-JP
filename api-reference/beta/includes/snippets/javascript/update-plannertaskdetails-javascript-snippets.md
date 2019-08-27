---
description: 自動的に生成されたファイル。 変更しない
ms.openlocfilehash: 2777a335f2b4863c20ab949e8364dcf7908bd4d8
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/27/2019
ms.locfileid: "36637916"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerTaskDetails = {
  previewType: "noPreview",
  references: {
    http%3A//developer%2Emicrosoft%2Ecom:{
      @odata.type: "microsoft.graph.plannerExternalReference",
      alias: "Documentation",
      previewPriority: " !",
      type: "Other"
    },
    https%3A//developer%2Emicrosoft%2Ecom/en-us/graph/graph-explorer:{
      @odata.type: "microsoft.graph.plannerExternalReference",
      previewPriority: "  !!",
    },
    http%3A//www%2Ebing%2Ecom: null
  },
  checklist: {
    95e27074-6c4a-447a-aa24-9d718a0b86fa:{
      @odata.type: "microsoft.graph.plannerChecklistItem",
      title: "Update task details",
      isChecked: true
    },
    d280ed1a-9f6b-4f9c-a962-fb4d00dc50ff:{
      @odata.type: "microsoft.graph.plannerChecklistItem",
      isChecked: true,
    },
    a93c93c5-10a6-4167-9551-8bafa09967a7: null
  }
};

let res = await client.api('/planner/tasks/gcrYAaAkgU2EQUvpkNNXLGQAGTtu/details')
    .version('beta')
    .update(plannerTaskDetails);

```