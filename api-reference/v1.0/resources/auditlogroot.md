---
title: auditLogRoot リソースの種類
description: さまざまな種類の監査ログが含まれています。 このリソースは、単一の監査ログリソースを返します。 使用可能なプロパティは含まれていません。
author: dhanyahk
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 457fb3d7e67049d25ce02ea448a206b732d2175b
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629335"
---
# <a name="auditlogroot-resource-type"></a><span data-ttu-id="f0093-105">auditLogRoot リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f0093-105">auditLogRoot resource type</span></span>

<span data-ttu-id="f0093-106">さまざまな種類の監査ログが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f0093-106">Contains different types of audit logs.</span></span> <span data-ttu-id="f0093-107">このリソースは、単一の監査ログリソースを返します。</span><span class="sxs-lookup"><span data-stu-id="f0093-107">This resources returns a singleton auditLog resource.</span></span> <span data-ttu-id="f0093-108">使用可能なプロパティは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="f0093-108">It doesn't contain any usable properties.</span></span>

## <a name="methods"></a><span data-ttu-id="f0093-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="f0093-109">Methods</span></span>

| <span data-ttu-id="f0093-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="f0093-110">Method</span></span>           | <span data-ttu-id="f0093-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f0093-111">Return Type</span></span>    |<span data-ttu-id="f0093-112">説明</span><span class="sxs-lookup"><span data-stu-id="f0093-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f0093-113">directoryAudits を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="f0093-113">List directoryAudits</span></span>](../api/directoryaudit-list.md) | [<span data-ttu-id="f0093-114">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="f0093-114">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="f0093-115">コレクションの中のディレクトリの監査アイテムとそのプロパティを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="f0093-115">List the directory audit items in the collection and their properties.</span></span>|
|[<span data-ttu-id="f0093-116">directoryAudit を取得する</span><span class="sxs-lookup"><span data-stu-id="f0093-116">Get directoryAudit</span></span>](../api/directoryaudit-get.md) | [<span data-ttu-id="f0093-117">directoryAudit</span><span class="sxs-lookup"><span data-stu-id="f0093-117">directoryAudit</span></span>](directoryaudit.md) |<span data-ttu-id="f0093-118">特定のディレクトリの監査アイテムとそのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="f0093-118">Get a specific directory audit item and its properties.</span></span>|
|[<span data-ttu-id="f0093-119">サインインを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="f0093-119">List signIn</span></span>](../api/signin-list.md) | [<span data-ttu-id="f0093-120">サインイン</span><span class="sxs-lookup"><span data-stu-id="f0093-120">signIn</span></span>](signin.md) |<span data-ttu-id="f0093-121">サインイン オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f0093-121">Read properties and relationships of signIn objects.</span></span>|
|[<span data-ttu-id="f0093-122">サインインを取得する</span><span class="sxs-lookup"><span data-stu-id="f0093-122">Get signIn</span></span>](../api/signin-get.md) | [<span data-ttu-id="f0093-123">サインイン</span><span class="sxs-lookup"><span data-stu-id="f0093-123">signIn</span></span>](signin.md) |<span data-ttu-id="f0093-124">サインイン オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f0093-124">Read properties and relationships of signIn object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f0093-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f0093-125">Properties</span></span>

<span data-ttu-id="f0093-126">なし</span><span class="sxs-lookup"><span data-stu-id="f0093-126">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="f0093-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f0093-127">Relationships</span></span>

| <span data-ttu-id="f0093-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f0093-128">Relationship</span></span> | <span data-ttu-id="f0093-129">型</span><span class="sxs-lookup"><span data-stu-id="f0093-129">Type</span></span>   |<span data-ttu-id="f0093-130">説明</span><span class="sxs-lookup"><span data-stu-id="f0093-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0093-131">directoryAudits</span><span class="sxs-lookup"><span data-stu-id="f0093-131">directoryAudits</span></span>|<span data-ttu-id="f0093-132">[Directoryaudit](directoryAudit.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f0093-132">[directoryAudit](directoryAudit.md) collection</span></span>| <span data-ttu-id="f0093-133">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="f0093-133">Read-only.</span></span> <span data-ttu-id="f0093-134">Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="f0093-134">Nullable.</span></span>|
|<span data-ttu-id="f0093-135">signIns</span><span class="sxs-lookup"><span data-stu-id="f0093-135">signIns</span></span>|<span data-ttu-id="f0093-136">[サインイン](signIn.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f0093-136">[signIn](signIn.md) collection</span></span>| <span data-ttu-id="f0093-p104">読み取り専用。Null 許容型です。</span><span class="sxs-lookup"><span data-stu-id="f0093-p104">Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f0093-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f0093-139">JSON representation</span></span>

<span data-ttu-id="f0093-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f0093-140">Here is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="f0093-141">例</span><span class="sxs-lookup"><span data-stu-id="f0093-141">Example</span></span>

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "auditLogRoot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
