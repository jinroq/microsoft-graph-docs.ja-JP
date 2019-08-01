---
title: 削除済みアイテムを取得する
description: '[削除済みアイテム] から、最近削除されたアイテムのプロパティを取得します。'
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a9c30dbdd2666b4eccfee4b09a7e53ea5a23330b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36015650"
---
# <a name="get-deleted-item"></a><span data-ttu-id="fd45e-103">削除済みアイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="fd45e-103">Get deleted item</span></span>

<span data-ttu-id="fd45e-104">[[削除済みアイテム]](../resources/directory.md) から、最近削除されたアイテムのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="fd45e-104">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="fd45e-105">現在、[削除済みアイテム] 機能は [group](../resources/group.md) および [user](../resources/user.md) リソースに対してのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="fd45e-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd45e-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fd45e-106">Permissions</span></span>
<span data-ttu-id="fd45e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fd45e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="fd45e-109">ユーザーの場合:</span><span class="sxs-lookup"><span data-stu-id="fd45e-109">For users:</span></span>

|<span data-ttu-id="fd45e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fd45e-110">Permission type</span></span>      | <span data-ttu-id="fd45e-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fd45e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd45e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fd45e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fd45e-113">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fd45e-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span></span> |
|<span data-ttu-id="fd45e-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fd45e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd45e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fd45e-115">Not supported.</span></span> |
|<span data-ttu-id="fd45e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fd45e-116">Application</span></span> | <span data-ttu-id="fd45e-117">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd45e-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="fd45e-118">グループの場合:</span><span class="sxs-lookup"><span data-stu-id="fd45e-118">For groups:</span></span>

|<span data-ttu-id="fd45e-119">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fd45e-119">Permission type</span></span>      | <span data-ttu-id="fd45e-120">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fd45e-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd45e-121">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fd45e-121">Delegated (work or school account)</span></span> | <span data-ttu-id="fd45e-122">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fd45e-122">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="fd45e-123">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fd45e-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd45e-124">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fd45e-124">Not supported.</span></span>    |
|<span data-ttu-id="fd45e-125">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fd45e-125">Application</span></span> | <span data-ttu-id="fd45e-126">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fd45e-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd45e-127">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fd45e-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deletedItems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fd45e-128">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="fd45e-128">Optional query parameters</span></span>
<span data-ttu-id="fd45e-129">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="fd45e-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fd45e-130">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fd45e-130">Request headers</span></span>
| <span data-ttu-id="fd45e-131">名前</span><span class="sxs-lookup"><span data-stu-id="fd45e-131">Name</span></span>      |<span data-ttu-id="fd45e-132">説明</span><span class="sxs-lookup"><span data-stu-id="fd45e-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fd45e-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd45e-133">Authorization</span></span>  | <span data-ttu-id="fd45e-134">ベアラー &lt;コード&gt; が*必要*</span><span class="sxs-lookup"><span data-stu-id="fd45e-134">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="fd45e-135">承諾</span><span class="sxs-lookup"><span data-stu-id="fd45e-135">Accept</span></span>  | <span data-ttu-id="fd45e-136">application/json</span><span class="sxs-lookup"><span data-stu-id="fd45e-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="fd45e-137">要求本文</span><span class="sxs-lookup"><span data-stu-id="fd45e-137">Request body</span></span>
<span data-ttu-id="fd45e-138">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fd45e-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd45e-139">応答</span><span class="sxs-lookup"><span data-stu-id="fd45e-139">Response</span></span>

<span data-ttu-id="fd45e-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fd45e-140">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fd45e-141">例</span><span class="sxs-lookup"><span data-stu-id="fd45e-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fd45e-142">要求</span><span class="sxs-lookup"><span data-stu-id="fd45e-142">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fd45e-143">プロトコル</span><span class="sxs-lookup"><span data-stu-id="fd45e-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```http
GET https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fd45e-144">C#</span><span class="sxs-lookup"><span data-stu-id="fd45e-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fd45e-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="fd45e-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fd45e-146">目的-C</span><span class="sxs-lookup"><span data-stu-id="fd45e-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fd45e-147">Java</span><span class="sxs-lookup"><span data-stu-id="fd45e-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fd45e-148">応答</span><span class="sxs-lookup"><span data-stu-id="fd45e-148">Response</span></span>
<span data-ttu-id="fd45e-p102">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fd45e-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
  "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
  "displayName":"SampleGroup",
  "groupTypes":["Unified"],
  "mail":"example@contoso.com",
  "mailEnabled":true,
  "mailNickname":"Example",
  "securityEnabled":false,
  "visibility":"Public"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
