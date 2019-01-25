---
title: NamedItem オブジェクトを更新する
description: nameditem オブジェクトのプロパティを更新します。
localization_priority: Normal
ms.openlocfilehash: ffb01e0998b3b94706e50ed461014fcfd11ce927
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514048"
---
# <a name="update-nameditem"></a><span data-ttu-id="8b2ee-103">NamedItem オブジェクトを更新する</span><span class="sxs-lookup"><span data-stu-id="8b2ee-103">Update nameditem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b2ee-104">nameditem オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8b2ee-104">Update the properties of nameditem object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8b2ee-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8b2ee-105">Permissions</span></span>
<span data-ttu-id="8b2ee-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8b2ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b2ee-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8b2ee-108">Permission type</span></span>      | <span data-ttu-id="8b2ee-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8b2ee-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b2ee-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8b2ee-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8b2ee-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b2ee-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8b2ee-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8b2ee-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b2ee-113">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8b2ee-113">Files.ReadWrite</span></span>    |
|<span data-ttu-id="8b2ee-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8b2ee-114">Application</span></span> | <span data-ttu-id="8b2ee-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8b2ee-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b2ee-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8b2ee-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)
```
## <a name="optional-request-headers"></a><span data-ttu-id="8b2ee-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8b2ee-117">Optional request headers</span></span>
| <span data-ttu-id="8b2ee-118">名前</span><span class="sxs-lookup"><span data-stu-id="8b2ee-118">Name</span></span>       | <span data-ttu-id="8b2ee-119">説明</span><span class="sxs-lookup"><span data-stu-id="8b2ee-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="8b2ee-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b2ee-120">Authorization</span></span>  | <span data-ttu-id="8b2ee-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8b2ee-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8b2ee-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="8b2ee-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="8b2ee-p103">変更を保持するかどうかを決定するブック セッション ID。省略可能。</span><span class="sxs-lookup"><span data-stu-id="8b2ee-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b2ee-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8b2ee-126">Request body</span></span>
<span data-ttu-id="8b2ee-p104">要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="8b2ee-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8b2ee-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8b2ee-130">Property</span></span>     | <span data-ttu-id="8b2ee-131">型</span><span class="sxs-lookup"><span data-stu-id="8b2ee-131">Type</span></span>   |<span data-ttu-id="8b2ee-132">説明</span><span class="sxs-lookup"><span data-stu-id="8b2ee-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8b2ee-133">visible</span><span class="sxs-lookup"><span data-stu-id="8b2ee-133">visible</span></span>|<span data-ttu-id="8b2ee-134">boolean</span><span class="sxs-lookup"><span data-stu-id="8b2ee-134">boolean</span></span>|<span data-ttu-id="8b2ee-135">オブジェクトを表示するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="8b2ee-135">Specifies whether the object is visible or not.</span></span>|
|<span data-ttu-id="8b2ee-136">comment</span><span class="sxs-lookup"><span data-stu-id="8b2ee-136">comment</span></span>|   <span data-ttu-id="8b2ee-137">string</span><span class="sxs-lookup"><span data-stu-id="8b2ee-137">string</span></span>  |<span data-ttu-id="8b2ee-138">この名前に関連付けられているコメントを表します。</span><span class="sxs-lookup"><span data-stu-id="8b2ee-138">Represents the comment associated with this name.</span></span>|

## <a name="response"></a><span data-ttu-id="8b2ee-139">応答</span><span class="sxs-lookup"><span data-stu-id="8b2ee-139">Response</span></span>

<span data-ttu-id="8b2ee-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [NamedItem](../resources/nameditem.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8b2ee-140">If successful, this method returns a `200 OK` response code and updated [NamedItem](../resources/nameditem.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8b2ee-141">例</span><span class="sxs-lookup"><span data-stu-id="8b2ee-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8b2ee-142">要求</span><span class="sxs-lookup"><span data-stu-id="8b2ee-142">Request</span></span>
<span data-ttu-id="8b2ee-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8b2ee-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_nameditem"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/names(<name>)
Content-type: application/json
Content-length: 87

{
  "type": "type-value",
  "scope": "scope-value",
  "comment": "comment-value",
  "value": {
  },
  "visible": true
}
```
##### <a name="response"></a><span data-ttu-id="8b2ee-144">応答</span><span class="sxs-lookup"><span data-stu-id="8b2ee-144">Response</span></span>
<span data-ttu-id="8b2ee-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8b2ee-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedItem"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 87

{
  "name": "name-value",
  "type": "type-value",
  "value": {
  },
  "visible": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update nameditem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/nameditem-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
