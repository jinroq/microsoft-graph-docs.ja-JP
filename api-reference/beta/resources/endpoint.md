---
title: エンドポイント リソースの種類
description: 'エンドポイントでは、エンティティに関連付けられているリソースの Url を表します。  などの Office 365 の新しいグループが作成されると、追加のリソースは Office 365 のグループの一部として作成も。 会話のグループのメールボックスとドキュメントやファイル グループの OneDrive フォルダーのようなものが含まれます。 これでグループのリソースの種類の*エンドポイント*のナビゲーションを使用して、関連付けられているリソースの Url を含む、Office 365 グループ リソースに関する詳細な情報を読み取ることができます。 これにより、これらのリソースを理解し、自分の経験にも URL が発生したリソースを埋め込むアプリケーションことができます。 '
localization_priority: Normal
ms.openlocfilehash: 5a342bee0a1918eb142542693198173239d1b3c7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871286"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="686e1-107">エンドポイント リソースの種類</span><span class="sxs-lookup"><span data-stu-id="686e1-107">Endpoint resource type</span></span>

> <span data-ttu-id="686e1-108">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="686e1-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="686e1-109">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="686e1-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="686e1-110">エンドポイントでは、エンティティに関連付けられているリソースの Url を表します。</span><span class="sxs-lookup"><span data-stu-id="686e1-110">Endpoints represent URLs for resources associated with an entity.</span></span>  <span data-ttu-id="686e1-111">などの Office 365 の新しいグループが作成されると、追加のリソースは Office 365 のグループの一部として作成も。</span><span class="sxs-lookup"><span data-stu-id="686e1-111">For example, when a new Office 365 group is created, additional resources are also created as part of the Office 365 group.</span></span> <span data-ttu-id="686e1-112">会話のグループのメールボックスとドキュメントやファイル グループの OneDrive フォルダーのようなものが含まれます。</span><span class="sxs-lookup"><span data-stu-id="686e1-112">These include things like a group mailbox for conversations and a group OneDrive folder for documents and files.</span></span> <span data-ttu-id="686e1-113">これでグループのリソースの種類の*エンドポイント*のナビゲーションを使用して、関連付けられているリソースの Url を含む、Office 365 グループ リソースに関する詳細な情報を読み取ることができます。</span><span class="sxs-lookup"><span data-stu-id="686e1-113">Further information about these Office 365 group resources, including their associated resource URLs can now be read using the *endpoints* navigation on the group resource-type.</span></span> <span data-ttu-id="686e1-114">これにより、これらのリソースを理解し、自分の経験にも URL が発生したリソースを埋め込むアプリケーションことができます。</span><span class="sxs-lookup"><span data-stu-id="686e1-114">This allows applications to understand these resources, and even embed the resource URL experiences in their own experiences.</span></span> 

## <a name="methods"></a><span data-ttu-id="686e1-115">メソッド</span><span class="sxs-lookup"><span data-stu-id="686e1-115">Methods</span></span>

| <span data-ttu-id="686e1-116">メソッド</span><span class="sxs-lookup"><span data-stu-id="686e1-116">Method</span></span>           | <span data-ttu-id="686e1-117">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="686e1-117">Return Type</span></span>    |<span data-ttu-id="686e1-118">説明</span><span class="sxs-lookup"><span data-stu-id="686e1-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="686e1-119">エンドポイントのリスト</span><span class="sxs-lookup"><span data-stu-id="686e1-119">List endpoints</span></span>](../api/group-list-endpoints.md) |<span data-ttu-id="686e1-120">[エンドポイント](endpoint.md)のコレクション</span><span class="sxs-lookup"><span data-stu-id="686e1-120">[Endpoint](endpoint.md) collection</span></span>| <span data-ttu-id="686e1-121">エンドポイント オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="686e1-121">Get an endpoint object collection.</span></span> |
|[<span data-ttu-id="686e1-122">エンドポイントを取得します。</span><span class="sxs-lookup"><span data-stu-id="686e1-122">Get endpoint</span></span>](../api/endpoint-get.md) | [<span data-ttu-id="686e1-123">エンドポイント</span><span class="sxs-lookup"><span data-stu-id="686e1-123">Endpoint</span></span>](endpoint.md) |<span data-ttu-id="686e1-124">エンドポイント オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="686e1-124">Read properties and relationships of an endpoint object.</span></span>|

