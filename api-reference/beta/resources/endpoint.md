---
title: エンドポイント リソースの種類
description: 'エンドポイントでは、エンティティに関連付けられているリソースの Url を表します。  などの Office 365 の新しいグループが作成されると、追加のリソースは Office 365 のグループの一部として作成も。 会話のグループのメールボックスとドキュメントやファイル グループの OneDrive フォルダーのようなものが含まれます。 これでグループのリソースの種類の*エンドポイント*のナビゲーションを使用して、関連付けられているリソースの Url を含む、Office 365 グループ リソースに関する詳細な情報を読み取ることができます。 これにより、これらのリソースを理解し、自分の経験にも URL が発生したリソースを埋め込むアプリケーションことができます。 '
localization_priority: Normal
ms.openlocfilehash: 6f923cdeb34ec0845d776a67f51db490256ec718
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512060"
---
# <a name="endpoint-resource-type"></a><span data-ttu-id="0e461-107">エンドポイント リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0e461-107">Endpoint resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e461-108">エンドポイントでは、エンティティに関連付けられているリソースの Url を表します。</span><span class="sxs-lookup"><span data-stu-id="0e461-108">Endpoints represent URLs for resources associated with an entity.</span></span>  <span data-ttu-id="0e461-109">などの Office 365 の新しいグループが作成されると、追加のリソースは Office 365 のグループの一部として作成も。</span><span class="sxs-lookup"><span data-stu-id="0e461-109">For example, when a new Office 365 group is created, additional resources are also created as part of the Office 365 group.</span></span> <span data-ttu-id="0e461-110">会話のグループのメールボックスとドキュメントやファイル グループの OneDrive フォルダーのようなものが含まれます。</span><span class="sxs-lookup"><span data-stu-id="0e461-110">These include things like a group mailbox for conversations and a group OneDrive folder for documents and files.</span></span> <span data-ttu-id="0e461-111">これでグループのリソースの種類の*エンドポイント*のナビゲーションを使用して、関連付けられているリソースの Url を含む、Office 365 グループ リソースに関する詳細な情報を読み取ることができます。</span><span class="sxs-lookup"><span data-stu-id="0e461-111">Further information about these Office 365 group resources, including their associated resource URLs can now be read using the *endpoints* navigation on the group resource-type.</span></span> <span data-ttu-id="0e461-112">これにより、これらのリソースを理解し、自分の経験にも URL が発生したリソースを埋め込むアプリケーションことができます。</span><span class="sxs-lookup"><span data-stu-id="0e461-112">This allows applications to understand these resources, and even embed the resource URL experiences in their own experiences.</span></span> 

## <a name="methods"></a><span data-ttu-id="0e461-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="0e461-113">Methods</span></span>

