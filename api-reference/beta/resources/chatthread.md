---
title: chatThread リソース型
description: ChatThread は、Microsoft Teams における chatMessages のコレクションです。
localization_priority: Priority
ms.openlocfilehash: a85b6aea6c48c9295fe88a7412fa7e6b96ee1d3f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521342"
---
# <a name="chatthread-resource-type"></a><span data-ttu-id="2a471-103">chatThread リソース型</span><span class="sxs-lookup"><span data-stu-id="2a471-103">chatThread resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a471-104">chatThread は、Microsoft Teams における [chatMessages](chatmessage.md) のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="2a471-104">A chatThread is a collection of [chatMessages](chatmessage.md) in Microsoft Teams.</span></span>

> <span data-ttu-id="2a471-105">現在のところ、ChatThreads は[チャネル内で作成](../api/channel-post-chatthreads.md)できます。</span><span class="sxs-lookup"><span data-stu-id="2a471-105">Currently, chatThreads can be [created in channels](../api/channel-post-chatthreads.md).</span></span>  <span data-ttu-id="2a471-106">API の今後のリリースでは、既存の chatThreads の読み取りに加えて、チームやチャネルの範囲外のユーザー間での直接チャットの読み取り/書き込みをサポートします。</span><span class="sxs-lookup"><span data-stu-id="2a471-106">Future API releases will support reading existing chatThreads, as well as reading/writing direct chats between users that are outside the scope of a team or channel.</span></span>

## <a name="methods"></a><span data-ttu-id="2a471-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="2a471-107">Methods</span></span>

| <span data-ttu-id="2a471-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="2a471-108">Method</span></span>       | <span data-ttu-id="2a471-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2a471-109">Return Type</span></span>  |<span data-ttu-id="2a471-110">説明</span><span class="sxs-lookup"><span data-stu-id="2a471-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2a471-111">Create thread</span><span class="sxs-lookup"><span data-stu-id="2a471-111">Create thread</span></span>](../api/channel-post-chatthreads.md) | [<span data-ttu-id="2a471-112">chatThread</span><span class="sxs-lookup"><span data-stu-id="2a471-112">chatThread</span></span>](chatthread.md) |<span data-ttu-id="2a471-113">最初のメッセージを指定して、指定したチャネルで新しいスレッドを開始します。</span><span class="sxs-lookup"><span data-stu-id="2a471-113">Start a new thread in the specified channel, providing the first message.</span></span>|

## <a name="properties"></a><span data-ttu-id="2a471-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2a471-114">Properties</span></span>
| <span data-ttu-id="2a471-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2a471-115">Property</span></span>     | <span data-ttu-id="2a471-116">型</span><span class="sxs-lookup"><span data-stu-id="2a471-116">Type</span></span>   |<span data-ttu-id="2a471-117">説明</span><span class="sxs-lookup"><span data-stu-id="2a471-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2a471-118">id</span><span class="sxs-lookup"><span data-stu-id="2a471-118">id</span></span>|<span data-ttu-id="2a471-119">String</span><span class="sxs-lookup"><span data-stu-id="2a471-119">String</span></span>| <span data-ttu-id="2a471-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2a471-120">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a471-121">関係</span><span class="sxs-lookup"><span data-stu-id="2a471-121">Relationships</span></span>
| <span data-ttu-id="2a471-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2a471-122">Relationship</span></span> | <span data-ttu-id="2a471-123">型</span><span class="sxs-lookup"><span data-stu-id="2a471-123">Type</span></span>   |<span data-ttu-id="2a471-124">説明</span><span class="sxs-lookup"><span data-stu-id="2a471-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2a471-125">rootMessage</span><span class="sxs-lookup"><span data-stu-id="2a471-125">rootMessage</span></span>|[<span data-ttu-id="2a471-126">chatMessage</span><span class="sxs-lookup"><span data-stu-id="2a471-126">chatMessage</span></span>](chatmessage.md)| <span data-ttu-id="2a471-127">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="2a471-127">Nullable.</span></span>|
|<span data-ttu-id="2a471-128">chatMessages</span><span class="sxs-lookup"><span data-stu-id="2a471-128">chatMessages</span></span>|<span data-ttu-id="2a471-129">[chatMessage](chatmessage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2a471-129">[chatMessage](chatmessage.md) collection</span></span>| <span data-ttu-id="2a471-130">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="2a471-130">Nullable.</span></span>|

> <span data-ttu-id="2a471-131">現在、これらの関係は暗黙的に存在しますが、読み取り/書き込みはできません。</span><span class="sxs-lookup"><span data-stu-id="2a471-131">Currently these relationships exist implicitly, but cannot read or written.</span></span>  <span data-ttu-id="2a471-132">将来的に、ベータ版の API リリースでこの機能がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="2a471-132">Future beta API releases will support this.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2a471-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2a471-133">JSON representation</span></span>

<span data-ttu-id="2a471-134">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="2a471-134">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "posts"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatThread"
}-->

```json
{
  "id": "string (identifier)"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chatThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chatthread.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
