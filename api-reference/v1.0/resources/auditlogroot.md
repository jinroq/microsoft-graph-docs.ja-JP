---
title: auditLogRoot リソースの種類
description: さまざまな種類の監査ログが含まれています。 このリソースは、単一の監査ログリソースを返します。 使用可能なプロパティは含まれていません。
author: dhanyahk
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 204dfbb3f03be9550429694434bcb420b93e788d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33951407"
---
# <a name="auditlogroot-resource-type"></a><span data-ttu-id="aabde-105">auditLogRoot リソースの種類</span><span class="sxs-lookup"><span data-stu-id="aabde-105">auditLogRoot resource type</span></span>

<span data-ttu-id="aabde-106">さまざまな種類の監査ログが含まれています。</span><span class="sxs-lookup"><span data-stu-id="aabde-106">Contains different types of audit logs.</span></span> <span data-ttu-id="aabde-107">このリソースは、単一の監査ログリソースを返します。</span><span class="sxs-lookup"><span data-stu-id="aabde-107">This resources returns a singleton auditLog resource.</span></span> <span data-ttu-id="aabde-108">使用可能なプロパティは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="aabde-108">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="aabde-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="aabde-109">Methods</span></span>

| <span data-ttu-id="aabde-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="aabde-110">Method</span></span>           | <span data-ttu-id="aabde-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="aabde-111">Return Type</span></span>    |<span data-ttu-id="aabde-112">説明</span><span class="sxs-lookup"><span data-stu-id="aabde-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="aabde-113">directoryAudits を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="aabde-113">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="aabde-114">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="aabde-114">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="aabde-115">コレクションの中のディレクトリの監査アイテムとそのプロパティを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="aabde-115">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="aabde-116">directoryAudit を取得する</span><span class="sxs-lookup"><span data-stu-id="aabde-116">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="aabde-117">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="aabde-117">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="aabde-118">特定のディレクトリの監査アイテムとそのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="aabde-118">Get a specific directory audit item and its properties.</span></span>|
|[<span data-ttu-id="aabde-119">サインインを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="aabde-119">List signIn</span></span>](../api/signin-list.md) | [<span data-ttu-id="aabde-120">サインイン</span><span class="sxs-lookup"><span data-stu-id="aabde-120">signIn</span></span>](signin.md) |<span data-ttu-id="aabde-121">サインイン オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="aabde-121">Read properties and relationships of signIn objects.</span></span>|
|[<span data-ttu-id="aabde-122">サインインを取得する</span><span class="sxs-lookup"><span data-stu-id="aabde-122">Get signIn</span></span>](../api/signin-get.md) | [<span data-ttu-id="aabde-123">サインイン</span><span class="sxs-lookup"><span data-stu-id="aabde-123">signIn</span></span>](signin.md) |<span data-ttu-id="aabde-124">サインイン オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="aabde-124">Read properties and relationships of signIn object.</span></span>|

## <a name="properties"></a><span data-ttu-id="aabde-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aabde-125">Properties</span></span>

<span data-ttu-id="aabde-126">なし</span><span class="sxs-lookup"><span data-stu-id="aabde-126">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="aabde-127">関係</span><span class="sxs-lookup"><span data-stu-id="aabde-127">Relationships</span></span>

| <span data-ttu-id="aabde-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="aabde-128">Relationship</span></span> | <span data-ttu-id="aabde-129">型</span><span class="sxs-lookup"><span data-stu-id="aabde-129">Type</span></span>   |<span data-ttu-id="aabde-130">説明</span><span class="sxs-lookup"><span data-stu-id="aabde-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aabde-131">directoryAudits</span><span class="sxs-lookup"><span data-stu-id="aabde-131">directoryAudits</span></span>|<span data-ttu-id="aabde-132">[Directoryaudit](directoryAudit.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="aabde-132">[directoryAudit](directoryAudit.md) collection</span></span>| <span data-ttu-id="aabde-133">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="aabde-133">Read-only.</span></span> <span data-ttu-id="aabde-134">Null 許容型です。</span><span class="sxs-lookup"><span data-stu-id="aabde-134">Nullable.</span></span>|
|<span data-ttu-id="aabde-135">signIns</span><span class="sxs-lookup"><span data-stu-id="aabde-135">signIns</span></span>|<span data-ttu-id="aabde-136">[サインイン](signIn.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="aabde-136">[signIn](signIn.md) collection</span></span>| <span data-ttu-id="aabde-p104">読み取り専用。Null 許容型です。</span><span class="sxs-lookup"><span data-stu-id="aabde-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aabde-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aabde-139">JSON representation</span></span>

<span data-ttu-id="aabde-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="aabde-140">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.auditLogRoot"
}-->

```json
{
}
```

## <a name="example"></a><span data-ttu-id="aabde-141">例</span><span class="sxs-lookup"><span data-stu-id="aabde-141">Example</span></span>

<!-- {
  "blockType": "request",
  "name": "get_auditLogs"
}-->
```http
GET https://graph.microsoft.com/v1.0/auditLogs
```

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.auditLogRoot"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="aabde-142">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="aabde-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="aabde-143">C#</span><span class="sxs-lookup"><span data-stu-id="aabde-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_auditLogs-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="aabde-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="aabde-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_auditLogs-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "auditLogRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/resources/auditlogroot.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/resources/auditlogroot.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
