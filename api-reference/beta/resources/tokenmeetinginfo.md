---
title: tokenMeetingInfo リソースの種類
description: TokenMeetingInfo 型です。
ms.openlocfilehash: ddaf9a0c36ce4a8a31c56e4db2e065ef186c4053
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067698"
---
# <a name="tokenmeetinginfo-resource-type"></a><span data-ttu-id="e8911-103">tokenMeetingInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e8911-103">tokenMeetingInfo resource type</span></span>

> <span data-ttu-id="e8911-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e8911-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8911-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8911-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e8911-106">TokenMeetingInfo 型です。</span><span class="sxs-lookup"><span data-stu-id="e8911-106">The tokenMeetingInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="e8911-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e8911-107">Properties</span></span>

| <span data-ttu-id="e8911-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e8911-108">Property</span></span>                     | <span data-ttu-id="e8911-109">型</span><span class="sxs-lookup"><span data-stu-id="e8911-109">Type</span></span>    | <span data-ttu-id="e8911-110">説明</span><span class="sxs-lookup"><span data-stu-id="e8911-110">Description</span></span>                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| <span data-ttu-id="e8911-111">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="e8911-111">allowConversationWithoutHost</span></span> | <span data-ttu-id="e8911-112">ブール値</span><span class="sxs-lookup"><span data-stu-id="e8911-112">Boolean</span></span> | <span data-ttu-id="e8911-113">会話のホストから離れると、会話を続行できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e8911-113">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="e8911-114">token</span><span class="sxs-lookup"><span data-stu-id="e8911-114">token</span></span>                        | <span data-ttu-id="e8911-115">String</span><span class="sxs-lookup"><span data-stu-id="e8911-115">String</span></span>  | <span data-ttu-id="e8911-116">会議を結合またはアクティブにするトークンです。</span><span class="sxs-lookup"><span data-stu-id="e8911-116">The token to join/activate the meeting.</span></span>                                        |

## <a name="json-representation"></a><span data-ttu-id="e8911-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e8911-117">JSON representation</span></span>

<span data-ttu-id="e8911-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e8911-118">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="e8911-119">使用例</span><span class="sxs-lookup"><span data-stu-id="e8911-119">Example</span></span>

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
