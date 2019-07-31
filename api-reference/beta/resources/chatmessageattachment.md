---
title: chatMessageAttachment リソースの種類
description: チャットメッセージエンティティへの添付ファイルを表します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 93034cb504f67b68045afb2de4533d11c963efb4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973483"
---
# <a name="chatmessageattachment-resource-type"></a><span data-ttu-id="3457b-103">chatMessageAttachment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3457b-103">chatMessageAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3457b-104">チャットメッセージエンティティへの添付ファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="3457b-104">Represents an attachment to a chat message entity.</span></span>

<span data-ttu-id="3457b-105">型`chatMessageAttachment`のエンティティは、 [chatmessage](chatmessage.md)エンティティの一部として、 [Get channel messages](../api/channel-list-messages.md) API の一部として返されます。</span><span class="sxs-lookup"><span data-stu-id="3457b-105">An entity of type `chatMessageAttachment` is returned as part of the [Get channel messages](../api/channel-list-messages.md) API, as a part of [chatMessage](chatmessage.md) entity.</span></span>

## <a name="properties"></a><span data-ttu-id="3457b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3457b-106">Properties</span></span>
| <span data-ttu-id="3457b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3457b-107">Property</span></span>     | <span data-ttu-id="3457b-108">型</span><span class="sxs-lookup"><span data-stu-id="3457b-108">Type</span></span>   |<span data-ttu-id="3457b-109">説明</span><span class="sxs-lookup"><span data-stu-id="3457b-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3457b-110">id</span><span class="sxs-lookup"><span data-stu-id="3457b-110">id</span></span>|<span data-ttu-id="3457b-111">string</span><span class="sxs-lookup"><span data-stu-id="3457b-111">string</span></span>| <span data-ttu-id="3457b-112">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="3457b-112">Read-only.</span></span> <span data-ttu-id="3457b-113">添付ファイルの一意の id です。</span><span class="sxs-lookup"><span data-stu-id="3457b-113">Unique id of the attachment.</span></span>|
|<span data-ttu-id="3457b-114">contentType</span><span class="sxs-lookup"><span data-stu-id="3457b-114">contentType</span></span>| <span data-ttu-id="3457b-115">string</span><span class="sxs-lookup"><span data-stu-id="3457b-115">string</span></span> | <span data-ttu-id="3457b-116">コンテンツの添付ファイルのメディアの種類。</span><span class="sxs-lookup"><span data-stu-id="3457b-116">The media type of the content attachment.</span></span> <span data-ttu-id="3457b-117">次の値を指定できます。</span><span class="sxs-lookup"><span data-stu-id="3457b-117">It can have the following values:</span></span> <br><ul><li><span data-ttu-id="3457b-118">参照: Attachment は、別のファイルへのリンクです。</span><span class="sxs-lookup"><span data-stu-id="3457b-118">reference: Attachment is a link to another file.</span></span> <span data-ttu-id="3457b-119">ContentURL に、オブジェクトへのリンクを設定します。</span><span class="sxs-lookup"><span data-stu-id="3457b-119">Populate the contentURL with the link to the object.</span></span><br></li><li><span data-ttu-id="3457b-120">ファイル: Raw ファイル添付ファイル。</span><span class="sxs-lookup"><span data-stu-id="3457b-120">file: Raw file attachment.</span></span> <span data-ttu-id="3457b-121">Contenturl フィールドに、data: 形式のファイルの base64 エンコードを設定します。</span><span class="sxs-lookup"><span data-stu-id="3457b-121">Populate the contenturl field with the base64 encoding of the file in data: format.</span></span><br></li><li><span data-ttu-id="3457b-122">画像/: 画像の種類 (画像/png、画像/jpeg、画像/gif) を指定した画像の種類。</span><span class="sxs-lookup"><span data-stu-id="3457b-122">image/: Image type with the type of the image specified ex: image/png, image/jpeg, image/gif.</span></span> <span data-ttu-id="3457b-123">ContentUrl フィールドに、data: 形式のファイルの base64 エンコードを設定します。</span><span class="sxs-lookup"><span data-stu-id="3457b-123">Populate the contentUrl field with the base64 encoding of the file in data: format.</span></span><br></li><li><span data-ttu-id="3457b-124">ビデオ/: 形式が指定されたビデオの種類。</span><span class="sxs-lookup"><span data-stu-id="3457b-124">video/: Video type with the format specified.</span></span> <span data-ttu-id="3457b-125">Ex: video/mp4。</span><span class="sxs-lookup"><span data-stu-id="3457b-125">Ex: video/mp4.</span></span> <span data-ttu-id="3457b-126">ContentUrl フィールドに、data: 形式のファイルの base64 エンコードを設定します。</span><span class="sxs-lookup"><span data-stu-id="3457b-126">Populate the contentUrl field with the base64 encoding of the file in data: format.</span></span><br></li><li><span data-ttu-id="3457b-127">audio/: 指定された形式のオーディオタイプ。</span><span class="sxs-lookup"><span data-stu-id="3457b-127">audio/: Audio type with the format specified.</span></span> <span data-ttu-id="3457b-128">Ex: 音声/wmw</span><span class="sxs-lookup"><span data-stu-id="3457b-128">Ex: audio/wmw.</span></span> <span data-ttu-id="3457b-129">ContentUrl フィールドに、data: 形式のファイルの base64 エンコードを設定します。</span><span class="sxs-lookup"><span data-stu-id="3457b-129">Populate the contentUrl field with the base64 encoding of the file in data: format.</span></span><br></li><li><span data-ttu-id="3457b-130">アプリケーション/カードの種類: カードの種類がリッチカードの添付ファイルで、使用する正確なカード形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="3457b-130">application/card type: Rich card attachment type with the card type specifying the exact card format to use.</span></span> <span data-ttu-id="3457b-131">カードの json 形式でコンテンツを設定します。</span><span class="sxs-lookup"><span data-stu-id="3457b-131">Set content with the json format of the card.</span></span> <span data-ttu-id="3457b-132">カード型でサポートされている値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="3457b-132">Supported values for card type include:</span></span><br><ul><li><span data-ttu-id="3457b-133">application/vnd: テキスト、音声、画像、ボタン、および入力フィールドの任意の組み合わせを含むことができるリッチカード。</span><span class="sxs-lookup"><span data-stu-id="3457b-133">application/vnd.microsoft.card.adaptive: A rich card that can contain any combination of text, speech, images,,buttons, and input fields.</span></span> <span data-ttu-id="3457b-134">Content プロパティを、AdaptiveCard オブジェクトに設定します。</span><span class="sxs-lookup"><span data-stu-id="3457b-134">Set the content property to,an AdaptiveCard object.</span></span></li><li><span data-ttu-id="3457b-135">アプリケーション/vnd。アニメーション: アニメーションを再生するリッチカード。</span><span class="sxs-lookup"><span data-stu-id="3457b-135">application/vnd.microsoft.card.animation: A rich card that plays animation.</span></span> <span data-ttu-id="3457b-136">コンテンツプロパティを、アニメーションの Cardobject に設定します。</span><span class="sxs-lookup"><span data-stu-id="3457b-136">Set the content property,to an AnimationCardobject.</span></span></li><li><span data-ttu-id="3457b-137">application/vnd audio: オーディオファイルを再生するリッチカード。</span><span class="sxs-lookup"><span data-stu-id="3457b-137">application/vnd.microsoft.card.audio: A rich card that plays audio files.</span></span> <span data-ttu-id="3457b-138">Content プロパティを AudioCard オブジェクトに設定します。</span><span class="sxs-lookup"><span data-stu-id="3457b-138">Set the content property,to an AudioCard object.</span></span></li><li><span data-ttu-id="3457b-139">application/vnd ビデオ: ビデオを再生するリッチカード。</span><span class="sxs-lookup"><span data-stu-id="3457b-139">application/vnd.microsoft.card.video: A rich card that plays videos.</span></span> <span data-ttu-id="3457b-140">Content プロパティを VideoCard オブジェクトに設定します。</span><span class="sxs-lookup"><span data-stu-id="3457b-140">Set the content property,to a VideoCard object.</span></span></li><li><span data-ttu-id="3457b-141">アプリケーション/vnd。ヒーロー: 英雄カード。</span><span class="sxs-lookup"><span data-stu-id="3457b-141">application/vnd.microsoft.card.hero: A Hero card.</span></span> <span data-ttu-id="3457b-142">Content プロパティを HeroCard オブジェクトに設定します。</span><span class="sxs-lookup"><span data-stu-id="3457b-142">Set the content property to a HeroCard object.</span></span></li><li><span data-ttu-id="3457b-143">application/vnd-サムネイルカード: サムネイルカード。</span><span class="sxs-lookup"><span data-stu-id="3457b-143">application/vnd.microsoft.card.thumbnail: A Thumbnail card.</span></span> <span data-ttu-id="3457b-144">Content プロパティを ThumbnailCard オブジェクトに設定します。</span><span class="sxs-lookup"><span data-stu-id="3457b-144">Set the content property to a ThumbnailCard object.</span></span></li><li><span data-ttu-id="3457b-145">アプリケーション/vnd。領収書: 領収書カード。</span><span class="sxs-lookup"><span data-stu-id="3457b-145">application/vnd.microsoft.com.card.receipt: A Receipt card.</span></span> <span data-ttu-id="3457b-146">Content プロパティを ReceiptCard オブジェクトに設定します。</span><span class="sxs-lookup"><span data-stu-id="3457b-146">Set the content property to a ReceiptCard object.</span></span></li><li><span data-ttu-id="3457b-147">アプリケーション/vnd: ユーザーがサインインカードをサインインします。</span><span class="sxs-lookup"><span data-stu-id="3457b-147">application/vnd.microsoft.com.card.signin: A user Sign In card.</span></span> <span data-ttu-id="3457b-148">Content プロパティを SignInCard オブジェクトに設定します。</span><span class="sxs-lookup"><span data-stu-id="3457b-148">Set the content property to a SignInCard object.</span></span></ul></ul>|
|<span data-ttu-id="3457b-149">contentUrl</span><span class="sxs-lookup"><span data-stu-id="3457b-149">contentUrl</span></span>|<span data-ttu-id="3457b-150">文字列</span><span class="sxs-lookup"><span data-stu-id="3457b-150">string</span></span>|<span data-ttu-id="3457b-151">添付ファイルのコンテンツの URL。</span><span class="sxs-lookup"><span data-stu-id="3457b-151">URL for the content of the attachment.</span></span> <span data-ttu-id="3457b-152">サポートされているプロトコル: http、https、ファイル、およびデータ。</span><span class="sxs-lookup"><span data-stu-id="3457b-152">Supported protocols: http, https, file and data.</span></span>|
|<span data-ttu-id="3457b-153">content</span><span class="sxs-lookup"><span data-stu-id="3457b-153">content</span></span>|<span data-ttu-id="3457b-154">string</span><span class="sxs-lookup"><span data-stu-id="3457b-154">string</span></span>|<span data-ttu-id="3457b-155">添付ファイルの内容。</span><span class="sxs-lookup"><span data-stu-id="3457b-155">The content of the attachment.</span></span> <span data-ttu-id="3457b-156">添付ファイルがリッチカードの場合は、プロパティをリッチカードオブジェクトに設定します。</span><span class="sxs-lookup"><span data-stu-id="3457b-156">If the attachment is a rich card, set the property to the rich card object.</span></span> <span data-ttu-id="3457b-157">このプロパティと contentUrl は相互に排他的です。</span><span class="sxs-lookup"><span data-stu-id="3457b-157">This property and contentUrl are mutually exclusive.</span></span>|
|<span data-ttu-id="3457b-158">name</span><span class="sxs-lookup"><span data-stu-id="3457b-158">name</span></span>|<span data-ttu-id="3457b-159">string</span><span class="sxs-lookup"><span data-stu-id="3457b-159">string</span></span>|<span data-ttu-id="3457b-160">添付ファイルの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="3457b-160">Name of the attachment.</span></span>|
|<span data-ttu-id="3457b-161">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="3457b-161">thumbnailUrl</span></span>| <span data-ttu-id="3457b-162">string</span><span class="sxs-lookup"><span data-stu-id="3457b-162">string</span></span> |<span data-ttu-id="3457b-163">別の小さな形式のコンテンツまたは contentUrl を使用してサポートされている場合に、チャネルが使用できるサムネイルイメージの URL。</span><span class="sxs-lookup"><span data-stu-id="3457b-163">URL to a thumbnail image that the channel can use if it supports using an alternative, smaller form of content or contentUrl.</span></span> <span data-ttu-id="3457b-164">たとえば、contentType を application/word に設定して、contentUrl を Word 文書の場所に設定した場合、ドキュメントを表すサムネイルイメージを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="3457b-164">For example, if you set contentType to application/word and set contentUrl to the location of the Word document, you might include a thumbnail image that represents the document.</span></span> <span data-ttu-id="3457b-165">チャネルは、ドキュメントの代わりにサムネイルイメージを表示することができます。</span><span class="sxs-lookup"><span data-stu-id="3457b-165">The channel could display the thumbnail image instead of the document.</span></span> <span data-ttu-id="3457b-166">ユーザーが画像をクリックすると、チャネルはドキュメントを開きます。</span><span class="sxs-lookup"><span data-stu-id="3457b-166">When the user clicks the image, the channel would open the document.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3457b-167">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3457b-167">JSON representation</span></span>
 <span data-ttu-id="3457b-168">リソースの JSON 表記を次に示します</span><span class="sxs-lookup"><span data-stu-id="3457b-168">The following is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "thumbnailUrl",
    "content",
    "contentUrl"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chatMessageAttachment"
}-->

```json
{
  "id": "string (identifier)",
  "contentType": "string",
  "contentUrl": "string",
  "content": "string",
  "name": "string",
  "thumbnailUrl": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
