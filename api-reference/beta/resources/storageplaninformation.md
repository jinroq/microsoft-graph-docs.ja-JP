---
author: psampath
ms.author: psampath
ms.date: 06/20/2018
title: StoragePlanInformation
localization_priority: Normal
ms.openlocfilehash: bbe4faaffbf53c24d4d0f5b8ea1f5ee1e1966a2c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860124"
---
# <a name="storageplaninformation-resource-type"></a><span data-ttu-id="aa7b4-102">storagePlanInformation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="aa7b4-102">storagePlanInformation resource type</span></span>

> <span data-ttu-id="aa7b4-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="aa7b4-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aa7b4-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aa7b4-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aa7b4-105">**StoragePlanInformation**リソースでは、ドライブの記憶域のクォータの計画に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="aa7b4-105">The **storagePlanInformation** resource provides information about the drive's storage quota plans.</span></span>

### <a name="json-representation"></a><span data-ttu-id="aa7b4-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aa7b4-106">JSON representation</span></span>

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
## <a name="properties"></a><span data-ttu-id="aa7b4-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aa7b4-107">Properties</span></span>

| <span data-ttu-id="aa7b4-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="aa7b4-108">Property name</span></span>     | <span data-ttu-id="aa7b4-109">Type</span><span class="sxs-lookup"><span data-stu-id="aa7b4-109">Type</span></span>      | <span data-ttu-id="aa7b4-110">説明</span><span class="sxs-lookup"><span data-stu-id="aa7b4-110">Description</span></span>                                                             |
|:------------------|:----------|:----------------------------------------------------------------------- |
| <span data-ttu-id="aa7b4-111">upgradeAvailable</span><span class="sxs-lookup"><span data-stu-id="aa7b4-111">upgradeAvailable</span></span>  | <span data-ttu-id="aa7b4-112">ブール型</span><span class="sxs-lookup"><span data-stu-id="aa7b4-112">Boolean</span></span>   | <span data-ttu-id="aa7b4-113">高いストレージ クォータのプランが利用できることを示します。</span><span class="sxs-lookup"><span data-stu-id="aa7b4-113">Indicates if there are higher storage quota plans available.</span></span> <span data-ttu-id="aa7b4-114">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="aa7b4-114">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "storagePlanInformation resource contains information about storage quota plans that make up the drive's storage space quota.",
  "keywords": "quota,plans,upgradeAvailable",
  "section": "documentation",
  "tocPath": "Resources/StoragePlanInformation"
} -->

