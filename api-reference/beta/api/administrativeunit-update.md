---
title: Administrativeunit の更新
description: AdministrativeUnit オブジェクトのプロパティを更新します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9df55c0292c51b509ba9d3d79eb1e41b27065cfb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439855"
---
# <a name="update-administrativeunit"></a><span data-ttu-id="7d088-103">Administrativeunit の更新</span><span class="sxs-lookup"><span data-stu-id="7d088-103">Update administrativeunit</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d088-104">[AdministrativeUnit](../resources/administrativeunit.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7d088-104">Update the properties of an [administrativeUnit](../resources/administrativeunit.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7d088-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7d088-105">Permissions</span></span>
<span data-ttu-id="7d088-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7d088-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7d088-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7d088-108">Permission type</span></span>      | <span data-ttu-id="7d088-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="7d088-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7d088-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7d088-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7d088-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7d088-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7d088-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7d088-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d088-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d088-113">Not supported.</span></span>    |
|<span data-ttu-id="7d088-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7d088-114">Application</span></span> | <span data-ttu-id="7d088-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7d088-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d088-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7d088-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /administrativeUnits/{id}
```

## <a name="request-headers"></a><span data-ttu-id="7d088-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7d088-117">Request headers</span></span>

| <span data-ttu-id="7d088-118">名前</span><span class="sxs-lookup"><span data-stu-id="7d088-118">Name</span></span>      |<span data-ttu-id="7d088-119">説明</span><span class="sxs-lookup"><span data-stu-id="7d088-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7d088-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d088-120">Authorization</span></span>  | <span data-ttu-id="7d088-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7d088-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7d088-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="7d088-123">Request body</span></span>

<span data-ttu-id="7d088-p103">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="7d088-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="7d088-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7d088-127">Property</span></span>   | <span data-ttu-id="7d088-128">型</span><span class="sxs-lookup"><span data-stu-id="7d088-128">Type</span></span> |<span data-ttu-id="7d088-129">説明</span><span class="sxs-lookup"><span data-stu-id="7d088-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7d088-130">description</span><span class="sxs-lookup"><span data-stu-id="7d088-130">description</span></span>|<span data-ttu-id="7d088-131">string</span><span class="sxs-lookup"><span data-stu-id="7d088-131">string</span></span>|<span data-ttu-id="7d088-132">管理単位の説明。</span><span class="sxs-lookup"><span data-stu-id="7d088-132">Description for the administrative unit.</span></span>|
|<span data-ttu-id="7d088-133">displayName</span><span class="sxs-lookup"><span data-stu-id="7d088-133">displayName</span></span>|<span data-ttu-id="7d088-134">string</span><span class="sxs-lookup"><span data-stu-id="7d088-134">string</span></span>|<span data-ttu-id="7d088-135">管理単位の表示名。</span><span class="sxs-lookup"><span data-stu-id="7d088-135">Display name for the administrative unit.</span></span>|
|<span data-ttu-id="7d088-136">visibility</span><span class="sxs-lookup"><span data-stu-id="7d088-136">visibility</span></span>|<span data-ttu-id="7d088-137">string</span><span class="sxs-lookup"><span data-stu-id="7d088-137">string</span></span>|<span data-ttu-id="7d088-138">管理単位の可視性。</span><span class="sxs-lookup"><span data-stu-id="7d088-138">Visibility for the administrative unit.</span></span> <span data-ttu-id="7d088-139">設定されていない場合、既定値は "public" です。</span><span class="sxs-lookup"><span data-stu-id="7d088-139">If not set then the default is "public".</span></span> <span data-ttu-id="7d088-140">"HiddenMembership" に設定できます。これにより、メンバー以外のメンバーシップが非表示になります。</span><span class="sxs-lookup"><span data-stu-id="7d088-140">Can be set to "HiddenMembership", which hides the membership from non-members.</span></span>|

<span data-ttu-id="7d088-141">**AdministrativeUnit**リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため`PATCH` 、操作を使用して、既存の**administrativeUnit**インスタンスの拡張機能のカスタムプロパティで、独自のアプリ固有のデータを追加、更新、または削除することができます。</span><span class="sxs-lookup"><span data-stu-id="7d088-141">Since the **administrativeUnit** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **administrativeUnit** instance.</span></span>

## <a name="response"></a><span data-ttu-id="7d088-142">応答</span><span class="sxs-lookup"><span data-stu-id="7d088-142">Response</span></span>

<span data-ttu-id="7d088-143">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="7d088-143">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7d088-144">例</span><span class="sxs-lookup"><span data-stu-id="7d088-144">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7d088-145">要求</span><span class="sxs-lookup"><span data-stu-id="7d088-145">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="7d088-146">プロトコル</span><span class="sxs-lookup"><span data-stu-id="7d088-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_administrativeunit"
}-->
```http
PATCH https://graph.microsoft.com/beta/administrativeUnits/{id}
Content-type: application/json
Content-length: 114

{
  "displayName": "displayName-value",
  "description": "description-value",
  "visibility": "visibility-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7d088-147">C#</span><span class="sxs-lookup"><span data-stu-id="7d088-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7d088-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="7d088-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7d088-149">目的-C</span><span class="sxs-lookup"><span data-stu-id="7d088-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7d088-150">応答</span><span class="sxs-lookup"><span data-stu-id="7d088-150">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeunit"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="7d088-151">関連項目</span><span class="sxs-lookup"><span data-stu-id="7d088-151">See also</span></span>

- [<span data-ttu-id="7d088-152">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="7d088-152">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="7d088-153">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="7d088-153">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update administrativeunit",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
