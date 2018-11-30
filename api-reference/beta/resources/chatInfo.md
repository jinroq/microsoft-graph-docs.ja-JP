---
title: chatInfo リソースの種類
description: マイクロソフトのチーム内のメッセージについて説明します。
ms.openlocfilehash: d7e90cf2cdf5180f6483675d919b4e635a1cd5fa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066478"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="001e9-103">chatInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="001e9-103">chatInfo resource type</span></span>

> <span data-ttu-id="001e9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="001e9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="001e9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="001e9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="001e9-106">マイクロソフトのチーム内のメッセージについて説明します。</span><span class="sxs-lookup"><span data-stu-id="001e9-106">Information about a message in Microsoft Teams.</span></span>

## <a name="properties"></a><span data-ttu-id="001e9-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="001e9-107">Properties</span></span>

| <span data-ttu-id="001e9-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="001e9-108">Property</span></span>            | <span data-ttu-id="001e9-109">型</span><span class="sxs-lookup"><span data-stu-id="001e9-109">Type</span></span>    | <span data-ttu-id="001e9-110">説明</span><span class="sxs-lookup"><span data-stu-id="001e9-110">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="001e9-111">メッセージ Id</span><span class="sxs-lookup"><span data-stu-id="001e9-111">messageId</span></span>           | <span data-ttu-id="001e9-112">String</span><span class="sxs-lookup"><span data-stu-id="001e9-112">String</span></span>  | <span data-ttu-id="001e9-113">マイクロソフト チームのチャネルでのメッセージの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="001e9-113">The unique identifier for a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="001e9-114">replyChainMessageId</span><span class="sxs-lookup"><span data-stu-id="001e9-114">replyChainMessageId</span></span> | <span data-ttu-id="001e9-115">String</span><span class="sxs-lookup"><span data-stu-id="001e9-115">String</span></span>  | <span data-ttu-id="001e9-116">返信メッセージの ID です。</span><span class="sxs-lookup"><span data-stu-id="001e9-116">The ID of the reply message.</span></span> |
| <span data-ttu-id="001e9-117">スレッド Id</span><span class="sxs-lookup"><span data-stu-id="001e9-117">threadId</span></span>            | <span data-ttu-id="001e9-118">String</span><span class="sxs-lookup"><span data-stu-id="001e9-118">String</span></span>  | <span data-ttu-id="001e9-119">マイクロソフトのチームでのスレッドの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="001e9-119">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="001e9-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="001e9-120">JSON representation</span></span>

<span data-ttu-id="001e9-121">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="001e9-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatInfo"
}-->
```json
{
  "messageId": "String",
  "replyChainMessageId": "String",
  "threadId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
