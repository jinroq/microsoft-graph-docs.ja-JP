---
title: token会議情報リソースの種類
description: token会議情報の種類。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 38a5aae17cf4364a1cfd58680c2e7b9437cf0e40
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345508"
---
# <a name="tokenmeetinginfo-resource-type"></a><span data-ttu-id="c72ab-103">token会議情報リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c72ab-103">tokenMeetingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c72ab-104">token会議情報の種類。</span><span class="sxs-lookup"><span data-stu-id="c72ab-104">The tokenMeetingInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="c72ab-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c72ab-105">Properties</span></span>

| <span data-ttu-id="c72ab-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c72ab-106">Property</span></span>                     | <span data-ttu-id="c72ab-107">型</span><span class="sxs-lookup"><span data-stu-id="c72ab-107">Type</span></span>    | <span data-ttu-id="c72ab-108">説明</span><span class="sxs-lookup"><span data-stu-id="c72ab-108">Description</span></span>                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| <span data-ttu-id="c72ab-109">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="c72ab-109">allowConversationWithoutHost</span></span> | <span data-ttu-id="c72ab-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="c72ab-110">Boolean</span></span> | <span data-ttu-id="c72ab-111">会話のホストが離れると、会話が続行できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c72ab-111">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="c72ab-112">token</span><span class="sxs-lookup"><span data-stu-id="c72ab-112">token</span></span>                        | <span data-ttu-id="c72ab-113">String</span><span class="sxs-lookup"><span data-stu-id="c72ab-113">String</span></span>  | <span data-ttu-id="c72ab-114">ミーティングへの参加/アクティブ化のトークン。</span><span class="sxs-lookup"><span data-stu-id="c72ab-114">The token to join/activate the meeting.</span></span>                                        |

## <a name="json-representation"></a><span data-ttu-id="c72ab-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c72ab-115">JSON representation</span></span>

<span data-ttu-id="c72ab-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c72ab-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
   "baseType": "microsoft.graph.meetingInfo",
  "@odata.type": "microsoft.graph.tokenMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "token": "String"
}
```

## <a name="example"></a><span data-ttu-id="c72ab-117">例</span><span class="sxs-lookup"><span data-stu-id="c72ab-117">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.tokenMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "token": "ABCD123"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "tokenMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
