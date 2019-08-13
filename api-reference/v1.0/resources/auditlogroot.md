---
title: auditLogRoot リソースの種類
description: さまざまな種類の監査ログが含まれています。 このリソースは、単一の監査ログリソースを返します。 使用可能なプロパティは含まれていません。
author: dhanyahk
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c0baab1704958a46235c22c8f49f93f1f488f072
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370360"
---
# <a name="auditlogroot-resource-type"></a><span data-ttu-id="12926-105">auditLogRoot リソースの種類</span><span class="sxs-lookup"><span data-stu-id="12926-105">auditLogRoot resource type</span></span>

<span data-ttu-id="12926-106">さまざまな種類の監査ログが含まれています。</span><span class="sxs-lookup"><span data-stu-id="12926-106">Contains different types of audit logs.</span></span> <span data-ttu-id="12926-107">このリソースは、単一の監査ログリソースを返します。</span><span class="sxs-lookup"><span data-stu-id="12926-107">This resources returns a singleton auditLog resource.</span></span> <span data-ttu-id="12926-108">使用可能なプロパティは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="12926-108">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="12926-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="12926-109">Methods</span></span>

| <span data-ttu-id="12926-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="12926-110">Method</span></span>           | <span data-ttu-id="12926-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="12926-111">Return Type</span></span>    |<span data-ttu-id="12926-112">説明</span><span class="sxs-lookup"><span data-stu-id="12926-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="12926-113">directoryAudits を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="12926-113">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="12926-114">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="12926-114">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="12926-115">コレクションの中のディレクトリの監査アイテムとそのプロパティを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="12926-115">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="12926-116">directoryAudit を取得する</span><span class="sxs-lookup"><span data-stu-id="12926-116">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="12926-117">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="12926-117">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="12926-118">特定のディレクトリの監査アイテムとそのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="12926-118">Get a specific directory audit item and its properties.</span></span>|
|[<span data-ttu-id="12926-119">サインインを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="12926-119">List signIn</span></span>](../api/signin-list.md) | [<span data-ttu-id="12926-120">サインイン</span><span class="sxs-lookup"><span data-stu-id="12926-120">signIn</span></span>](signin.md) |<span data-ttu-id="12926-121">サインイン オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="12926-121">Read properties and relationships of signIn objects.</span></span>|
|[<span data-ttu-id="12926-122">サインインを取得する</span><span class="sxs-lookup"><span data-stu-id="12926-122">Get signIn</span></span>](../api/signin-get.md) | [<span data-ttu-id="12926-123">サインイン</span><span class="sxs-lookup"><span data-stu-id="12926-123">signIn</span></span>](signin.md) |<span data-ttu-id="12926-124">サインイン オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="12926-124">Read properties and relationships of signIn object.</span></span>|

## <a name="properties"></a><span data-ttu-id="12926-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="12926-125">Properties</span></span>

<span data-ttu-id="12926-126">なし</span><span class="sxs-lookup"><span data-stu-id="12926-126">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="12926-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="12926-127">Relationships</span></span>

| <span data-ttu-id="12926-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="12926-128">Relationship</span></span> | <span data-ttu-id="12926-129">型</span><span class="sxs-lookup"><span data-stu-id="12926-129">Type</span></span>   |<span data-ttu-id="12926-130">説明</span><span class="sxs-lookup"><span data-stu-id="12926-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="12926-131">directoryAudits</span><span class="sxs-lookup"><span data-stu-id="12926-131">directoryAudits</span></span>|<span data-ttu-id="12926-132">[Directoryaudit](directoryaudit.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="12926-132">[directoryAudit](directoryaudit.md) collection</span></span>| <span data-ttu-id="12926-133">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="12926-133">Read-only.</span></span> <span data-ttu-id="12926-134">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="12926-134">Nullable.</span></span>|
|<span data-ttu-id="12926-135">signIns</span><span class="sxs-lookup"><span data-stu-id="12926-135">signIns</span></span>|<span data-ttu-id="12926-136">[サインイン](signin.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="12926-136">[signIn](signin.md) collection</span></span>| <span data-ttu-id="12926-p104">読み取り専用。Null 許容型です。</span><span class="sxs-lookup"><span data-stu-id="12926-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="12926-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="12926-139">JSON representation</span></span>

<span data-ttu-id="12926-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="12926-140">Here is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="12926-141">例</span><span class="sxs-lookup"><span data-stu-id="12926-141">Example</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="12926-142">プロトコル</span><span class="sxs-lookup"><span data-stu-id="12926-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_auditLogs"
}-->
```http
GET https://graph.microsoft.com/v1.0/auditLogs
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="12926-143">C#</span><span class="sxs-lookup"><span data-stu-id="12926-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-auditlogs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="12926-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="12926-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-auditlogs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="12926-145">目的-C</span><span class="sxs-lookup"><span data-stu-id="12926-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-auditlogs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="12926-146">Java</span><span class="sxs-lookup"><span data-stu-id="12926-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-auditlogs-java-snippets.md)]
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
