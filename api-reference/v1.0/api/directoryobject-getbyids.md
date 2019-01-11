---
title: ID のリストからディレクトリ オブジェクトを取得します。
description: 選択 ' クエリ オプションはこの操作に使用できません。
author: lleonard-msft
localization_priority: Priority
ms.openlocfilehash: b504fc69deecd6688f61c20c30e17133f80b1dc8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889650"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="c5929-103">ID のリストからディレクトリ オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="c5929-103">Get directory objects from a list of ids</span></span>

<span data-ttu-id="c5929-p101">ID のリストで指定されたディレクトリ オブジェクトを返します。注:ここで返されるディレクトリ オブジェクトは、**すべて**のプロパティを含む完全なオブジェクトです。この操作に `$select` クエリ オプションは使用できません。</span><span class="sxs-lookup"><span data-stu-id="c5929-p101">Returns the directory objects specified in a list of ids.  NOTE: The directory objects returned are the full objects containing **all** their properties. The `$select` query option is not available for this operation.</span></span>

<span data-ttu-id="c5929-107">この関数の一般的な用途は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="c5929-107">Some common uses for this function are to:</span></span>

* <span data-ttu-id="c5929-108">[getMemberObjects](directoryobject-getmemberobjects.md) または [getMemberGroups](directoryobject-getmembergroups.md) などの (ID のコレクションを返す) 関数から返された ID を、バッキング ディレクトリ オブジェクトに解決する。</span><span class="sxs-lookup"><span data-stu-id="c5929-108">Resolve ids returned by functions (that return collections of ids) such as [getMemberObjects](directoryobject-getmemberobjects.md) or [getMemberGroups](directoryobject-getmembergroups.md)  to their backing directory objects.</span></span>
* <span data-ttu-id="c5929-109">アプリケーションによって外部記憶装置に保存されている ID をバッキング ディレクトリ オブジェクトに解決する。</span><span class="sxs-lookup"><span data-stu-id="c5929-109">Resolve ids persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5929-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c5929-110">Permissions</span></span>

<span data-ttu-id="c5929-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c5929-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c5929-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c5929-113">Permission type</span></span>      | <span data-ttu-id="c5929-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c5929-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5929-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c5929-115">Delegated (work or school account)</span></span> | <span data-ttu-id="c5929-116">Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c5929-116">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c5929-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c5929-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5929-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c5929-118">Not supported.</span></span>    |
|<span data-ttu-id="c5929-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c5929-119">Application</span></span> | <span data-ttu-id="c5929-120">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c5929-120">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5929-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c5929-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="c5929-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c5929-122">Request headers</span></span>

| <span data-ttu-id="c5929-123">名前</span><span class="sxs-lookup"><span data-stu-id="c5929-123">Name</span></span>       | <span data-ttu-id="c5929-124">種類</span><span class="sxs-lookup"><span data-stu-id="c5929-124">Type</span></span> | <span data-ttu-id="c5929-125">説明</span><span class="sxs-lookup"><span data-stu-id="c5929-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c5929-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5929-126">Authorization</span></span>  | <span data-ttu-id="c5929-127">string</span><span class="sxs-lookup"><span data-stu-id="c5929-127">string</span></span>  | <span data-ttu-id="c5929-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c5929-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c5929-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c5929-130">Content-Type</span></span>  | <span data-ttu-id="c5929-131">string</span><span class="sxs-lookup"><span data-stu-id="c5929-131">string</span></span> | <span data-ttu-id="c5929-132">application/json</span><span class="sxs-lookup"><span data-stu-id="c5929-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c5929-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="c5929-133">Request body</span></span>

<span data-ttu-id="c5929-134">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="c5929-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c5929-135">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c5929-135">Parameter</span></span>   | <span data-ttu-id="c5929-136">Type</span><span class="sxs-lookup"><span data-stu-id="c5929-136">Type</span></span> |<span data-ttu-id="c5929-137">説明</span><span class="sxs-lookup"><span data-stu-id="c5929-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c5929-138">ids</span><span class="sxs-lookup"><span data-stu-id="c5929-138">ids</span></span>|<span data-ttu-id="c5929-139">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c5929-139">String collection</span></span>| <span data-ttu-id="c5929-p104">オブジェクトを戻す ID のコレクション。最大 1000 ID まで指定できます。</span><span class="sxs-lookup"><span data-stu-id="c5929-p104">A collection of ids for which to return objects. You can specify up to 1000 ids.</span></span> |
|<span data-ttu-id="c5929-142">types</span><span class="sxs-lookup"><span data-stu-id="c5929-142">types</span></span>|<span data-ttu-id="c5929-143">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c5929-143">String collection</span></span>| <span data-ttu-id="c5929-144">検索するリソースのコレクションのセットを指定するリソースの種類のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="c5929-144">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="c5929-145">指定しない場合、既定では[directoryObject](../resources/directoryobject.md)、すべてのディレクトリで定義されているリソースの種類が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c5929-145">If not specified, the default is [directoryObject](../resources/directoryobject.md), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="c5929-146">派生したオブジェクトは、`directoryObject`コレクションに指定することがあります例:[ユーザー](../resources/user.md)、[グループ](../resources/group.md)、[デバイス](../resources/device.md)、およびようにします。</span><span class="sxs-lookup"><span data-stu-id="c5929-146">Any object that derives from `directoryObject` may be specified in the collection; for example: [user](../resources/user.md), [group](../resources/group.md), [device](../resources/device.md), and so on.</span></span> <span data-ttu-id="c5929-147">値は、大文字小文字を区別しません。</span><span class="sxs-lookup"><span data-stu-id="c5929-147">The values are not case-sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="c5929-148">応答</span><span class="sxs-lookup"><span data-stu-id="c5929-148">Response</span></span>

<span data-ttu-id="c5929-149">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c5929-149">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c5929-150">例</span><span class="sxs-lookup"><span data-stu-id="c5929-150">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c5929-151">要求</span><span class="sxs-lookup"><span data-stu-id="c5929-151">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_getById"
}-->

```http
POST https://graph.microsoft.com/v1.0/directoryObjects/getByIds
Content-type: application/json

{
    "ids":["84b80893874940a3-97b7-68513b600544","5d6059b6368d-45f8-91e18e07d485f1d0"],
    "types":["user"]
}
```

##### <a name="response"></a><span data-ttu-id="c5929-152">応答</span><span class="sxs-lookup"><span data-stu-id="c5929-152">Response</span></span>

<span data-ttu-id="c5929-p106">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c5929-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects",
    "value": [
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Trevor Jones"
      },
      {
        "@odata.type": "#microsoft.graph.user",
        "id": "84b80893-8749-40a3-97b7-68513b600544",
        "accountEnabled": true,
        "displayName": "Billy Smith"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject: getById",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
