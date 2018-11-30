---
title: 受信者リソースの種類
description: 'イベント、メッセージ、またはグループ投稿の送信側または受信側のユーザーに関する情報を表します。 '
ms.openlocfilehash: 7ae272d239f44c3d2f709a03438facb2f0247e49
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020777"
---
# <a name="recipient-resource-type"></a><span data-ttu-id="b5922-103">受信者リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b5922-103">recipient resource type</span></span>

<span data-ttu-id="b5922-104">イベント、メッセージ、またはグループ投稿の送信側または受信側のユーザーに関する情報を表します。</span><span class="sxs-lookup"><span data-stu-id="b5922-104">Represents information about a user in the sending or receiving end of an event, message or group post.</span></span> 

## <a name="properties"></a><span data-ttu-id="b5922-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b5922-105">Properties</span></span>
| <span data-ttu-id="b5922-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b5922-106">Property</span></span>     | <span data-ttu-id="b5922-107">型</span><span class="sxs-lookup"><span data-stu-id="b5922-107">Type</span></span>   |<span data-ttu-id="b5922-108">説明</span><span class="sxs-lookup"><span data-stu-id="b5922-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b5922-109">emailAddress</span><span class="sxs-lookup"><span data-stu-id="b5922-109">emailAddress</span></span>|[<span data-ttu-id="b5922-110">EmailAddress</span><span class="sxs-lookup"><span data-stu-id="b5922-110">EmailAddress</span></span>](emailaddress.md)|<span data-ttu-id="b5922-111">受信者の電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="b5922-111">The recipient's email address.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b5922-112">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b5922-112">JSON representation</span></span>

<span data-ttu-id="b5922-113">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="b5922-113">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recipient"
}-->

```json
{
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->