## <a name="properties"></a><span data-ttu-id="686e1-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="686e1-125">Properties</span></span>
| <span data-ttu-id="686e1-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="686e1-126">Property</span></span>     | <span data-ttu-id="686e1-127">種類</span><span class="sxs-lookup"><span data-stu-id="686e1-127">Type</span></span>   |<span data-ttu-id="686e1-128">説明</span><span class="sxs-lookup"><span data-stu-id="686e1-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="686e1-129">capability</span><span class="sxs-lookup"><span data-stu-id="686e1-129">capability</span></span>     | <span data-ttu-id="686e1-130">String</span><span class="sxs-lookup"><span data-stu-id="686e1-130">String</span></span>  | <span data-ttu-id="686e1-131">このリソースに関連付けられている機能をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="686e1-131">Describes the capability that is associated with this resource.</span></span> <span data-ttu-id="686e1-132">(例: メッセージ、会話など) Null を許容しません。</span><span class="sxs-lookup"><span data-stu-id="686e1-132">(e.g. Messages, Conversations, etc.)  Not nullable.</span></span> <span data-ttu-id="686e1-133">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="686e1-133">Read-only.</span></span> |
| <span data-ttu-id="686e1-134">id</span><span class="sxs-lookup"><span data-stu-id="686e1-134">id</span></span>             | <span data-ttu-id="686e1-135">String</span><span class="sxs-lookup"><span data-stu-id="686e1-135">String</span></span>  | <span data-ttu-id="686e1-136">エンドポイントの一意の識別子キーです。</span><span class="sxs-lookup"><span data-stu-id="686e1-136">Unique identifier for the endpoint; Key.</span></span> <span data-ttu-id="686e1-137">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="686e1-137">Not nullable.</span></span> <span data-ttu-id="686e1-138">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="686e1-138">Read-only.</span></span>|
| <span data-ttu-id="686e1-139">providerId</span><span class="sxs-lookup"><span data-stu-id="686e1-139">providerId</span></span>     | <span data-ttu-id="686e1-140">String</span><span class="sxs-lookup"><span data-stu-id="686e1-140">String</span></span>  | <span data-ttu-id="686e1-141">アプリケーション id が公開するサービスの基になるのです。</span><span class="sxs-lookup"><span data-stu-id="686e1-141">Application id of the publishing underlying service.</span></span> <span data-ttu-id="686e1-142">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="686e1-142">Not nullable.</span></span> <span data-ttu-id="686e1-143">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="686e1-143">Read-only.</span></span>|
| <span data-ttu-id="686e1-144">プロバイダー</span><span class="sxs-lookup"><span data-stu-id="686e1-144">providerName</span></span>   | <span data-ttu-id="686e1-145">String</span><span class="sxs-lookup"><span data-stu-id="686e1-145">String</span></span>  | <span data-ttu-id="686e1-146">公開するサービスの基になるの名前です。</span><span class="sxs-lookup"><span data-stu-id="686e1-146">Name of the publishing underlying service.</span></span> <span data-ttu-id="686e1-147">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="686e1-147">Read-only.</span></span>|
| <span data-ttu-id="686e1-148">providerResourceId</span><span class="sxs-lookup"><span data-stu-id="686e1-148">providerResourceId</span></span>|<span data-ttu-id="686e1-149">String</span><span class="sxs-lookup"><span data-stu-id="686e1-149">String</span></span>| <span data-ttu-id="686e1-150">Office 365 グループでは、この処理は、リソース (たとえば Yammer.FeedURL など) の既知の名前に設定されます。</span><span class="sxs-lookup"><span data-stu-id="686e1-150">For Office 365 groups, this is set to a well-known name for the resource (e.g. Yammer.FeedURL etc.).</span></span> <span data-ttu-id="686e1-151">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="686e1-151">Not nullable.</span></span> <span data-ttu-id="686e1-152">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="686e1-152">Read-only.</span></span>|
| <span data-ttu-id="686e1-153">uri</span><span class="sxs-lookup"><span data-stu-id="686e1-153">uri</span></span>            | <span data-ttu-id="686e1-154">String</span><span class="sxs-lookup"><span data-stu-id="686e1-154">String</span></span>  | <span data-ttu-id="686e1-155">公開されたリソースの URL です。</span><span class="sxs-lookup"><span data-stu-id="686e1-155">URL of the published resource.</span></span> <span data-ttu-id="686e1-156">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="686e1-156">Not nullable.</span></span> <span data-ttu-id="686e1-157">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="686e1-157">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="686e1-158">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="686e1-158">Relationships</span></span>

<span data-ttu-id="686e1-159">なし。</span><span class="sxs-lookup"><span data-stu-id="686e1-159">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="686e1-160">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="686e1-160">JSON representation</span></span>
<span data-ttu-id="686e1-161">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="686e1-161">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.Endpoint"
}-->

```json
{
  "capability": "String",
  "id": "String (identifier)",
  "providerId": "String",
  "providerName": "String",
  "providerResourceId": "String",
  "uri": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Endpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
