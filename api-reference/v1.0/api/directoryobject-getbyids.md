---
title: ID のリストからディレクトリ オブジェクトを取得します。
description: この操作に ` クエリ オプションは使用できません。
author: lleonard-msft
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a209d391c72edd453bbfe9232b7d02121ca98128
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572011"
---
# <a name="get-directory-objects-from-a-list-of-ids"></a><span data-ttu-id="1d98e-103">ID のリストからディレクトリ オブジェクトを取得します。</span><span class="sxs-lookup"><span data-stu-id="1d98e-103">Get directory objects from a list of ids</span></span>

<span data-ttu-id="1d98e-p101">ID のリストで指定されたディレクトリ オブジェクトを返します。注:ここで返されるディレクトリ オブジェクトは、**すべて**のプロパティを含む完全なオブジェクトです。この操作に `$select` クエリ オプションは使用できません。</span><span class="sxs-lookup"><span data-stu-id="1d98e-p101">Returns the directory objects specified in a list of ids.  NOTE: The directory objects returned are the full objects containing **all** their properties. The `$select` query option is not available for this operation.</span></span>

<span data-ttu-id="1d98e-107">この関数の一般的な用途は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="1d98e-107">Some common uses for this function are to:</span></span>

* <span data-ttu-id="1d98e-108">[getMemberObjects](directoryobject-getmemberobjects.md) または [getMemberGroups](directoryobject-getmembergroups.md) などの (ID のコレクションを返す) 関数から返された ID を、バッキング ディレクトリ オブジェクトに解決する。</span><span class="sxs-lookup"><span data-stu-id="1d98e-108">Resolve ids returned by functions (that return collections of ids) such as [getMemberObjects](directoryobject-getmemberobjects.md) or [getMemberGroups](directoryobject-getmembergroups.md)  to their backing directory objects.</span></span>
* <span data-ttu-id="1d98e-109">アプリケーションによって外部記憶装置に保存されている ID をバッキング ディレクトリ オブジェクトに解決する。</span><span class="sxs-lookup"><span data-stu-id="1d98e-109">Resolve ids persisted in an external store by the application to their backing directory objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="1d98e-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1d98e-110">Permissions</span></span>

<span data-ttu-id="1d98e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1d98e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1d98e-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1d98e-113">Permission type</span></span>      | <span data-ttu-id="1d98e-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1d98e-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1d98e-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1d98e-115">Delegated (work or school account)</span></span> | <span data-ttu-id="1d98e-116">Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1d98e-116">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1d98e-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1d98e-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1d98e-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d98e-118">Not supported.</span></span>    |
|<span data-ttu-id="1d98e-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1d98e-119">Application</span></span> | <span data-ttu-id="1d98e-120">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="1d98e-120">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1d98e-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1d98e-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /directoryObjects/getByIds
```

## <a name="request-headers"></a><span data-ttu-id="1d98e-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1d98e-122">Request headers</span></span>

| <span data-ttu-id="1d98e-123">名前</span><span class="sxs-lookup"><span data-stu-id="1d98e-123">Name</span></span>       | <span data-ttu-id="1d98e-124">型</span><span class="sxs-lookup"><span data-stu-id="1d98e-124">Type</span></span> | <span data-ttu-id="1d98e-125">説明</span><span class="sxs-lookup"><span data-stu-id="1d98e-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1d98e-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="1d98e-126">Authorization</span></span>  | <span data-ttu-id="1d98e-127">string</span><span class="sxs-lookup"><span data-stu-id="1d98e-127">string</span></span>  | <span data-ttu-id="1d98e-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1d98e-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1d98e-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1d98e-130">Content-Type</span></span>  | <span data-ttu-id="1d98e-131">string</span><span class="sxs-lookup"><span data-stu-id="1d98e-131">string</span></span> | <span data-ttu-id="1d98e-132">application/json</span><span class="sxs-lookup"><span data-stu-id="1d98e-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1d98e-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="1d98e-133">Request body</span></span>

