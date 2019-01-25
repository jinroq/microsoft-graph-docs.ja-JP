---
title: ownedObjects を一覧表示する　
description: ユーザーが所有しているディレクトリ オブジェクトの一覧を取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9436b1aa225885f007268e72cb35f83810db835c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525578"
---
# <a name="list-ownedobjects"></a><span data-ttu-id="17d48-103">ownedObjects を一覧表示する　</span><span class="sxs-lookup"><span data-stu-id="17d48-103">List ownedObjects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17d48-104">ユーザーが所有しているディレクトリ オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="17d48-104">Get the list of directory objects that are owned by the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="17d48-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="17d48-105">Permissions</span></span>
<span data-ttu-id="17d48-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="17d48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17d48-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="17d48-108">Permission type</span></span>      | <span data-ttu-id="17d48-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="17d48-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17d48-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="17d48-110">Delegated (work or school account)</span></span> | <span data-ttu-id="17d48-111">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="17d48-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="17d48-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="17d48-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17d48-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="17d48-113">Not supported.</span></span>    |
|<span data-ttu-id="17d48-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="17d48-114">Application</span></span> | <span data-ttu-id="17d48-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17d48-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="17d48-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="17d48-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/ownedObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="17d48-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="17d48-117">Optional query parameters</span></span>
<span data-ttu-id="17d48-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="17d48-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="17d48-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="17d48-119">Request headers</span></span>
| <span data-ttu-id="17d48-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="17d48-120">Header</span></span>       | <span data-ttu-id="17d48-121">値</span><span class="sxs-lookup"><span data-stu-id="17d48-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="17d48-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="17d48-122">Authorization</span></span>  | <span data-ttu-id="17d48-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="17d48-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="17d48-125">承諾</span><span class="sxs-lookup"><span data-stu-id="17d48-125">Accept</span></span>  | <span data-ttu-id="17d48-126">application/json</span><span class="sxs-lookup"><span data-stu-id="17d48-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="17d48-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="17d48-127">Request body</span></span>
<span data-ttu-id="17d48-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="17d48-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17d48-129">応答</span><span class="sxs-lookup"><span data-stu-id="17d48-129">Response</span></span>

<span data-ttu-id="17d48-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="17d48-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="17d48-131">例</span><span class="sxs-lookup"><span data-stu-id="17d48-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="17d48-132">要求</span><span class="sxs-lookup"><span data-stu-id="17d48-132">Request</span></span>
<span data-ttu-id="17d48-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="17d48-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_ownedobjects"
}-->
```http
GET https://graph.microsoft.com/beta/me/ownedObjects
```
##### <a name="response"></a><span data-ttu-id="17d48-134">応答</span><span class="sxs-lookup"><span data-stu-id="17d48-134">Response</span></span>
<span data-ttu-id="17d48-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="17d48-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List ownedObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-ownedobjects.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
