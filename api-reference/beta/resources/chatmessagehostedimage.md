---
title: chatMessageHostedImage リソースの種類
description: ChatMessage 内のホストされているイメージを表します。
localization_priority: Normal
author: clearab
ms.openlocfilehash: 1f7ce24dfae680937ecb1c43f9a34f6b9bb35646
ms.sourcegitcommit: b523648530fcc8c2a3ded35b419be8047b9fcd10
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/20/2019
ms.locfileid: "35085838"
---
# <a name="chatmessagehostedimage-resource-type"></a><span data-ttu-id="14da3-103">chatMessageHostedImage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="14da3-103">chatMessageHostedImage resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14da3-104">[Chatmessage](../resources/chatmessage.md)内のホストされているイメージを表します。</span><span class="sxs-lookup"><span data-stu-id="14da3-104">Represents a hosted image inside a [chatMessage](../resources/chatmessage.md).</span></span>

<span data-ttu-id="14da3-105">ホストされた画像は、メッセージの本文に表示されるイメージです\<。 img> タグの内容は、で`https://graph.microsoft.com`始まる src 属性を使用し**ます。**</span><span class="sxs-lookup"><span data-stu-id="14da3-105">Hosted images are the images that appear in the message's **body.content** in an \<img> tag with a src attribute that starts with `https://graph.microsoft.com`.</span></span>

<span data-ttu-id="14da3-106">メッセージ内の画像がホストされているわけではないため、Microsoft Teams も (img src 属性がパブリック web サイトをポイントする) パブリック画像をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="14da3-106">Not all images in a message are hosted images, Microsoft Teams also supports public images (where the img src attribute points to a public website).</span></span>

## <a name="methods"></a><span data-ttu-id="14da3-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="14da3-107">Methods</span></span>

| <span data-ttu-id="14da3-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="14da3-108">Method</span></span>       | <span data-ttu-id="14da3-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="14da3-109">Return Type</span></span>  |<span data-ttu-id="14da3-110">説明</span><span class="sxs-lookup"><span data-stu-id="14da3-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="14da3-111">ChatMessage 内の chatMessageHostedImages を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="14da3-111">List chatMessageHostedImages in a chatMessage</span></span>](../api/chatmessagehostedimage-list-hostedimages.md) | <span data-ttu-id="14da3-112">[Chatmessagehostedimage](chatmessagehostedimage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="14da3-112">[chatMessageHostedImage](chatmessagehostedimage.md) collection</span></span> | <span data-ttu-id="14da3-113">**Chatmessage**でホストされているすべての画像のリスト。</span><span class="sxs-lookup"><span data-stu-id="14da3-113">List of all hosted images in a **chatMessage**.</span></span>|
|[<span data-ttu-id="14da3-114">ChatMessageHostedImage を取得する</span><span class="sxs-lookup"><span data-stu-id="14da3-114">Get chatMessageHostedImage</span></span>](../api/chatmessagehostedimage-get.md) | [<span data-ttu-id="14da3-115">chatMessageHostedImage</span><span class="sxs-lookup"><span data-stu-id="14da3-115">chatMessageHostedImage</span></span>](chatmessagehostedimage.md) | <span data-ttu-id="14da3-116">1つのホストイメージを取得します。</span><span class="sxs-lookup"><span data-stu-id="14da3-116">Get a single hosted image.</span></span>|
|[<span data-ttu-id="14da3-117">chatMessageHostedImage: getBytes</span><span class="sxs-lookup"><span data-stu-id="14da3-117">chatMessageHostedImage: getBytes</span></span>](../api/chatmessagehostedimage-getbytes.md) | <span data-ttu-id="14da3-118">コンテンツタイプ: image/jpeg</span><span class="sxs-lookup"><span data-stu-id="14da3-118">Content-type: image/jpeg</span></span> | <span data-ttu-id="14da3-119">ホストされているイメージの生バイトを取得します。</span><span class="sxs-lookup"><span data-stu-id="14da3-119">Get the raw bytes of the hosted image.</span></span>|

## <a name="properties"></a><span data-ttu-id="14da3-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="14da3-120">Properties</span></span>

| <span data-ttu-id="14da3-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="14da3-121">Property</span></span>     | <span data-ttu-id="14da3-122">型</span><span class="sxs-lookup"><span data-stu-id="14da3-122">Type</span></span>   |<span data-ttu-id="14da3-123">説明</span><span class="sxs-lookup"><span data-stu-id="14da3-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="14da3-124">id</span><span class="sxs-lookup"><span data-stu-id="14da3-124">id</span></span>|<span data-ttu-id="14da3-125">String</span><span class="sxs-lookup"><span data-stu-id="14da3-125">String</span></span>| <span data-ttu-id="14da3-126">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="14da3-126">Read-only.</span></span> <span data-ttu-id="14da3-127">メッセージの一意の ID。</span><span class="sxs-lookup"><span data-stu-id="14da3-127">Unique ID of the message.</span></span>|
|<span data-ttu-id="14da3-128">URL</span><span class="sxs-lookup"><span data-stu-id="14da3-128">URL</span></span>| <span data-ttu-id="14da3-129">string</span><span class="sxs-lookup"><span data-stu-id="14da3-129">string</span></span> | <span data-ttu-id="14da3-130">画像コンテンツを取得する url。</span><span class="sxs-lookup"><span data-stu-id="14da3-130">The url to retrieve the image contents from.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="14da3-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="14da3-131">JSON representation</span></span>

<span data-ttu-id="14da3-132">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="14da3-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageHostedImage"
}-->

```json
{
  "id": "string (identifier)",
  "url": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chatmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
