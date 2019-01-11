---
title: 受信者リソースの種類
description: 'イベント、メッセージ、またはグループ投稿の送信側または受信側のユーザーに関する情報を表します。 '
localization_priority: Normal
ms.openlocfilehash: b234cac0526ee66a59a19f7059dbebdc8a1bdcb3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27848378"
---
# <a name="recipient-resource-type"></a><span data-ttu-id="664f5-103">受信者リソースの種類</span><span class="sxs-lookup"><span data-stu-id="664f5-103">recipient resource type</span></span>

> <span data-ttu-id="664f5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="664f5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="664f5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="664f5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="664f5-106">イベント、メッセージ、またはグループ投稿の送信側または受信側のユーザーに関する情報を表します。</span><span class="sxs-lookup"><span data-stu-id="664f5-106">Represents information about a user in the sending or receiving end of an event, message or group post.</span></span> 

## <a name="properties"></a><span data-ttu-id="664f5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="664f5-107">Properties</span></span>
| <span data-ttu-id="664f5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="664f5-108">Property</span></span>     | <span data-ttu-id="664f5-109">種類</span><span class="sxs-lookup"><span data-stu-id="664f5-109">Type</span></span>   |<span data-ttu-id="664f5-110">説明</span><span class="sxs-lookup"><span data-stu-id="664f5-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="664f5-111">emailAddress</span><span class="sxs-lookup"><span data-stu-id="664f5-111">emailAddress</span></span>|[<span data-ttu-id="664f5-112">EmailAddress</span><span class="sxs-lookup"><span data-stu-id="664f5-112">EmailAddress</span></span>](emailaddress.md)|<span data-ttu-id="664f5-113">受信者の電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="664f5-113">The recipient's email address.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="664f5-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="664f5-114">JSON representation</span></span>

<span data-ttu-id="664f5-115">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="664f5-115">Here is a JSON representation of the resource</span></span>

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
