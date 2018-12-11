---
title: ID のリストからディレクトリ オブジェクトを取得します。
description: 選択 ' クエリ オプションはこの操作に使用できません。
ms.openlocfilehash: e6f987a3269b209c5df71b4961cf73081286a76d
ms.sourcegitcommit: 72d4da2a6bfaf99fa4edaf6ce3b97b1a6d96d874
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/11/2018
ms.locfileid: "27222450"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="c601c-103">ID のリストからディレクトリ オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="c601c-103">Get directory objects from a list of ids</span></span>

> <span data-ttu-id="c601c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c601c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c601c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c601c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c601c-p102">ID のリストで指定されたディレクトリ オブジェクトを返します。注:ここで返されるディレクトリ オブジェクトは、**すべて**のプロパティを含む完全なオブジェクトです。この操作に `$select` クエリ オプションは使用できません。</span><span class="sxs-lookup"><span data-stu-id="c601c-p102">Returns the directory objects specified in a list of ids.  NOTE: The directory objects returned are the full objects containing **all** their properties. The `$select` query option is not available for this operation.</span></span>

<span data-ttu-id="c601c-109">この関数の一般的な用途は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="c601c-109">Some common uses for this function are to:</span></span>

* <span data-ttu-id="c601c-110">[getMemberObjects](/graph/api/directoryobject-getmemberobjects.md?view=graph-rest-beta) または [getMemberGroups](/graph/api/directoryobject-getmembergroups.md?view=graph-rest-beta) などの (ID のコレクションを返す) 関数から返された ID を、バッキング ディレクトリ オブジェクトに解決する。</span><span class="sxs-lookup"><span data-stu-id="c601c-110">Resolve ids returned by functions (that return collections of ids) such as [getMemberObjects](/graph/api/directoryobject-getmemberobjects.md?view=graph-rest-beta) or [getMemberGroups](/graph/api/directoryobject-getmembergroups.md?view=graph-rest-beta)  to their backing directory objects.</span></span>
* <span data-ttu-id="c601c-111">アプリケーションによって外部記憶装置に保存されている ID をバッキング ディレクトリ オブジェクトに解決する。</span><span class="sxs-lookup"><span data-stu-id="c601c-111">Resolve ids persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c601c-112">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c601c-112">Permissions</span></span>

<span data-ttu-id="c601c-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c601c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c601c-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c601c-115">Permission type</span></span>      | <span data-ttu-id="c601c-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c601c-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c601c-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c601c-117">Delegated (work or school account)</span></span> | <span data-ttu-id="c601c-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c601c-118">Directory.Read.All</span></span>    |
|<span data-ttu-id="c601c-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c601c-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c601c-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c601c-120">Not supported.</span></span>    |
|<span data-ttu-id="c601c-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c601c-121">Application</span></span> | <span data-ttu-id="c601c-122">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="c601c-122">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c601c-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c601c-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="c601c-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c601c-124">Request headers</span></span>

| <span data-ttu-id="c601c-125">名前</span><span class="sxs-lookup"><span data-stu-id="c601c-125">Name</span></span>       | <span data-ttu-id="c601c-126">種類</span><span class="sxs-lookup"><span data-stu-id="c601c-126">Type</span></span> | <span data-ttu-id="c601c-127">説明</span><span class="sxs-lookup"><span data-stu-id="c601c-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c601c-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="c601c-128">Authorization</span></span>  | <span data-ttu-id="c601c-129">string</span><span class="sxs-lookup"><span data-stu-id="c601c-129">string</span></span>  | <span data-ttu-id="c601c-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c601c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c601c-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c601c-132">Content-Type</span></span>  | <span data-ttu-id="c601c-133">application/json</span><span class="sxs-lookup"><span data-stu-id="c601c-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c601c-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="c601c-134">Request body</span></span>

