---
title: childFolders を一覧表示する
description: 指定した連絡先フォルダーの下の子フォルダーのコレクションを取得します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5e4230976e032ff77189bf0b691ddcd365e92522
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507846"
---
# <a name="list-childfolders"></a><span data-ttu-id="78518-103">childFolders を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="78518-103">List childFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78518-104">指定した連絡先フォルダーの下の子フォルダーのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="78518-104">Get a collection of child folders under the specified contact folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="78518-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="78518-105">Permissions</span></span>
<span data-ttu-id="78518-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="78518-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78518-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="78518-108">Permission type</span></span>      | <span data-ttu-id="78518-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="78518-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78518-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="78518-110">Delegated (work or school account)</span></span> | <span data-ttu-id="78518-111">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="78518-111">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="78518-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="78518-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78518-113">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="78518-113">Contacts.Read, Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="78518-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="78518-114">Application</span></span> | <span data-ttu-id="78518-115">Contacts.Read、Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="78518-115">Contacts.Read, Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="78518-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="78518-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/contactFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="78518-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="78518-117">Optional query parameters</span></span>
<span data-ttu-id="78518-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="78518-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="78518-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="78518-119">Request headers</span></span>
| <span data-ttu-id="78518-120">名前</span><span class="sxs-lookup"><span data-stu-id="78518-120">Name</span></span>       | <span data-ttu-id="78518-121">型</span><span class="sxs-lookup"><span data-stu-id="78518-121">Type</span></span> | <span data-ttu-id="78518-122">説明</span><span class="sxs-lookup"><span data-stu-id="78518-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="78518-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="78518-123">Authorization</span></span>  | <span data-ttu-id="78518-124">string</span><span class="sxs-lookup"><span data-stu-id="78518-124">string</span></span>  | <span data-ttu-id="78518-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="78518-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="78518-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="78518-127">Request body</span></span>
<span data-ttu-id="78518-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="78518-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="78518-129">応答</span><span class="sxs-lookup"><span data-stu-id="78518-129">Response</span></span>

<span data-ttu-id="78518-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [ContactFolder](../resources/contactfolder.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="78518-130">If successful, this method returns a `200 OK` response code and collection of [ContactFolder](../resources/contactfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="78518-131">例</span><span class="sxs-lookup"><span data-stu-id="78518-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="78518-132">要求</span><span class="sxs-lookup"><span data-stu-id="78518-132">Request</span></span>
<span data-ttu-id="78518-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="78518-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/contactFolders/{id}/childFolders
```
##### <a name="response"></a><span data-ttu-id="78518-134">応答</span><span class="sxs-lookup"><span data-stu-id="78518-134">Response</span></span>
<span data-ttu-id="78518-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="78518-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 145

{
  "value": [
    {
      "parentFolderId": "parentFolderId-value",
      "displayName": "displayName-value",
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
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/contactfolder-list-childfolders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
