---
title: schemaExtension を更新する
description: 指定された schemaExtension の定義に含まれるプロパティを更新します。
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: cdd0ac41e65e72ba16f5111c8b67869321f934dc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938497"
---
# <a name="update-schemaextension"></a><span data-ttu-id="19bdd-103">schemaExtension を更新する</span><span class="sxs-lookup"><span data-stu-id="19bdd-103">Update schemaExtension</span></span>

> <span data-ttu-id="19bdd-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="19bdd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19bdd-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19bdd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="19bdd-106">指定された [schemaExtension](../resources/schemaextension.md) の定義に含まれるプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="19bdd-106">Update properties in the definition of the specified [schemaExtension](../resources/schemaextension.md).</span></span>

<span data-ttu-id="19bdd-p102">この更新は、拡張機能の **targetTypes** プロパティに含まれるすべてのリソースに適用されます。これらのリソースは、[サポートしているリソースの種類](/graph/extensibility-overview#supported-resources)にあります。</span><span class="sxs-lookup"><span data-stu-id="19bdd-p102">The update applies to all the resources that are included in the **targetTypes** property of the extension. These resources are among the [supporting resource types](/graph/extensibility-overview#supported-resources).</span></span>

<span data-ttu-id="19bdd-p103">スキーマ拡張機能を作成したアプリ (所有者アプリ) に限り、その拡張機能が **InDevelopment** か **Available** の状態である場合、拡張機能に対して付加的な更新を行うことができます。したがって、そのアプリは、定義からカスタム プロパティやターゲット リソースの種類を削除できません。ただし、このアプリで拡張機能の説明を変更することはできます。</span><span class="sxs-lookup"><span data-stu-id="19bdd-p103">Only the app that created a schema extension (owner app) can make additive updates to the extension when the extension is in the **InDevelopment** or **Available** status. That means the app cannot remove custom properties or target resource types from the definition. The app can, however, change the description of the extension.</span></span>

## <a name="permissions"></a><span data-ttu-id="19bdd-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="19bdd-112">Permissions</span></span>

<span data-ttu-id="19bdd-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="19bdd-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="19bdd-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="19bdd-115">Permission type</span></span>      | <span data-ttu-id="19bdd-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="19bdd-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19bdd-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="19bdd-117">Delegated (work or school account)</span></span> | <span data-ttu-id="19bdd-118">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="19bdd-118">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="19bdd-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="19bdd-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19bdd-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19bdd-120">Not supported.</span></span>    |
|<span data-ttu-id="19bdd-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="19bdd-121">Application</span></span> | <span data-ttu-id="19bdd-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19bdd-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="19bdd-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="19bdd-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /schemaExtensions/{id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="19bdd-124">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="19bdd-124">Optional request headers</span></span>

| <span data-ttu-id="19bdd-125">名前</span><span class="sxs-lookup"><span data-stu-id="19bdd-125">Name</span></span>      |<span data-ttu-id="19bdd-126">説明</span><span class="sxs-lookup"><span data-stu-id="19bdd-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="19bdd-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="19bdd-127">Authorization</span></span>  | <span data-ttu-id="19bdd-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="19bdd-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="19bdd-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="19bdd-130">Content-Type</span></span>   | <span data-ttu-id="19bdd-131">application/json</span><span class="sxs-lookup"><span data-stu-id="19bdd-131">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="19bdd-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="19bdd-132">Request body</span></span>

<span data-ttu-id="19bdd-p106">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="19bdd-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="19bdd-136">プロパティ</span><span class="sxs-lookup"><span data-stu-id="19bdd-136">Property</span></span>   | <span data-ttu-id="19bdd-137">型</span><span class="sxs-lookup"><span data-stu-id="19bdd-137">Type</span></span> |<span data-ttu-id="19bdd-138">説明</span><span class="sxs-lookup"><span data-stu-id="19bdd-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19bdd-139">説明</span><span class="sxs-lookup"><span data-stu-id="19bdd-139">description</span></span>|<span data-ttu-id="19bdd-140">String</span><span class="sxs-lookup"><span data-stu-id="19bdd-140">String</span></span>|<span data-ttu-id="19bdd-141">スキーマ拡張機能の説明。</span><span class="sxs-lookup"><span data-stu-id="19bdd-141">Description for the schema extension.</span></span>|
|<span data-ttu-id="19bdd-142">properties</span><span class="sxs-lookup"><span data-stu-id="19bdd-142">properties</span></span>|<span data-ttu-id="19bdd-143">[extensionSchemaProperty](../resources/extensionschemaproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="19bdd-143">[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection</span></span>|<span data-ttu-id="19bdd-p107">スキーマ拡張機能の定義を構成するプロパティの名前と種類のコレクション。付加的な変更のみが許可されます。</span><span class="sxs-lookup"><span data-stu-id="19bdd-p107">The collection of property names and types that make up the schema extension definition. Only additive changes are permitted.</span></span> |
|<span data-ttu-id="19bdd-146">status</span><span class="sxs-lookup"><span data-stu-id="19bdd-146">status</span></span>|<span data-ttu-id="19bdd-147">String</span><span class="sxs-lookup"><span data-stu-id="19bdd-147">String</span></span>|<span data-ttu-id="19bdd-148">スキーマ拡張機能のライフサイクル状態。</span><span class="sxs-lookup"><span data-stu-id="19bdd-148">The lifecycle state of the schema extension.</span></span> <span data-ttu-id="19bdd-149">作成時に初期状態は、 **InDevelopment**です。</span><span class="sxs-lookup"><span data-stu-id="19bdd-149">The initial state upon creation is **InDevelopment**.</span></span> <span data-ttu-id="19bdd-150">状態遷移は、 **InDevelopment**を**使用可能**および**使用可能な\*\*\*\*非推奨**です。</span><span class="sxs-lookup"><span data-stu-id="19bdd-150">Possible states transitions are from **InDevelopment** to **Available** and **Available** to **Deprecated**.</span></span>|
|<span data-ttu-id="19bdd-151">targetTypes</span><span class="sxs-lookup"><span data-stu-id="19bdd-151">targetTypes</span></span>|<span data-ttu-id="19bdd-152">String コレクション</span><span class="sxs-lookup"><span data-stu-id="19bdd-152">String collection</span></span>|<span data-ttu-id="19bdd-p109">スキーマ拡張機能に適用できる (拡張機能をサポートできる) 一連の Microsoft Graph の種類。付加的な変更のみが許可されます。</span><span class="sxs-lookup"><span data-stu-id="19bdd-p109">Set of Microsoft Graph types (that can support extensions) that the schema extension can be applied to.  Only additive changes are permitted.</span></span>|

## <a name="response"></a><span data-ttu-id="19bdd-155">応答</span><span class="sxs-lookup"><span data-stu-id="19bdd-155">Response</span></span>

<span data-ttu-id="19bdd-156">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="19bdd-156">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="19bdd-157">例</span><span class="sxs-lookup"><span data-stu-id="19bdd-157">Example</span></span>

##### <a name="request"></a><span data-ttu-id="19bdd-158">要求</span><span class="sxs-lookup"><span data-stu-id="19bdd-158">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="19bdd-159">応答</span><span class="sxs-lookup"><span data-stu-id="19bdd-159">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schemaExtension"
} -->

```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="19bdd-160">関連項目</span><span class="sxs-lookup"><span data-stu-id="19bdd-160">See also</span></span>

- [<span data-ttu-id="19bdd-161">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="19bdd-161">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="19bdd-162">スキーマ拡張機能を使用したグループへのカスタム データの追加</span><span class="sxs-lookup"><span data-stu-id="19bdd-162">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update schemaextension",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
