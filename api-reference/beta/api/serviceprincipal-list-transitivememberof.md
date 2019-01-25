---
title: リスト servicePrincipal 推移的な所属するグループ
description: このサービス主体のメンバーであるグループおよびディレクトリの役割を取得します。 この操作では、推移的では、このサービス ・ プリンシパルには、入れ子にされたメンバーのすべてのグループが含まれます。
localization_priority: Normal
ms.openlocfilehash: 4588f5ea4c6190b3743988c1d97bfd5caacbfaa4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526229"
---
# <a name="list-serviceprincipal-transitive-memberof"></a><span data-ttu-id="66758-104">リスト servicePrincipal 推移的な所属するグループ</span><span class="sxs-lookup"><span data-stu-id="66758-104">List servicePrincipal transitive memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66758-105">このサービス主体のメンバーであるグループおよびディレクトリの役割を取得します。</span><span class="sxs-lookup"><span data-stu-id="66758-105">Get the groups and directory roles that this service principal is a member of.</span></span> <span data-ttu-id="66758-106">この操作では、推移的では、このサービス ・ プリンシパルには、入れ子にされたメンバーのすべてのグループが含まれます。</span><span class="sxs-lookup"><span data-stu-id="66758-106">This operation is transitive and will include all groups that this service principal is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="66758-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="66758-107">Permissions</span></span>
<span data-ttu-id="66758-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="66758-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66758-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="66758-110">Permission type</span></span>      | <span data-ttu-id="66758-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="66758-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66758-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="66758-112">Delegated (work or school account)</span></span> | <span data-ttu-id="66758-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="66758-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="66758-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="66758-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66758-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66758-115">Not supported.</span></span>    |
|<span data-ttu-id="66758-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="66758-116">Application</span></span> | <span data-ttu-id="66758-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66758-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="66758-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="66758-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="66758-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="66758-119">Optional query parameters</span></span>
<span data-ttu-id="66758-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="66758-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="66758-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="66758-121">Request headers</span></span>
| <span data-ttu-id="66758-122">名前</span><span class="sxs-lookup"><span data-stu-id="66758-122">Name</span></span>       | <span data-ttu-id="66758-123">型</span><span class="sxs-lookup"><span data-stu-id="66758-123">Type</span></span> | <span data-ttu-id="66758-124">説明</span><span class="sxs-lookup"><span data-stu-id="66758-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="66758-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="66758-125">Authorization</span></span>  | <span data-ttu-id="66758-126">string</span><span class="sxs-lookup"><span data-stu-id="66758-126">string</span></span>  | <span data-ttu-id="66758-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="66758-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66758-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="66758-129">Request body</span></span>
<span data-ttu-id="66758-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="66758-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="66758-131">応答</span><span class="sxs-lookup"><span data-stu-id="66758-131">Response</span></span>

<span data-ttu-id="66758-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="66758-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66758-133">例</span><span class="sxs-lookup"><span data-stu-id="66758-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="66758-134">要求</span><span class="sxs-lookup"><span data-stu-id="66758-134">Request</span></span>

<span data-ttu-id="66758-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="66758-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf
```

### <a name="response"></a><span data-ttu-id="66758-136">応答</span><span class="sxs-lookup"><span data-stu-id="66758-136">Response</span></span>

<span data-ttu-id="66758-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="66758-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List servicePrincipal memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-list-transitivememberof.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
