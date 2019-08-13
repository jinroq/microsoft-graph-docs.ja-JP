---
title: 削除済みアイテムを取得する
description: '[削除済みアイテム] から、最近削除されたアイテムのプロパティを取得します。'
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bd511a85349012dbd8ea7c5230a7e74cd22be7b9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373855"
---
# <a name="get-deleted-item"></a><span data-ttu-id="43e76-103">削除済みアイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="43e76-103">Get deleted item</span></span>

<span data-ttu-id="43e76-104">[[削除済みアイテム]](../resources/directory.md) から、最近削除されたアイテムのプロパティを取得します。</span><span class="sxs-lookup"><span data-stu-id="43e76-104">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="43e76-105">現在、[削除済みアイテム] 機能は [group](../resources/group.md) および [user](../resources/user.md) リソースに対してのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="43e76-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="43e76-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="43e76-106">Permissions</span></span>
<span data-ttu-id="43e76-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="43e76-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="for-users"></a><span data-ttu-id="43e76-109">ユーザーの場合:</span><span class="sxs-lookup"><span data-stu-id="43e76-109">For users:</span></span>

|<span data-ttu-id="43e76-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="43e76-110">Permission type</span></span>      | <span data-ttu-id="43e76-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="43e76-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="43e76-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="43e76-112">Delegated (work or school account)</span></span> | <span data-ttu-id="43e76-113">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="43e76-113">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory AccessAsUser.All</span></span> |
|<span data-ttu-id="43e76-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="43e76-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43e76-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="43e76-115">Not supported.</span></span> |
|<span data-ttu-id="43e76-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="43e76-116">Application</span></span> | <span data-ttu-id="43e76-117">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43e76-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

### <a name="for-groups"></a><span data-ttu-id="43e76-118">グループの場合:</span><span class="sxs-lookup"><span data-stu-id="43e76-118">For groups:</span></span>

|<span data-ttu-id="43e76-119">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="43e76-119">Permission type</span></span>      | <span data-ttu-id="43e76-120">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="43e76-120">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="43e76-121">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="43e76-121">Delegated (work or school account)</span></span> | <span data-ttu-id="43e76-122">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="43e76-122">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="43e76-123">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="43e76-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43e76-124">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="43e76-124">Not supported.</span></span>    |
|<span data-ttu-id="43e76-125">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="43e76-125">Application</span></span> | <span data-ttu-id="43e76-126">Group.Read.All、Group.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43e76-126">Group.Read.All, Group.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="43e76-127">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="43e76-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deletedItems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="43e76-128">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="43e76-128">Optional query parameters</span></span>
<span data-ttu-id="43e76-129">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="43e76-129">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="43e76-130">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="43e76-130">Request headers</span></span>
| <span data-ttu-id="43e76-131">名前</span><span class="sxs-lookup"><span data-stu-id="43e76-131">Name</span></span>      |<span data-ttu-id="43e76-132">説明</span><span class="sxs-lookup"><span data-stu-id="43e76-132">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="43e76-133">Authorization</span><span class="sxs-lookup"><span data-stu-id="43e76-133">Authorization</span></span>  | <span data-ttu-id="43e76-134">ベアラー &lt;コード&gt; が*必要*</span><span class="sxs-lookup"><span data-stu-id="43e76-134">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="43e76-135">承諾</span><span class="sxs-lookup"><span data-stu-id="43e76-135">Accept</span></span>  | <span data-ttu-id="43e76-136">application/json</span><span class="sxs-lookup"><span data-stu-id="43e76-136">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="43e76-137">要求本文</span><span class="sxs-lookup"><span data-stu-id="43e76-137">Request body</span></span>
<span data-ttu-id="43e76-138">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="43e76-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43e76-139">応答</span><span class="sxs-lookup"><span data-stu-id="43e76-139">Response</span></span>

<span data-ttu-id="43e76-140">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="43e76-140">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="43e76-141">例</span><span class="sxs-lookup"><span data-stu-id="43e76-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="43e76-142">要求</span><span class="sxs-lookup"><span data-stu-id="43e76-142">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="43e76-143">プロトコル</span><span class="sxs-lookup"><span data-stu-id="43e76-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```http
GET https://graph.microsoft.com/v1.0/directory/deletedItems/{object-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="43e76-144">C#</span><span class="sxs-lookup"><span data-stu-id="43e76-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="43e76-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="43e76-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="43e76-146">目的-C</span><span class="sxs-lookup"><span data-stu-id="43e76-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="43e76-147">Java</span><span class="sxs-lookup"><span data-stu-id="43e76-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-directory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="43e76-148">応答</span><span class="sxs-lookup"><span data-stu-id="43e76-148">Response</span></span>
<span data-ttu-id="43e76-p102">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="43e76-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
