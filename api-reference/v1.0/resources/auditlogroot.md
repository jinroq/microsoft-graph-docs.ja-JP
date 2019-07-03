---
title: auditLogRoot リソースの種類
description: さまざまな種類の監査ログが含まれています。 このリソースは、単一の監査ログリソースを返します。 使用可能なプロパティは含まれていません。
author: dhanyahk
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c43367465ac89116fcdca2460deb832d2cfbe746
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35444023"
---
# <a name="auditlogroot-resource-type"></a><span data-ttu-id="e1861-105">auditLogRoot リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e1861-105">auditLogRoot resource type</span></span>

<span data-ttu-id="e1861-106">さまざまな種類の監査ログが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e1861-106">Contains different types of audit logs.</span></span> <span data-ttu-id="e1861-107">このリソースは、単一の監査ログリソースを返します。</span><span class="sxs-lookup"><span data-stu-id="e1861-107">This resources returns a singleton auditLog resource.</span></span> <span data-ttu-id="e1861-108">使用可能なプロパティは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="e1861-108">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="e1861-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="e1861-109">Methods</span></span>

| <span data-ttu-id="e1861-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="e1861-110">Method</span></span>           | <span data-ttu-id="e1861-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e1861-111">Return Type</span></span>    |<span data-ttu-id="e1861-112">説明</span><span class="sxs-lookup"><span data-stu-id="e1861-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e1861-113">directoryAudits を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e1861-113">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="e1861-114">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="e1861-114">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="e1861-115">コレクションの中のディレクトリの監査アイテムとそのプロパティを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="e1861-115">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="e1861-116">directoryAudit を取得する</span><span class="sxs-lookup"><span data-stu-id="e1861-116">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="e1861-117">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="e1861-117">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="e1861-118">特定のディレクトリの監査アイテムとそのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="e1861-118">Get a specific directory audit item and its properties.</span></span>|
|[<span data-ttu-id="e1861-119">サインインを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e1861-119">List signIn</span></span>](../api/signin-list.md) | [<span data-ttu-id="e1861-120">サインイン</span><span class="sxs-lookup"><span data-stu-id="e1861-120">signIn</span></span>](signin.md) |<span data-ttu-id="e1861-121">サインイン オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e1861-121">Read properties and relationships of signIn objects.</span></span>|
|[<span data-ttu-id="e1861-122">サインインを取得する</span><span class="sxs-lookup"><span data-stu-id="e1861-122">Get signIn</span></span>](../api/signin-get.md) | [<span data-ttu-id="e1861-123">サインイン</span><span class="sxs-lookup"><span data-stu-id="e1861-123">signIn</span></span>](signin.md) |<span data-ttu-id="e1861-124">サインイン オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e1861-124">Read properties and relationships of signIn object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e1861-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e1861-125">Properties</span></span>

<span data-ttu-id="e1861-126">なし</span><span class="sxs-lookup"><span data-stu-id="e1861-126">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="e1861-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e1861-127">Relationships</span></span>

| <span data-ttu-id="e1861-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e1861-128">Relationship</span></span> | <span data-ttu-id="e1861-129">型</span><span class="sxs-lookup"><span data-stu-id="e1861-129">Type</span></span>   |<span data-ttu-id="e1861-130">説明</span><span class="sxs-lookup"><span data-stu-id="e1861-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1861-131">directoryAudits</span><span class="sxs-lookup"><span data-stu-id="e1861-131">directoryAudits</span></span>|<span data-ttu-id="e1861-132">[Directoryaudit](directoryaudit.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e1861-132">[directoryAudit](directoryaudit.md) collection</span></span>| <span data-ttu-id="e1861-133">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="e1861-133">Read-only.</span></span> <span data-ttu-id="e1861-134">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="e1861-134">Nullable.</span></span>|
|<span data-ttu-id="e1861-135">signIns</span><span class="sxs-lookup"><span data-stu-id="e1861-135">signIns</span></span>|<span data-ttu-id="e1861-136">[サインイン](signin.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e1861-136">[signIn](signin.md) collection</span></span>| <span data-ttu-id="e1861-p104">読み取り専用。Null 許容型です。</span><span class="sxs-lookup"><span data-stu-id="e1861-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e1861-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e1861-139">JSON representation</span></span>

<span data-ttu-id="e1861-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e1861-140">Here is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="e1861-141">例</span><span class="sxs-lookup"><span data-stu-id="e1861-141">Example</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="e1861-142">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e1861-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_auditLogs"
}-->
```http
GET https://graph.microsoft.com/v1.0/auditLogs
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e1861-143">C#</span><span class="sxs-lookup"><span data-stu-id="e1861-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-auditlogs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e1861-144">Javascript</span><span class="sxs-lookup"><span data-stu-id="e1861-144">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-auditlogs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e1861-145">目的-C</span><span class="sxs-lookup"><span data-stu-id="e1861-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-auditlogs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "auditLogRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
