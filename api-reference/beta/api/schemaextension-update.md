---
title: schemaExtension を更新する
description: 指定した schemaExtension の定義のプロパティを更新します。
localization_priority: Normal
author: dkershaw10
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: caddc1274c38149b323b4f72567ca8f6c47e3f86
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410561"
---
# <a name="update-schemaextension"></a><span data-ttu-id="f6d79-103">schemaExtension を更新する</span><span class="sxs-lookup"><span data-stu-id="f6d79-103">Update schemaExtension</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6d79-104">指定した[Schemaextension](../resources/schemaextension.md)の定義のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f6d79-104">Update properties in the definition of the specified [schemaExtension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="f6d79-105">この更新は、拡張機能の**Targettypes**プロパティに含まれるすべてのリソースに適用されます。</span><span class="sxs-lookup"><span data-stu-id="f6d79-105">The update applies to all the resources that are included in the **targetTypes** property of the extension.</span></span> <span data-ttu-id="f6d79-106">これらのリソースは、[サポート](/graph/extensibility-overview#supported-resources)されているリソースの種類の中にあります。</span><span class="sxs-lookup"><span data-stu-id="f6d79-106">These resources are among the [supporting resource types](/graph/extensibility-overview#supported-resources).</span></span>

<span data-ttu-id="f6d79-107">拡張機能が**Indevelopment**または**Available** status にある場合は、スキーマ拡張機能 (所有者アプリ) を作成したアプリのみが拡張機能を追加で更新できます。</span><span class="sxs-lookup"><span data-stu-id="f6d79-107">Only the app that created a schema extension (owner app) can make additive updates to the extension when the extension is in the **InDevelopment** or **Available** status.</span></span> <span data-ttu-id="f6d79-108">つまり、アプリでカスタムプロパティを削除したり、ターゲットリソースの種類を定義から削除したりすることはできません。</span><span class="sxs-lookup"><span data-stu-id="f6d79-108">That means the app cannot remove custom properties or target resource types from the definition.</span></span> <span data-ttu-id="f6d79-109">ただし、アプリで拡張機能の説明を変更することはできます。</span><span class="sxs-lookup"><span data-stu-id="f6d79-109">The app can, however, change the description of the extension.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6d79-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f6d79-110">Permissions</span></span>

<span data-ttu-id="f6d79-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f6d79-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f6d79-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f6d79-113">Permission type</span></span>      | <span data-ttu-id="f6d79-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f6d79-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6d79-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f6d79-115">Delegated (work or school account)</span></span> | <span data-ttu-id="f6d79-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f6d79-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f6d79-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f6d79-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6d79-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f6d79-118">Not supported.</span></span>    |
|<span data-ttu-id="f6d79-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f6d79-119">Application</span></span> | <span data-ttu-id="f6d79-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f6d79-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6d79-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f6d79-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /schemaExtensions/{id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="f6d79-122">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f6d79-122">Optional request headers</span></span>

| <span data-ttu-id="f6d79-123">名前</span><span class="sxs-lookup"><span data-stu-id="f6d79-123">Name</span></span>      |<span data-ttu-id="f6d79-124">説明</span><span class="sxs-lookup"><span data-stu-id="f6d79-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f6d79-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6d79-125">Authorization</span></span>  | <span data-ttu-id="f6d79-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f6d79-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f6d79-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f6d79-128">Content-Type</span></span>   | <span data-ttu-id="f6d79-129">application/json</span><span class="sxs-lookup"><span data-stu-id="f6d79-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f6d79-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="f6d79-130">Request body</span></span>

