---
title: schemaExtension を更新する
description: 指定された schemaExtension の定義に含まれるプロパティを更新します。
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: 9f8bfc77ddcb3633160f76ce5d900e4ba09af1c9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960778"
---
# <a name="update-schemaextension"></a><span data-ttu-id="77130-103">schemaExtension を更新する</span><span class="sxs-lookup"><span data-stu-id="77130-103">Update schemaExtension</span></span>

<span data-ttu-id="77130-104">指定された [schemaExtension](../resources/schemaextension.md) の定義に含まれるプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="77130-104">Update properties in the definition of the specified [schemaExtension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="77130-p101">この更新は、拡張機能の **targetTypes** プロパティに含まれるすべてのリソースに適用されます。これらのリソースは、[サポートしているリソースの種類](/graph/extensibility-overview#supported-resources)にあります。</span><span class="sxs-lookup"><span data-stu-id="77130-p101">The update applies to all the resources that are included in the **targetTypes** property of the extension. These resources are among the [supporting resource types](/graph/extensibility-overview#supported-resources).</span></span>

<span data-ttu-id="77130-p102">スキーマ拡張機能を作成したアプリ (所有者アプリ) に限り、その拡張機能が **InDevelopment** か **Available** の状態である場合、拡張機能に対して付加的な更新を行うことができます。したがって、そのアプリは、定義からカスタム プロパティやターゲット リソースの種類を削除できません。ただし、このアプリで拡張機能の説明を変更することはできます。</span><span class="sxs-lookup"><span data-stu-id="77130-p102">Only the app that created a schema extension (owner app) can make additive updates to the extension when the extension is in the **InDevelopment** or **Available** status. That means the app cannot remove custom properties or target resource types from the definition. The app can, however, change the description of the extension.</span></span>

## <a name="permissions"></a><span data-ttu-id="77130-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="77130-110">Permissions</span></span>
<span data-ttu-id="77130-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="77130-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="77130-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="77130-113">Permission type</span></span>      | <span data-ttu-id="77130-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="77130-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77130-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="77130-115">Delegated (work or school account)</span></span> | <span data-ttu-id="77130-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="77130-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="77130-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="77130-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77130-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77130-118">Not supported.</span></span>    |
|<span data-ttu-id="77130-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="77130-119">Application</span></span> | <span data-ttu-id="77130-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77130-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="77130-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="77130-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /schemaExtensions/{id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="77130-122">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="77130-122">Optional request headers</span></span>

| <span data-ttu-id="77130-123">名前</span><span class="sxs-lookup"><span data-stu-id="77130-123">Name</span></span>      |<span data-ttu-id="77130-124">説明</span><span class="sxs-lookup"><span data-stu-id="77130-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="77130-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="77130-125">Authorization</span></span>  | <span data-ttu-id="77130-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="77130-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="77130-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="77130-128">Content-Type</span></span>   | <span data-ttu-id="77130-129">application/json</span><span class="sxs-lookup"><span data-stu-id="77130-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="77130-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="77130-130">Request body</span></span>

<span data-ttu-id="77130-p105">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="77130-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="77130-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="77130-134">Property</span></span>   | <span data-ttu-id="77130-135">種類</span><span class="sxs-lookup"><span data-stu-id="77130-135">Type</span></span> |<span data-ttu-id="77130-136">説明</span><span class="sxs-lookup"><span data-stu-id="77130-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77130-137">説明</span><span class="sxs-lookup"><span data-stu-id="77130-137">description</span></span>|<span data-ttu-id="77130-138">String</span><span class="sxs-lookup"><span data-stu-id="77130-138">String</span></span>|<span data-ttu-id="77130-139">スキーマ拡張機能の説明。</span><span class="sxs-lookup"><span data-stu-id="77130-139">Description for the schema extension.</span></span>|
|<span data-ttu-id="77130-140">properties</span><span class="sxs-lookup"><span data-stu-id="77130-140">properties</span></span>|<span data-ttu-id="77130-141">[extensionSchemaProperty](../resources/extensionschemaproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="77130-141">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="77130-p106">スキーマ拡張機能の定義を構成するプロパティの名前と種類のコレクション。付加的な変更のみが許可されます。</span><span class="sxs-lookup"><span data-stu-id="77130-p106">The collection of property names and types that make up the schema extension definition. Only additive changes are permitted.</span></span> |
|<span data-ttu-id="77130-144">status</span><span class="sxs-lookup"><span data-stu-id="77130-144">status</span></span>|<span data-ttu-id="77130-145">String</span><span class="sxs-lookup"><span data-stu-id="77130-145">String</span></span>|<span data-ttu-id="77130-146">スキーマ拡張機能のライフサイクル状態。</span><span class="sxs-lookup"><span data-stu-id="77130-146">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="77130-147">作成時に初期状態は、 **InDevelopment**です。</span><span class="sxs-lookup"><span data-stu-id="77130-147">The initial state upon creation is **InDevelopment**.</span></span> <span data-ttu-id="77130-148">状態遷移は、 **InDevelopment**を**使用可能**および**使用可能な\*\*\*\*非推奨**です。</span><span class="sxs-lookup"><span data-stu-id="77130-148">Possible states transitions are from **InDevelopment** to **Available** and **Available** to **Deprecated**.</span></span>|
|<span data-ttu-id="77130-149">targetTypes</span><span class="sxs-lookup"><span data-stu-id="77130-149">targetTypes</span></span>|<span data-ttu-id="77130-150">String コレクション</span><span class="sxs-lookup"><span data-stu-id="77130-150">String collection</span></span>|<span data-ttu-id="77130-p108">スキーマ拡張機能に適用できる (拡張機能をサポートできる) 一連の Microsoft Graph の種類。付加的な変更のみが許可されます。</span><span class="sxs-lookup"><span data-stu-id="77130-p108">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.  Only additive changes are permitted.</span></span>|

## <a name="response"></a><span data-ttu-id="77130-153">応答</span><span class="sxs-lookup"><span data-stu-id="77130-153">Response</span></span>

<span data-ttu-id="77130-154">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="77130-154">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="77130-155">例</span><span class="sxs-lookup"><span data-stu-id="77130-155">Example</span></span>

##### <a name="request"></a><span data-ttu-id="77130-156">要求</span><span class="sxs-lookup"><span data-stu-id="77130-156">Request</span></span>

<span data-ttu-id="77130-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="77130-157">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_schemaextension"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/schemaExtensions/{id}
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

##### <a name="response"></a><span data-ttu-id="77130-158">応答</span><span class="sxs-lookup"><span data-stu-id="77130-158">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="77130-159">関連項目</span><span class="sxs-lookup"><span data-stu-id="77130-159">See also</span></span>

- [<span data-ttu-id="77130-160">拡張機能を使用したリソースへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="77130-160">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="77130-161">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="77130-161">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update schemaextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
