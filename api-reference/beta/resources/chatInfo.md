---
title: chatInfo リソースの種類
description: マイクロソフトのチーム内のメッセージについて説明します。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 840073d6882d6665be60e7386eaafe3168b70dbe
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940751"
---
# <a name="chatinfo-resource-type"></a><span data-ttu-id="7f357-103">chatInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7f357-103">chatInfo resource type</span></span>

> <span data-ttu-id="7f357-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7f357-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f357-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f357-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7f357-106">マイクロソフトのチーム内のメッセージについて説明します。</span><span class="sxs-lookup"><span data-stu-id="7f357-106">Information about a message in Microsoft Teams.</span></span>

## <a name="properties"></a><span data-ttu-id="7f357-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f357-107">Properties</span></span>

| <span data-ttu-id="7f357-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f357-108">Property</span></span>            | <span data-ttu-id="7f357-109">種類</span><span class="sxs-lookup"><span data-stu-id="7f357-109">Type</span></span>    | <span data-ttu-id="7f357-110">説明</span><span class="sxs-lookup"><span data-stu-id="7f357-110">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="7f357-111">メッセージ Id</span><span class="sxs-lookup"><span data-stu-id="7f357-111">messageId</span></span>           | <span data-ttu-id="7f357-112">String</span><span class="sxs-lookup"><span data-stu-id="7f357-112">String</span></span>  | <span data-ttu-id="7f357-113">マイクロソフト チームのチャネルでのメッセージの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="7f357-113">The unique identifier for a message in a Microsoft Teams channel.</span></span> |
| <span data-ttu-id="7f357-114">replyChainMessageId</span><span class="sxs-lookup"><span data-stu-id="7f357-114">replyChainMessageId</span></span> | <span data-ttu-id="7f357-115">String</span><span class="sxs-lookup"><span data-stu-id="7f357-115">String</span></span>  | <span data-ttu-id="7f357-116">返信メッセージの ID です。</span><span class="sxs-lookup"><span data-stu-id="7f357-116">The ID of the reply message.</span></span> |
| <span data-ttu-id="7f357-117">スレッド Id</span><span class="sxs-lookup"><span data-stu-id="7f357-117">threadId</span></span>            | <span data-ttu-id="7f357-118">String</span><span class="sxs-lookup"><span data-stu-id="7f357-118">String</span></span>  | <span data-ttu-id="7f357-119">マイクロソフトのチームでのスレッドの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="7f357-119">The unique identifier for a thread in Microsoft Teams.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7f357-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7f357-120">JSON representation</span></span>

<span data-ttu-id="7f357-121">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7f357-121">The following is a JSON representation of the resource.</span></span>

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
