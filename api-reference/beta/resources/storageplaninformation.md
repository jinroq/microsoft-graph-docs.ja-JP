---
author: psampath
ms.author: psampath
ms.date: 06/20/2018
title: StoragePlanInformation
localization_priority: Normal
ms.openlocfilehash: 05140b3256e434449d663c4992e74298bbdedd30
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582115"
---
# <a name="storageplaninformation-resource-type"></a><span data-ttu-id="7757a-102">storageplan 情報リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7757a-102">storagePlanInformation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7757a-103">**storageplan information**リソースは、ドライブの記憶域クォータプランに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="7757a-103">The **storagePlanInformation** resource provides information about the drive's storage quota plans.</span></span>

### <a name="json-representation"></a><span data-ttu-id="7757a-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7757a-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
   "@odata.type": "microsoft.graph.storagePlanInformation",
} -->

```json
{
  "upgradeAvailable": true
}

```
## <a name="properties"></a><span data-ttu-id="7757a-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7757a-105">Properties</span></span>

| <span data-ttu-id="7757a-106">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="7757a-106">Property name</span></span>     | <span data-ttu-id="7757a-107">種類</span><span class="sxs-lookup"><span data-stu-id="7757a-107">Type</span></span>      | <span data-ttu-id="7757a-108">説明</span><span class="sxs-lookup"><span data-stu-id="7757a-108">Description</span></span>                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| <span data-ttu-id="7757a-109">upgradeavailable</span><span class="sxs-lookup"><span data-stu-id="7757a-109">upgradeAvailable</span></span>  | <span data-ttu-id="7757a-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="7757a-110">Boolean</span></span>   | <span data-ttu-id="7757a-111">利用可能なストレージクォータプランが高であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7757a-111">Indicates if there are higher storage quota plans available.</span></span> <span data-ttu-id="7757a-112">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="7757a-112">Read-only.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "storagePlanInformation resource contains information about storage quota plans that make up the drive's storage space quota.",
  "keywords": "quota,plans,upgradeAvailable",
  "section": "documentation",
  "tocPath": "Resources/StoragePlanInformation",
  "suppressions": [
    "Error: /api-reference/beta/resources/storageplaninformation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

