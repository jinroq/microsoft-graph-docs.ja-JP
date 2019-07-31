---
title: エンドポイントリソースの種類
description: 'エンドポイントは、エンティティに関連付けられているリソースの Url を表します。  たとえば、新しい Office 365 グループを作成すると、その他のリソースも Office 365 グループの一部として作成されます。 これには、会話のグループメールボックスや、ドキュメントやファイルのグループ OneDrive フォルダーなどが含まれます。 これらの Office 365 グループリソースの詳細については、「グループリソースの種類の*エンドポイント*ナビゲーションを使用して、関連付けられたリソース url」を参照してください。 これにより、アプリケーションはこれらのリソースを理解し、リソース URL エクスペリエンスを独自のエクスペリエンスに埋め込むこともできます。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: db9904c4c668ff86e56be85835c2752ab0d17525
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972125"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="d9daf-107">エンドポイントリソースの種類</span><span class="sxs-lookup"><span data-stu-id="d9daf-107">Endpoint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9daf-108">エンドポイントは、エンティティに関連付けられているリソースの Url を表します。</span><span class="sxs-lookup"><span data-stu-id="d9daf-108">Endpoints represent URLs for resources associated with an entity.</span></span>  <span data-ttu-id="d9daf-109">たとえば、新しい Office 365 グループを作成すると、その他のリソースも Office 365 グループの一部として作成されます。</span><span class="sxs-lookup"><span data-stu-id="d9daf-109">For example, when a new Office 365 group is created, additional resources are also created as part of the Office 365 group.</span></span> <span data-ttu-id="d9daf-110">これには、会話のグループメールボックスや、ドキュメントやファイルのグループ OneDrive フォルダーなどが含まれます。</span><span class="sxs-lookup"><span data-stu-id="d9daf-110">These include things like a group mailbox for conversations and a group OneDrive folder for documents and files.</span></span> <span data-ttu-id="d9daf-111">これらの Office 365 グループリソースの詳細については、「グループリソースの種類の*エンドポイント*ナビゲーションを使用して、関連付けられたリソース url」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d9daf-111">Further information about these Office 365 group resources, including their associated resource URLs can now be read using the *endpoints* navigation on the group resource-type.</span></span> <span data-ttu-id="d9daf-112">これにより、アプリケーションはこれらのリソースを理解し、リソース URL エクスペリエンスを独自のエクスペリエンスに埋め込むこともできます。</span><span class="sxs-lookup"><span data-stu-id="d9daf-112">This allows applications to understand these resources, and even embed the resource URL experiences in their own experiences.</span></span> 

## <a name="methods"></a><span data-ttu-id="d9daf-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="d9daf-113">Methods</span></span>