| <span data-ttu-id="0e461-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="0e461-114">Method</span></span>           | <span data-ttu-id="0e461-115">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0e461-115">Return Type</span></span>    |<span data-ttu-id="0e461-116">説明</span><span class="sxs-lookup"><span data-stu-id="0e461-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0e461-117">エンドポイントを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="0e461-117">List endpoints</span></span>](../api/group-list-endpoints.md) |<span data-ttu-id="0e461-118">[Endpoint](endpoint.md) collection</span><span class="sxs-lookup"><span data-stu-id="0e461-118">[Endpoint](endpoint.md) collection</span></span>| <span data-ttu-id="0e461-119">endpoint オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="0e461-119">Get an endpoint object collection.</span></span> |
|[<span data-ttu-id="0e461-120">エンドポイントを取得する</span><span class="sxs-lookup"><span data-stu-id="0e461-120">Get endpoint</span></span>](../api/endpoint-get.md) | [<span data-ttu-id="0e461-121">エンドポイント</span><span class="sxs-lookup"><span data-stu-id="0e461-121">Endpoint</span></span>](endpoint.md) |<span data-ttu-id="0e461-122">endpoint オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0e461-122">Read properties and relationships of an endpoint object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0e461-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e461-123">Properties</span></span>
| <span data-ttu-id="0e461-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e461-124">Property</span></span>     | <span data-ttu-id="0e461-125">型</span><span class="sxs-lookup"><span data-stu-id="0e461-125">Type</span></span>   |<span data-ttu-id="0e461-126">説明</span><span class="sxs-lookup"><span data-stu-id="0e461-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0e461-127">capability</span><span class="sxs-lookup"><span data-stu-id="0e461-127">capability</span></span>     | <span data-ttu-id="0e461-128">String</span><span class="sxs-lookup"><span data-stu-id="0e461-128">String</span></span>  | <span data-ttu-id="0e461-129">このリソースに関連付けられている機能をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="0e461-129">Describes the capability that is associated with this resource.</span></span> <span data-ttu-id="0e461-130">(例: メッセージ、会話など) Null を許容しません。</span><span class="sxs-lookup"><span data-stu-id="0e461-130">(e.g. Messages, Conversations, etc.)  Not nullable.</span></span> <span data-ttu-id="0e461-131">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0e461-131">Read-only.</span></span> |
| <span data-ttu-id="0e461-132">id</span><span class="sxs-lookup"><span data-stu-id="0e461-132">id</span></span>             | <span data-ttu-id="0e461-133">String</span><span class="sxs-lookup"><span data-stu-id="0e461-133">String</span></span>  | <span data-ttu-id="0e461-134">エンドポイントの一意の識別子キーです。</span><span class="sxs-lookup"><span data-stu-id="0e461-134">Unique identifier for the endpoint; Key.</span></span> <span data-ttu-id="0e461-135">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="0e461-135">Not nullable.</span></span> <span data-ttu-id="0e461-136">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0e461-136">Read-only.</span></span>|
| <span data-ttu-id="0e461-137">ProviderID</span><span class="sxs-lookup"><span data-stu-id="0e461-137">providerId</span></span>     | <span data-ttu-id="0e461-138">String</span><span class="sxs-lookup"><span data-stu-id="0e461-138">String</span></span>  | <span data-ttu-id="0e461-139">アプリケーション id が公開するサービスの基になるのです。</span><span class="sxs-lookup"><span data-stu-id="0e461-139">Application id of the publishing underlying service.</span></span> <span data-ttu-id="0e461-140">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="0e461-140">Not nullable.</span></span> <span data-ttu-id="0e461-141">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0e461-141">Read-only.</span></span>|
| <span data-ttu-id="0e461-142">ProviderName</span><span class="sxs-lookup"><span data-stu-id="0e461-142">providerName</span></span>   | <span data-ttu-id="0e461-143">String</span><span class="sxs-lookup"><span data-stu-id="0e461-143">String</span></span>  | <span data-ttu-id="0e461-144">公開するサービスの基になるの名前です。</span><span class="sxs-lookup"><span data-stu-id="0e461-144">Name of the publishing underlying service.</span></span> <span data-ttu-id="0e461-145">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0e461-145">Read-only.</span></span>|
| <span data-ttu-id="0e461-146">providerResourceId</span><span class="sxs-lookup"><span data-stu-id="0e461-146">providerResourceId</span></span>|<span data-ttu-id="0e461-147">String</span><span class="sxs-lookup"><span data-stu-id="0e461-147">String</span></span>| <span data-ttu-id="0e461-148">Office 365 グループでは、この処理は、リソース (たとえば Yammer.FeedURL など) の既知の名前に設定されます。</span><span class="sxs-lookup"><span data-stu-id="0e461-148">For Office 365 groups, this is set to a well-known name for the resource (e.g. Yammer.FeedURL etc.).</span></span> <span data-ttu-id="0e461-149">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="0e461-149">Not nullable.</span></span> <span data-ttu-id="0e461-150">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0e461-150">Read-only.</span></span>|
| <span data-ttu-id="0e461-151">uri</span><span class="sxs-lookup"><span data-stu-id="0e461-151">uri</span></span>            | <span data-ttu-id="0e461-152">String</span><span class="sxs-lookup"><span data-stu-id="0e461-152">String</span></span>  | <span data-ttu-id="0e461-153">公開されたリソースの URL です。</span><span class="sxs-lookup"><span data-stu-id="0e461-153">URL of the published resource.</span></span> <span data-ttu-id="0e461-154">null 許容ではありません。</span><span class="sxs-lookup"><span data-stu-id="0e461-154">Not nullable.</span></span> <span data-ttu-id="0e461-155">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0e461-155">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e461-156">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0e461-156">Relationships</span></span>

<span data-ttu-id="0e461-157">なし。</span><span class="sxs-lookup"><span data-stu-id="0e461-157">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="0e461-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0e461-158">JSON representation</span></span>
<span data-ttu-id="0e461-159">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0e461-159">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Endpoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/endpoint.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
