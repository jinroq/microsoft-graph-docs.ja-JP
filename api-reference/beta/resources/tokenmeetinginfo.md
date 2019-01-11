---
title: tokenMeetingInfo リソースの種類
description: TokenMeetingInfo 型です。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 9a618906df450ce58f7428a76367e896b315591a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806980"
---
# <a name="tokenmeetinginfo-resource-type"></a><span data-ttu-id="32c94-103">tokenMeetingInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="32c94-103">tokenMeetingInfo resource type</span></span>

> <span data-ttu-id="32c94-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="32c94-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="32c94-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="32c94-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="32c94-106">TokenMeetingInfo 型です。</span><span class="sxs-lookup"><span data-stu-id="32c94-106">The tokenMeetingInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="32c94-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="32c94-107">Properties</span></span>

| <span data-ttu-id="32c94-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="32c94-108">Property</span></span>                     | <span data-ttu-id="32c94-109">種類</span><span class="sxs-lookup"><span data-stu-id="32c94-109">Type</span></span>    | <span data-ttu-id="32c94-110">説明</span><span class="sxs-lookup"><span data-stu-id="32c94-110">Description</span></span>                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| <span data-ttu-id="32c94-111">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="32c94-111">allowConversationWithoutHost</span></span> | <span data-ttu-id="32c94-112">ブール型</span><span class="sxs-lookup"><span data-stu-id="32c94-112">Boolean</span></span> | <span data-ttu-id="32c94-113">会話のホストから離れると、会話を続行できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="32c94-113">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="32c94-114">token</span><span class="sxs-lookup"><span data-stu-id="32c94-114">token</span></span>                        | <span data-ttu-id="32c94-115">String</span><span class="sxs-lookup"><span data-stu-id="32c94-115">String</span></span>  | <span data-ttu-id="32c94-116">会議を結合またはアクティブにするトークンです。</span><span class="sxs-lookup"><span data-stu-id="32c94-116">The token to join/activate the meeting.</span></span>                                        |

## <a name="json-representation"></a><span data-ttu-id="32c94-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="32c94-117">JSON representation</span></span>

<span data-ttu-id="32c94-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="32c94-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tokenMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "token": "String"
}
```

## <a name="example"></a><span data-ttu-id="32c94-119">例</span><span class="sxs-lookup"><span data-stu-id="32c94-119">Example</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "tokenMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
