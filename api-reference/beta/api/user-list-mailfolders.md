---
title: mailFolders を一覧表示する　
description: サインインしているユーザーのメールボックス内のすべてのメールフォルダーを取得します。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 64b96620d30188c720beaae4875712b1dc8d8e37
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544330"
---
# <a name="list-mailfolders"></a><span data-ttu-id="aac07-103">mailFolders を一覧表示する　</span><span class="sxs-lookup"><span data-stu-id="aac07-103">List mailFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aac07-104">サインインしているユーザーのメールボックス内のすべてのメールフォルダーを取得します。</span><span class="sxs-lookup"><span data-stu-id="aac07-104">Get all the mail folders in the signed-in user's mailbox.</span></span>

## <a name="permissions"></a><span data-ttu-id="aac07-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="aac07-105">Permissions</span></span>
<span data-ttu-id="aac07-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aac07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aac07-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="aac07-108">Permission type</span></span>      | <span data-ttu-id="aac07-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="aac07-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aac07-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="aac07-110">Delegated (work or school account)</span></span> | <span data-ttu-id="aac07-111">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aac07-111">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="aac07-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="aac07-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aac07-113">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aac07-113">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="aac07-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="aac07-114">Application</span></span> | <span data-ttu-id="aac07-115">Mail.Read、Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aac07-115">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="aac07-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="aac07-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders
GET /users/{id | userPrincipalName}/mailFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="aac07-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="aac07-117">Optional query parameters</span></span>
<span data-ttu-id="aac07-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="aac07-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="aac07-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aac07-119">Request headers</span></span>
| <span data-ttu-id="aac07-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aac07-120">Header</span></span>       | <span data-ttu-id="aac07-121">値</span><span class="sxs-lookup"><span data-stu-id="aac07-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="aac07-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="aac07-122">Authorization</span></span>  | <span data-ttu-id="aac07-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="aac07-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="aac07-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="aac07-125">Content-Type</span></span>   | <span data-ttu-id="aac07-126">application/json</span><span class="sxs-lookup"><span data-stu-id="aac07-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="aac07-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="aac07-127">Request body</span></span>
<span data-ttu-id="aac07-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="aac07-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aac07-129">応答</span><span class="sxs-lookup"><span data-stu-id="aac07-129">Response</span></span>

<span data-ttu-id="aac07-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [MailFolder](../resources/mailfolder.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="aac07-130">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="aac07-131">例</span><span class="sxs-lookup"><span data-stu-id="aac07-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aac07-132">要求</span><span class="sxs-lookup"><span data-stu-id="aac07-132">Request</span></span>
<span data-ttu-id="aac07-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="aac07-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders
```
##### <a name="response"></a><span data-ttu-id="aac07-134">応答</span><span class="sxs-lookup"><span data-stu-id="aac07-134">Response</span></span>
<span data-ttu-id="aac07-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="aac07-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
  "value": [
    {
      "displayName": "displayName-value",
      "parentFolderId": "parentFolderId-value",
      "childFolderCount": 99,
      "unreadItemCount": 99,
      "totalItemCount": 99,
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
  "description": "List mailFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-mailfolders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