<span data-ttu-id="f6d79-p105">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="f6d79-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="f6d79-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f6d79-134">Property</span></span>   | <span data-ttu-id="f6d79-135">型</span><span class="sxs-lookup"><span data-stu-id="f6d79-135">Type</span></span> |<span data-ttu-id="f6d79-136">説明</span><span class="sxs-lookup"><span data-stu-id="f6d79-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f6d79-137">description</span><span class="sxs-lookup"><span data-stu-id="f6d79-137">description</span></span>|<span data-ttu-id="f6d79-138">String</span><span class="sxs-lookup"><span data-stu-id="f6d79-138">String</span></span>|<span data-ttu-id="f6d79-139">スキーマ拡張機能の説明。</span><span class="sxs-lookup"><span data-stu-id="f6d79-139">Description for the schema extension.</span></span>|
|<span data-ttu-id="f6d79-140">properties</span><span class="sxs-lookup"><span data-stu-id="f6d79-140">properties</span></span>|<span data-ttu-id="f6d79-141">[extensionSchemaProperty](../resources/extensionschemaproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f6d79-141">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="f6d79-142">スキーマ拡張機能の定義を構成するプロパティの名前と種類のコレクション。</span><span class="sxs-lookup"><span data-stu-id="f6d79-142">The collection of property names and types that make up the schema extension definition.</span></span> <span data-ttu-id="f6d79-143">加法変更のみが許可されます。</span><span class="sxs-lookup"><span data-stu-id="f6d79-143">Only additive changes are permitted.</span></span> |
|<span data-ttu-id="f6d79-144">status</span><span class="sxs-lookup"><span data-stu-id="f6d79-144">status</span></span>|<span data-ttu-id="f6d79-145">String</span><span class="sxs-lookup"><span data-stu-id="f6d79-145">String</span></span>|<span data-ttu-id="f6d79-146">スキーマ拡張機能のライフサイクル状態。</span><span class="sxs-lookup"><span data-stu-id="f6d79-146">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="f6d79-147">作成時の初期状態は**開発**中です。</span><span class="sxs-lookup"><span data-stu-id="f6d79-147">The initial state upon creation is **InDevelopment**.</span></span> <span data-ttu-id="f6d79-148">可能な状態遷移は**開発**から**利用可能**であり、**廃止**から利用**可能**です。</span><span class="sxs-lookup"><span data-stu-id="f6d79-148">Possible states transitions are from **InDevelopment** to **Available** and **Available** to **Deprecated**.</span></span>|
|<span data-ttu-id="f6d79-149">targetTypes</span><span class="sxs-lookup"><span data-stu-id="f6d79-149">targetTypes</span></span>|<span data-ttu-id="f6d79-150">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f6d79-150">String collection</span></span>|<span data-ttu-id="f6d79-151">スキーマ拡張機能に適用できる (拡張機能をサポートできる) 一連の Microsoft Graph の種類。</span><span class="sxs-lookup"><span data-stu-id="f6d79-151">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.</span></span>  <span data-ttu-id="f6d79-152">加法変更のみが許可されます。</span><span class="sxs-lookup"><span data-stu-id="f6d79-152">Only additive changes are permitted.</span></span>|

## <a name="response"></a><span data-ttu-id="f6d79-153">応答</span><span class="sxs-lookup"><span data-stu-id="f6d79-153">Response</span></span>

<span data-ttu-id="f6d79-154">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="f6d79-154">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f6d79-155">例</span><span class="sxs-lookup"><span data-stu-id="f6d79-155">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f6d79-156">要求</span><span class="sxs-lookup"><span data-stu-id="f6d79-156">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f6d79-157">プロトコル</span><span class="sxs-lookup"><span data-stu-id="f6d79-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_schemaextension"
}-->
```http
PATCH https://graph.microsoft.com/beta/schemaExtensions/{id}
Content-type: application/json
Content-length: 201

{
  "properties": [
    {
      "name":"new-name-value",
      "type":"new-type-value"
    },
    {
      "name":"additional-name-value",
      "type":"additional-type-value"
    }
  ],
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f6d79-158">C#</span><span class="sxs-lookup"><span data-stu-id="f6d79-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-schemaextension-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f6d79-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6d79-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-schemaextension-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f6d79-160">目的-C</span><span class="sxs-lookup"><span data-stu-id="f6d79-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-schemaextension-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f6d79-161">応答</span><span class="sxs-lookup"><span data-stu-id="f6d79-161">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="f6d79-162">関連項目</span><span class="sxs-lookup"><span data-stu-id="f6d79-162">See also</span></span>

- [<span data-ttu-id="f6d79-163">拡張機能を使用したリソースへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="f6d79-163">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="f6d79-164">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="f6d79-164">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update schemaextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
