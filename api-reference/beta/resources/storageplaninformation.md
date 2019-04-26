---
author: psampath
ms.author: psampath
ms.date: 06/20/2018
title: StoragePlanInformation
localization_priority: Normal
ms.openlocfilehash: 3911d3af5f2149d1043ed246e7c11d287c840842
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342953"
---
# <a name="storageplaninformation-resource-type"></a><span data-ttu-id="8492b-102">storageplan 情報リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8492b-102">storagePlanInformation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8492b-103">**storageplan information**リソースは、ドライブの記憶域クォータプランに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="8492b-103">The **storagePlanInformation** resource provides information about the drive's storage quota plans.</span></span>

### <a name="json-representation"></a><span data-ttu-id="8492b-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8492b-104">JSON representation</span></span>

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
## <a name="properties"></a><span data-ttu-id="8492b-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8492b-105">Properties</span></span>

| <span data-ttu-id="8492b-106">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="8492b-106">Property name</span></span>     | <span data-ttu-id="8492b-107">種類</span><span class="sxs-lookup"><span data-stu-id="8492b-107">Type</span></span>      | <span data-ttu-id="8492b-108">説明</span><span class="sxs-lookup"><span data-stu-id="8492b-108">Description</span></span>                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| <span data-ttu-id="8492b-109">upgradeavailable</span><span class="sxs-lookup"><span data-stu-id="8492b-109">upgradeAvailable</span></span>  | <span data-ttu-id="8492b-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="8492b-110">Boolean</span></span>   | <span data-ttu-id="8492b-111">利用可能なストレージクォータプランが高であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8492b-111">Indicates if there are higher storage quota plans available.</span></span> <span data-ttu-id="8492b-112">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="8492b-112">Read-only.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "storagePlanInformation resource contains information about storage quota plans that make up the drive's storage space quota.",
  "keywords": "quota,plans,upgradeAvailable",
  "section": "documentation",
  "tocPath": "Resources/StoragePlanInformation",
  "suppressions": []
}
-->

