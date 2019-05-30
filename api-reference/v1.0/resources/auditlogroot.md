---
title: auditLogRoot リソースの種類
description: さまざまな種類の監査ログが含まれています。 このリソースは、単一の監査ログリソースを返します。 使用可能なプロパティは含まれていません。
author: dhanyahk
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a0f961850e0ef48776cf708348fcbacf4c9642c3
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536037"
---
# <a name="auditlogroot-resource-type"></a><span data-ttu-id="09376-105">auditLogRoot リソースの種類</span><span class="sxs-lookup"><span data-stu-id="09376-105">auditLogRoot resource type</span></span>

<span data-ttu-id="09376-106">さまざまな種類の監査ログが含まれています。</span><span class="sxs-lookup"><span data-stu-id="09376-106">Contains different types of audit logs.</span></span> <span data-ttu-id="09376-107">このリソースは、単一の監査ログリソースを返します。</span><span class="sxs-lookup"><span data-stu-id="09376-107">This resources returns a singleton auditLog resource.</span></span> <span data-ttu-id="09376-108">使用可能なプロパティは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="09376-108">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="09376-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="09376-109">Methods</span></span>

| <span data-ttu-id="09376-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="09376-110">Method</span></span>           | <span data-ttu-id="09376-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="09376-111">Return Type</span></span>    |<span data-ttu-id="09376-112">説明</span><span class="sxs-lookup"><span data-stu-id="09376-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="09376-113">directoryAudits を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="09376-113">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="09376-114">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="09376-114">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="09376-115">コレクションの中のディレクトリの監査アイテムとそのプロパティを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="09376-115">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="09376-116">directoryAudit を取得する</span><span class="sxs-lookup"><span data-stu-id="09376-116">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="09376-117">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="09376-117">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="09376-118">特定のディレクトリの監査アイテムとそのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="09376-118">Get a specific directory audit item and its properties.</span></span>|
|[<span data-ttu-id="09376-119">サインインを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="09376-119">List signIn</span></span>](../api/signin-list.md) | [<span data-ttu-id="09376-120">サインイン</span><span class="sxs-lookup"><span data-stu-id="09376-120">signIn</span></span>](signin.md) |<span data-ttu-id="09376-121">サインイン オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="09376-121">Read properties and relationships of signIn objects.</span></span>|
|[<span data-ttu-id="09376-122">サインインを取得する</span><span class="sxs-lookup"><span data-stu-id="09376-122">Get signIn</span></span>](../api/signin-get.md) | [<span data-ttu-id="09376-123">サインイン</span><span class="sxs-lookup"><span data-stu-id="09376-123">signIn</span></span>](signin.md) |<span data-ttu-id="09376-124">サインイン オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="09376-124">Read properties and relationships of signIn object.</span></span>|

## <a name="properties"></a><span data-ttu-id="09376-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09376-125">Properties</span></span>

<span data-ttu-id="09376-126">なし</span><span class="sxs-lookup"><span data-stu-id="09376-126">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="09376-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="09376-127">Relationships</span></span>

| <span data-ttu-id="09376-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="09376-128">Relationship</span></span> | <span data-ttu-id="09376-129">型</span><span class="sxs-lookup"><span data-stu-id="09376-129">Type</span></span>   |<span data-ttu-id="09376-130">説明</span><span class="sxs-lookup"><span data-stu-id="09376-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="09376-131">directoryAudits</span><span class="sxs-lookup"><span data-stu-id="09376-131">directoryAudits</span></span>|<span data-ttu-id="09376-132">[Directoryaudit](directoryaudit.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="09376-132">[directoryAudit](directoryaudit.md) collection</span></span>| <span data-ttu-id="09376-133">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="09376-133">Read-only.</span></span> <span data-ttu-id="09376-134">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="09376-134">Nullable.</span></span>|
|<span data-ttu-id="09376-135">signIns</span><span class="sxs-lookup"><span data-stu-id="09376-135">signIns</span></span>|<span data-ttu-id="09376-136">[サインイン](signin.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="09376-136">[signIn](signin.md) collection</span></span>| <span data-ttu-id="09376-p104">読み取り専用。Null 許容型です。</span><span class="sxs-lookup"><span data-stu-id="09376-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="09376-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="09376-139">JSON representation</span></span>

<span data-ttu-id="09376-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="09376-140">Here is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="09376-141">例</span><span class="sxs-lookup"><span data-stu-id="09376-141">Example</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="09376-142">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="09376-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="09376-143">C#</span><span class="sxs-lookup"><span data-stu-id="09376-143">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_auditLogs-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="09376-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="09376-144">Javascript</span></span>](#tab/javascript)
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
