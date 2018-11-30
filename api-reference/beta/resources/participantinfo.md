---
title: participantInfo リソースの種類
description: 参加者のアイデンティティについての追加のプロパティが含まれています
ms.openlocfilehash: c6f429e353d80ea53c5f5c00ca084ae7a8a4a7c1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066557"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="31dec-103">participantInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="31dec-103">participantInfo resource type</span></span>

> <span data-ttu-id="31dec-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="31dec-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31dec-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31dec-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="31dec-106">参加者のアイデンティティについての追加のプロパティが含まれています</span><span class="sxs-lookup"><span data-stu-id="31dec-106">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="31dec-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31dec-107">Properties</span></span>

| <span data-ttu-id="31dec-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31dec-108">Property</span></span>       | <span data-ttu-id="31dec-109">型</span><span class="sxs-lookup"><span data-stu-id="31dec-109">Type</span></span>                          | <span data-ttu-id="31dec-110">説明</span><span class="sxs-lookup"><span data-stu-id="31dec-110">Description</span></span>  |
|:---------------|:------------------------------|:-------------|
| <span data-ttu-id="31dec-111">identity</span><span class="sxs-lookup"><span data-stu-id="31dec-111">identity</span></span>       | [<span data-ttu-id="31dec-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="31dec-112">identitySet</span></span>](identityset.md) | <span data-ttu-id="31dec-113">この構成要素に関連付けられている[identitySet](identityset.md) 。</span><span class="sxs-lookup"><span data-stu-id="31dec-113">The [identitySet](identityset.md) associated with this participant.</span></span> |
| <span data-ttu-id="31dec-114">languageId</span><span class="sxs-lookup"><span data-stu-id="31dec-114">languageId</span></span>     | <span data-ttu-id="31dec-115">String</span><span class="sxs-lookup"><span data-stu-id="31dec-115">String</span></span>                        | <span data-ttu-id="31dec-116">言語カルチャの文字列です。</span><span class="sxs-lookup"><span data-stu-id="31dec-116">The language culture string.</span></span> |
| <span data-ttu-id="31dec-117">地域</span><span class="sxs-lookup"><span data-stu-id="31dec-117">region</span></span>         | <span data-ttu-id="31dec-118">String</span><span class="sxs-lookup"><span data-stu-id="31dec-118">String</span></span>                        | <span data-ttu-id="31dec-119">参加者の領域です。</span><span class="sxs-lookup"><span data-stu-id="31dec-119">Region of the participant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="31dec-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="31dec-120">JSON representation</span></span>

<span data-ttu-id="31dec-121">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="31dec-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "languageId", "region"
  ],
  "@odata.type": "microsoft.graph.participantInfo"
}-->
```json
{
  "identity": { "@odata.type": "#microsoft.graph.identitySet" },
  "languageId": "String",
  "region": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "participantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->