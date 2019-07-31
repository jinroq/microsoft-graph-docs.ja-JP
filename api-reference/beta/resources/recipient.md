---
title: 受信者リソースの種類
description: 'イベント、メッセージ、またはグループ投稿の送信側または受信側のユーザーに関する情報を表します。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 5964164937f184ce94d068636a39301a988937e6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008811"
---
# <a name="recipient-resource-type"></a><span data-ttu-id="a4878-103">受信者リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a4878-103">recipient resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4878-104">イベント、メッセージ、またはグループ投稿の送信側または受信側のユーザーに関する情報を表します。</span><span class="sxs-lookup"><span data-stu-id="a4878-104">Represents information about a user in the sending or receiving end of an event, message or group post.</span></span> 

## <a name="properties"></a><span data-ttu-id="a4878-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4878-105">Properties</span></span>
| <span data-ttu-id="a4878-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a4878-106">Property</span></span>     | <span data-ttu-id="a4878-107">型</span><span class="sxs-lookup"><span data-stu-id="a4878-107">Type</span></span>   |<span data-ttu-id="a4878-108">説明</span><span class="sxs-lookup"><span data-stu-id="a4878-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4878-109">emailAddress</span><span class="sxs-lookup"><span data-stu-id="a4878-109">emailAddress</span></span>|[<span data-ttu-id="a4878-110">EmailAddress</span><span class="sxs-lookup"><span data-stu-id="a4878-110">EmailAddress</span></span>](emailaddress.md)|<span data-ttu-id="a4878-111">受信者の電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="a4878-111">The recipient's email address.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a4878-112">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a4878-112">JSON representation</span></span>

<span data-ttu-id="a4878-113">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="a4878-113">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "recipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
