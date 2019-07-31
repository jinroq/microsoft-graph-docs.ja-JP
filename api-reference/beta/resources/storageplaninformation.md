---
author: psampath
description: Storageplan Information リソースは、ドライブの記憶域クォータプランに関する情報を提供します。
ms.date: 06/20/2018
title: StoragePlanInformation
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: d8ddb39f9f7c6443f0e669052084af27b8fd5cec
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008083"
---
# <a name="storageplaninformation-resource-type"></a><span data-ttu-id="6086a-103">Storageplan 情報リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6086a-103">storagePlanInformation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6086a-104">**Storageplan information**リソースは、ドライブの記憶域クォータプランに関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="6086a-104">The **storagePlanInformation** resource provides information about the drive's storage quota plans.</span></span>

### <a name="json-representation"></a><span data-ttu-id="6086a-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6086a-105">JSON representation</span></span>

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
## <a name="properties"></a><span data-ttu-id="6086a-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6086a-106">Properties</span></span>

| <span data-ttu-id="6086a-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="6086a-107">Property name</span></span>     | <span data-ttu-id="6086a-108">種類</span><span class="sxs-lookup"><span data-stu-id="6086a-108">Type</span></span>      | <span data-ttu-id="6086a-109">説明</span><span class="sxs-lookup"><span data-stu-id="6086a-109">Description</span></span>                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| <span data-ttu-id="6086a-110">upgradeAvailable</span><span class="sxs-lookup"><span data-stu-id="6086a-110">upgradeAvailable</span></span>  | <span data-ttu-id="6086a-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="6086a-111">Boolean</span></span>   | <span data-ttu-id="6086a-112">利用可能なストレージクォータプランが高であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6086a-112">Indicates if there are higher storage quota plans available.</span></span> <span data-ttu-id="6086a-113">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="6086a-113">Read-only.</span></span> |


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