<span data-ttu-id="1d98e-134">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="1d98e-134">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1d98e-135">パラメーター</span><span class="sxs-lookup"><span data-stu-id="1d98e-135">Parameter</span></span>   | <span data-ttu-id="1d98e-136">型</span><span class="sxs-lookup"><span data-stu-id="1d98e-136">Type</span></span> |<span data-ttu-id="1d98e-137">説明</span><span class="sxs-lookup"><span data-stu-id="1d98e-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1d98e-138">ids</span><span class="sxs-lookup"><span data-stu-id="1d98e-138">ids</span></span>|<span data-ttu-id="1d98e-139">String collection</span><span class="sxs-lookup"><span data-stu-id="1d98e-139">String collection</span></span>| <span data-ttu-id="1d98e-p104">オブジェクトを戻す ID のコレクション。最大 1000 ID まで指定できます。</span><span class="sxs-lookup"><span data-stu-id="1d98e-p104">A collection of ids for which to return objects. You can specify up to 1000 ids.</span></span> |
|<span data-ttu-id="1d98e-142">types</span><span class="sxs-lookup"><span data-stu-id="1d98e-142">types</span></span>|<span data-ttu-id="1d98e-143">String コレクション</span><span class="sxs-lookup"><span data-stu-id="1d98e-143">String collection</span></span>| <span data-ttu-id="1d98e-144">検索する一連のリソース コレクションを指定するリソース型のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="1d98e-144">A collection of resource types that specifies the set of resource collections to search.</span></span> <span data-ttu-id="1d98e-145">指定しない場合、既定値は、ディレクトリで定義されているすべてのリソース型を含む [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) になります。</span><span class="sxs-lookup"><span data-stu-id="1d98e-145">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), which contains all of the resource types defined in the directory.</span></span> <span data-ttu-id="1d98e-146">[directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) から派生する任意のオブジェクトをコレクションに指定できます。例: [user](/graph/api/resources/user?view=graph-rest-v1.0)、[group](/graph/api/resources/group?view=graph-rest-v1.0)、[device](/graph/api/resources/device?view=graph-rest-v1.0) など。</span><span class="sxs-lookup"><span data-stu-id="1d98e-146">Any object that derives from [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) may be specified in the collection; for example: [user](/graph/api/resources/user?view=graph-rest-v1.0), [group](/graph/api/resources/group?view=graph-rest-v1.0), [device](/graph/api/resources/device?view=graph-rest-v1.0), and so on.</span></span> <span data-ttu-id="1d98e-147">[クラウド ソリューション プロバイダー](https://partner.microsoft.com/ja-JP/cloud-solution-provider) パートナー組織への参照を検索するには、[directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-v1.0) を指定します。</span><span class="sxs-lookup"><span data-stu-id="1d98e-147">To search for references to a [Cloud Solution Provider](https://partner.microsoft.com/ja-JP/cloud-solution-provider) partner organization specify [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-v1.0).</span></span> <span data-ttu-id="1d98e-148">指定しない場合、既定値は、ディレクトリで定義されているすべてのリソース型を含む [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0) になります ([クラウド ソリューション プロバイダー](https://partner.microsoft.com/ja-JP/cloud-solution-provider) パートナー組織への参照をのぞく)。</span><span class="sxs-lookup"><span data-stu-id="1d98e-148">If not specified, the default is [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-v1.0), which contains all of the resource types defined in the directory, except for references to a [Cloud Solution Provider](https://partner.microsoft.com/ja-JP/cloud-solution-provider) partner organization.</span></span> <span data-ttu-id="1d98e-149">値では、大文字と小文字は区別されません。</span><span class="sxs-lookup"><span data-stu-id="1d98e-149">The values are not case-sensitive.</span></span>|

## <a name="response"></a><span data-ttu-id="1d98e-150">応答</span><span class="sxs-lookup"><span data-stu-id="1d98e-150">Response</span></span>

<span data-ttu-id="1d98e-151">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1d98e-151">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d98e-152">例</span><span class="sxs-lookup"><span data-stu-id="1d98e-152">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1d98e-153">要求</span><span class="sxs-lookup"><span data-stu-id="1d98e-153">Request</span></span>

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

##### <a name="response"></a><span data-ttu-id="1d98e-154">応答</span><span class="sxs-lookup"><span data-stu-id="1d98e-154">Response</span></span>

<span data-ttu-id="1d98e-p106">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1d98e-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