| <span data-ttu-id="d9daf-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="d9daf-114">Method</span></span>           | <span data-ttu-id="d9daf-115">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d9daf-115">Return Type</span></span>    |<span data-ttu-id="d9daf-116">説明</span><span class="sxs-lookup"><span data-stu-id="d9daf-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d9daf-117">エンドポイントを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="d9daf-117">List endpoints</span></span>](../api/group-list-endpoints.md) |<span data-ttu-id="d9daf-118">[Endpoint](endpoint.md) collection</span><span class="sxs-lookup"><span data-stu-id="d9daf-118">[Endpoint](endpoint.md) collection</span></span>| <span data-ttu-id="d9daf-119">endpoint オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="d9daf-119">Get an endpoint object collection.</span></span> |
|[<span data-ttu-id="d9daf-120">エンドポイントを取得する</span><span class="sxs-lookup"><span data-stu-id="d9daf-120">Get endpoint</span></span>](../api/endpoint-get.md) | [<span data-ttu-id="d9daf-121">エンドポイント</span><span class="sxs-lookup"><span data-stu-id="d9daf-121">Endpoint</span></span>](endpoint.md) |<span data-ttu-id="d9daf-122">endpoint オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d9daf-122">Read properties and relationships of an endpoint object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d9daf-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d9daf-123">Properties</span></span>
| <span data-ttu-id="d9daf-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d9daf-124">Property</span></span>     | <span data-ttu-id="d9daf-125">型</span><span class="sxs-lookup"><span data-stu-id="d9daf-125">Type</span></span>   |<span data-ttu-id="d9daf-126">説明</span><span class="sxs-lookup"><span data-stu-id="d9daf-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d9daf-127">capability</span><span class="sxs-lookup"><span data-stu-id="d9daf-127">capability</span></span>     | <span data-ttu-id="d9daf-128">String</span><span class="sxs-lookup"><span data-stu-id="d9daf-128">String</span></span>  | <span data-ttu-id="d9daf-129">このリソースに関連付けられている機能について説明します。</span><span class="sxs-lookup"><span data-stu-id="d9daf-129">Describes the capability that is associated with this resource.</span></span> <span data-ttu-id="d9daf-130">(例: メッセージ、会話など) Null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="d9daf-130">(e.g. Messages, Conversations, etc.)  Not nullable.</span></span> <span data-ttu-id="d9daf-131">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d9daf-131">Read-only.</span></span> |
| <span data-ttu-id="d9daf-132">id</span><span class="sxs-lookup"><span data-stu-id="d9daf-132">id</span></span>             | <span data-ttu-id="d9daf-133">String</span><span class="sxs-lookup"><span data-stu-id="d9daf-133">String</span></span>  | <span data-ttu-id="d9daf-134">エンドポイントの一意の識別子。要点.</span><span class="sxs-lookup"><span data-stu-id="d9daf-134">Unique identifier for the endpoint; Key.</span></span> <span data-ttu-id="d9daf-135">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="d9daf-135">Not nullable.</span></span> <span data-ttu-id="d9daf-136">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d9daf-136">Read-only.</span></span>|
| <span data-ttu-id="d9daf-137">providerId</span><span class="sxs-lookup"><span data-stu-id="d9daf-137">providerId</span></span>     | <span data-ttu-id="d9daf-138">String</span><span class="sxs-lookup"><span data-stu-id="d9daf-138">String</span></span>  | <span data-ttu-id="d9daf-139">発行元のサービスのアプリケーション id。</span><span class="sxs-lookup"><span data-stu-id="d9daf-139">Application id of the publishing underlying service.</span></span> <span data-ttu-id="d9daf-140">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="d9daf-140">Not nullable.</span></span> <span data-ttu-id="d9daf-141">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d9daf-141">Read-only.</span></span>|
| <span data-ttu-id="d9daf-142">プロバイダー</span><span class="sxs-lookup"><span data-stu-id="d9daf-142">providerName</span></span>   | <span data-ttu-id="d9daf-143">String</span><span class="sxs-lookup"><span data-stu-id="d9daf-143">String</span></span>  | <span data-ttu-id="d9daf-144">発行元のサービスの名前。</span><span class="sxs-lookup"><span data-stu-id="d9daf-144">Name of the publishing underlying service.</span></span> <span data-ttu-id="d9daf-145">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d9daf-145">Read-only.</span></span>|
| <span data-ttu-id="d9daf-146">providerResourceId</span><span class="sxs-lookup"><span data-stu-id="d9daf-146">providerResourceId</span></span>|<span data-ttu-id="d9daf-147">String</span><span class="sxs-lookup"><span data-stu-id="d9daf-147">String</span></span>| <span data-ttu-id="d9daf-148">Office 365 グループの場合は、リソースの既知の名前 (たとえば、FeedURL など) に設定されます。</span><span class="sxs-lookup"><span data-stu-id="d9daf-148">For Office 365 groups, this is set to a well-known name for the resource (e.g. Yammer.FeedURL etc.).</span></span> <span data-ttu-id="d9daf-149">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="d9daf-149">Not nullable.</span></span> <span data-ttu-id="d9daf-150">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d9daf-150">Read-only.</span></span>|
| <span data-ttu-id="d9daf-151">uri</span><span class="sxs-lookup"><span data-stu-id="d9daf-151">uri</span></span>            | <span data-ttu-id="d9daf-152">String</span><span class="sxs-lookup"><span data-stu-id="d9daf-152">String</span></span>  | <span data-ttu-id="d9daf-153">発行されたリソースの URL。</span><span class="sxs-lookup"><span data-stu-id="d9daf-153">URL of the published resource.</span></span> <span data-ttu-id="d9daf-154">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="d9daf-154">Not nullable.</span></span> <span data-ttu-id="d9daf-155">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d9daf-155">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9daf-156">関係</span><span class="sxs-lookup"><span data-stu-id="d9daf-156">Relationships</span></span>

<span data-ttu-id="d9daf-157">なし。</span><span class="sxs-lookup"><span data-stu-id="d9daf-157">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="d9daf-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d9daf-158">JSON representation</span></span>
<span data-ttu-id="d9daf-159">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d9daf-159">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.endpoint"
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
<!--
{
  "type": "#page.annotation",
  "description": "Endpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
