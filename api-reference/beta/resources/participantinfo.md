---
title: participantInfo リソースの種類
description: 参加者のアイデンティティについての追加のプロパティが含まれています
author: VinodRavichandran
ms.openlocfilehash: 335626d1c34e2c54a86b0494e931c2da3fe283e7
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380493"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="08ab1-103">participantInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="08ab1-103">participantInfo resource type</span></span>

> <span data-ttu-id="08ab1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="08ab1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="08ab1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="08ab1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="08ab1-106">参加者のアイデンティティについての追加のプロパティが含まれています</span><span class="sxs-lookup"><span data-stu-id="08ab1-106">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="08ab1-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="08ab1-107">Properties</span></span>

| <span data-ttu-id="08ab1-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="08ab1-108">Property</span></span>       | <span data-ttu-id="08ab1-109">型</span><span class="sxs-lookup"><span data-stu-id="08ab1-109">Type</span></span>                          | <span data-ttu-id="08ab1-110">説明</span><span class="sxs-lookup"><span data-stu-id="08ab1-110">Description</span></span>  |
|:---------------|:------------------------------|:-------------|
| <span data-ttu-id="08ab1-111">identity</span><span class="sxs-lookup"><span data-stu-id="08ab1-111">identity</span></span>       | [<span data-ttu-id="08ab1-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="08ab1-112">identitySet</span></span>](identityset.md) | <span data-ttu-id="08ab1-113">この構成要素に関連付けられている[identitySet](identityset.md) 。</span><span class="sxs-lookup"><span data-stu-id="08ab1-113">The [identitySet](identityset.md) associated with this participant.</span></span> |
| <span data-ttu-id="08ab1-114">languageId</span><span class="sxs-lookup"><span data-stu-id="08ab1-114">languageId</span></span>     | <span data-ttu-id="08ab1-115">String</span><span class="sxs-lookup"><span data-stu-id="08ab1-115">String</span></span>                        | <span data-ttu-id="08ab1-116">言語カルチャの文字列です。</span><span class="sxs-lookup"><span data-stu-id="08ab1-116">The language culture string.</span></span> |
| <span data-ttu-id="08ab1-117">地域</span><span class="sxs-lookup"><span data-stu-id="08ab1-117">region</span></span>         | <span data-ttu-id="08ab1-118">String</span><span class="sxs-lookup"><span data-stu-id="08ab1-118">String</span></span>                        | <span data-ttu-id="08ab1-119">参加者の領域です。</span><span class="sxs-lookup"><span data-stu-id="08ab1-119">Region of the participant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="08ab1-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="08ab1-120">JSON representation</span></span>

<span data-ttu-id="08ab1-121">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="08ab1-121">The following is a JSON representation of the resource.</span></span>

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