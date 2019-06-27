---
title: ID のリストからディレクトリ オブジェクトを取得します。
description: この操作に ` クエリ オプションは使用できません。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7392dec92b25e9d4f651503f393b9d7d7d8a9ffe
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260775"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="66d3c-103">ID のリストからディレクトリ オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="66d3c-103">Get directory objects from a list of ids</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66d3c-p101">ID のリストで指定されたディレクトリ オブジェクトを返します。注:ここで返されるディレクトリ オブジェクトは、**すべて**のプロパティを含む完全なオブジェクトです。この操作に `$select` クエリ オプションは使用できません。</span><span class="sxs-lookup"><span data-stu-id="66d3c-p101">Returns the directory objects specified in a list of ids.  NOTE: The directory objects returned are the full objects containing **all** their properties. The `$select` query option is not available for this operation.</span></span>

<span data-ttu-id="66d3c-107">この関数の一般的な用途は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="66d3c-107">Some common uses for this function are to:</span></span>

* <span data-ttu-id="66d3c-108">[getMemberObjects](/graph/api/directoryobject-getmemberobjects.md?view=graph-rest-beta) または [getMemberGroups](/graph/api/directoryobject-getmembergroups.md?view=graph-rest-beta) などの (ID のコレクションを返す) 関数から返された ID を、バッキング ディレクトリ オブジェクトに解決する。</span><span class="sxs-lookup"><span data-stu-id="66d3c-108">Resolve ids returned by functions (that return collections of ids) such as [getMemberObjects](/graph/api/directoryobject-getmemberobjects.md?view=graph-rest-beta) or [getMemberGroups](/graph/api/directoryobject-getmembergroups.md?view=graph-rest-beta)  to their backing directory objects.</span></span>
* <span data-ttu-id="66d3c-109">アプリケーションによって外部記憶装置に保存されている ID をバッキング ディレクトリ オブジェクトに解決する。</span><span class="sxs-lookup"><span data-stu-id="66d3c-109">Resolve ids persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="66d3c-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="66d3c-110">Permissions</span></span>

<span data-ttu-id="66d3c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="66d3c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="66d3c-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="66d3c-113">Permission type</span></span>      | <span data-ttu-id="66d3c-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="66d3c-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66d3c-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="66d3c-115">Delegated (work or school account)</span></span> | <span data-ttu-id="66d3c-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="66d3c-116">Directory.Read.All</span></span>    |
|<span data-ttu-id="66d3c-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="66d3c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66d3c-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66d3c-118">Not supported.</span></span>    |
|<span data-ttu-id="66d3c-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="66d3c-119">Application</span></span> | <span data-ttu-id="66d3c-120">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="66d3c-120">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="66d3c-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="66d3c-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="66d3c-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="66d3c-122">Request headers</span></span>

| <span data-ttu-id="66d3c-123">名前</span><span class="sxs-lookup"><span data-stu-id="66d3c-123">Name</span></span>       | <span data-ttu-id="66d3c-124">型</span><span class="sxs-lookup"><span data-stu-id="66d3c-124">Type</span></span> | <span data-ttu-id="66d3c-125">説明</span><span class="sxs-lookup"><span data-stu-id="66d3c-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="66d3c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="66d3c-126">Authorization</span></span>  | <span data-ttu-id="66d3c-127">string</span><span class="sxs-lookup"><span data-stu-id="66d3c-127">string</span></span>  | <span data-ttu-id="66d3c-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="66d3c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="66d3c-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="66d3c-130">Content-Type</span></span>  | <span data-ttu-id="66d3c-131">application/json</span><span class="sxs-lookup"><span data-stu-id="66d3c-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="66d3c-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="66d3c-132">Request body</span></span>

<span data-ttu-id="66d3c-133">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="66d3c-133">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="66d3c-134">パラメーター</span><span class="sxs-lookup"><span data-stu-id="66d3c-134">Parameter</span></span>   | <span data-ttu-id="66d3c-135">型</span><span class="sxs-lookup"><span data-stu-id="66d3c-135">Type</span></span> |<span data-ttu-id="66d3c-136">説明</span><span class="sxs-lookup"><span data-stu-id="66d3c-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="66d3c-137">ids</span><span class="sxs-lookup"><span data-stu-id="66d3c-137">ids</span></span>|<span data-ttu-id="66d3c-138">String collection</span><span class="sxs-lookup"><span data-stu-id="66d3c-138">String collection</span></span>| <span data-ttu-id="66d3c-p104">オブジェクトを戻す ID のコレクション。最大 1000 ID まで指定できます。</span><span class="sxs-lookup"><span data-stu-id="66d3c-p104">A collection of ids for which to return objects. You can specify up to 1000 ids.</span></span> |
|<span data-ttu-id="66d3c-141">types</span><span class="sxs-lookup"><span data-stu-id="66d3c-141">types</span></span>|<span data-ttu-id="66d3c-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="66d3c-142">String collection</span></span>| <span data-ttu-id="66d3c-143">検索する一連のリソース コレクションを指定するリソース型のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="66d3c-143">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="66d3c-144">指定しない場合、既定値は、ディレクトリで定義されているすべてのリソース型を含む [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta) になります。</span><span class="sxs-lookup"><span data-stu-id="66d3c-144">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="66d3c-145">[directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta) から派生する任意のオブジェクトをコレクションに指定できます。例: [user](/graph/api/resources/user?view=graph-rest-beta)、[group](/graph/api/resources/group?view=graph-rest-beta)、[device](/graph/api/resources/device?view=graph-rest-beta) など。</span><span class="sxs-lookup"><span data-stu-id="66d3c-145">Any object that derives from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta) may be specified in the collection; for example: [user](/graph/api/resources/user?view=graph-rest-beta), [group](/graph/api/resources/group?view=graph-rest-beta), [device](/graph/api/resources/device?view=graph-rest-beta), and so on.</span></span> <span data-ttu-id="66d3c-146">[クラウド ソリューション プロバイダー](https://partner.microsoft.com/en-us/cloud-solution-provider) パートナー組織への参照を検索するには、[directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta) を指定します。</span><span class="sxs-lookup"><span data-stu-id="66d3c-146">To search for references to a [Cloud Solution Provider](https://partner.microsoft.com/en-us/cloud-solution-provider) partner organization specify [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta).</span></span> <span data-ttu-id="66d3c-147">指定しない場合、既定値は、ディレクトリで定義されているすべてのリソース型を含む [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta) になります ([クラウド ソリューション プロバイダー](https://partner.microsoft.com/en-us/cloud-solution-provider) パートナー組織への参照をのぞく)。</span><span class="sxs-lookup"><span data-stu-id="66d3c-147">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-beta), which contains all of the resource types defined in the directory, except for references to a [Cloud Solution Provider](https://partner.microsoft.com/en-us/cloud-solution-provider) partner organization.</span></span> <span data-ttu-id="66d3c-148">値では、大文字と小文字は区別されません。</span><span class="sxs-lookup"><span data-stu-id="66d3c-148">The values are not case-sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="66d3c-149">応答</span><span class="sxs-lookup"><span data-stu-id="66d3c-149">Response</span></span>

<span data-ttu-id="66d3c-150">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="66d3c-150">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66d3c-151">例</span><span class="sxs-lookup"><span data-stu-id="66d3c-151">Example</span></span>

##### <a name="request"></a><span data-ttu-id="66d3c-152">要求</span><span class="sxs-lookup"><span data-stu-id="66d3c-152">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="66d3c-153">応答</span><span class="sxs-lookup"><span data-stu-id="66d3c-153">Response</span></span>

<span data-ttu-id="66d3c-p106">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="66d3c-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="66d3c-156">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="66d3c-156">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="66d3c-157">C#</span><span class="sxs-lookup"><span data-stu-id="66d3c-157">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/directoryobject_getByIds-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="66d3c-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="66d3c-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/directoryobject_getByIds-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="66d3c-159">目的-C</span><span class="sxs-lookup"><span data-stu-id="66d3c-159">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/directoryobject_getByIds-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject: getById",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryobject-getbyids.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/directoryobject-getbyids.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directoryobject-getbyids.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