<span data-ttu-id="c601c-135">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="c601c-135">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c601c-136">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c601c-136">Parameter</span></span>   | <span data-ttu-id="c601c-137">Type</span><span class="sxs-lookup"><span data-stu-id="c601c-137">Type</span></span> |<span data-ttu-id="c601c-138">説明</span><span class="sxs-lookup"><span data-stu-id="c601c-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c601c-139">ids</span><span class="sxs-lookup"><span data-stu-id="c601c-139">ids</span></span>|<span data-ttu-id="c601c-140">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c601c-140">String collection</span></span>| <span data-ttu-id="c601c-p105">オブジェクトを戻す ID のコレクション。最大 1000 ID まで指定できます。</span><span class="sxs-lookup"><span data-stu-id="c601c-p105">A collection of ids for which to return objects. You can specify up to 1000 ids.</span></span> |
|<span data-ttu-id="c601c-143">types</span><span class="sxs-lookup"><span data-stu-id="c601c-143">types</span></span>|<span data-ttu-id="c601c-144">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c601c-144">String collection</span></span>| <span data-ttu-id="c601c-145">検索するリソースのコレクションのセットを指定するリソースの種類のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="c601c-145">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="c601c-146">指定しない場合、既定では[directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta)、すべてのディレクトリで定義されているリソースの種類が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c601c-146">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="c601c-147">[DirectoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta)から派生した任意のオブジェクトをコレクションに指定する場合があります。例:[ユーザー](/graph/api/resources/user?view=graph-rest-beta)、[グループ](/graph/api/resources/group?view=graph-rest-beta)、[デバイス](/graph/api/resources/device?view=graph-rest-beta)、およびようにします。</span><span class="sxs-lookup"><span data-stu-id="c601c-147">Any object that derives from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta) may be specified in the collection; for example: [user](/graph/api/resources/user?view=graph-rest-beta), [group](/graph/api/resources/group?view=graph-rest-beta), [device](/graph/api/resources/device?view=graph-rest-beta), and so on.</span></span> <span data-ttu-id="c601c-148">[クラウド ソリューション プロバイダー](https://partner.microsoft.com/en-us/cloud-solution-provider)パートナーへの参照を検索するのには、組織は、 [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta)を指定します。</span><span class="sxs-lookup"><span data-stu-id="c601c-148">To search for references to a [Cloud Solution Provider](https://partner.microsoft.com/en-us/cloud-solution-provider) partner organization specify [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta).</span></span> <span data-ttu-id="c601c-149">指定しない場合、既定では[directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta)、すべての[クラウド ソリューション プロバイダー](https://partner.microsoft.com/en-us/cloud-solution-provider)パートナーの組織への参照を除いて、ディレクトリで定義されているリソースの種類が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c601c-149">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), which contains all of the resource types defined in the directory, except for references to a [Cloud Solution Provider](https://partner.microsoft.com/en-us/cloud-solution-provider) partner organization.</span></span> <span data-ttu-id="c601c-150">値は、大文字小文字を区別しません。</span><span class="sxs-lookup"><span data-stu-id="c601c-150">The values are not case-sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="c601c-151">応答</span><span class="sxs-lookup"><span data-stu-id="c601c-151">Response</span></span>

<span data-ttu-id="c601c-152">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c601c-152">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c601c-153">例</span><span class="sxs-lookup"><span data-stu-id="c601c-153">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c601c-154">要求</span><span class="sxs-lookup"><span data-stu-id="c601c-154">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_getByIds"
}-->

```http
POST https://graph.microsoft.com/beta/directoryObjects/getByIds
Content-type: application/json

{
    "ids":["84b80893-8749-40a3-97b7-68513b600544","5d6059b6-368d-45f8-91e1-8e07d485f1d0"],
    "types":["user"]
}
```

##### <a name="response"></a><span data-ttu-id="c601c-155">応答</span><span class="sxs-lookup"><span data-stu-id="c601c-155">Response</span></span>

<span data-ttu-id="c601c-p107">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c601c-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryObjects",
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
