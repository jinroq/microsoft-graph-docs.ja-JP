---
title: アプリケーションを一覧表示する
description: この組織内のアプリケーションの一覧を取得します。
author: lleonard-msft
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 802bf9197ad7574dbf2480fb7c0631e3fd212d9d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524682"
---
# <a name="list-applications"></a><span data-ttu-id="e97af-103">アプリケーションを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="e97af-103">List applications</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e97af-104">この組織内のアプリケーションの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="e97af-104">Retrieve the list of applications in this organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="e97af-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e97af-105">Permissions</span></span>
<span data-ttu-id="e97af-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e97af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e97af-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e97af-108">Permission type</span></span>      | <span data-ttu-id="e97af-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e97af-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e97af-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e97af-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e97af-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e97af-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e97af-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e97af-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e97af-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e97af-113">Not supported.</span></span>    |
|<span data-ttu-id="e97af-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e97af-114">Application</span></span> | <span data-ttu-id="e97af-115">Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e97af-115">Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e97af-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e97af-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /applications
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e97af-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e97af-117">Optional query parameters</span></span>
<span data-ttu-id="e97af-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e97af-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e97af-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e97af-119">Request headers</span></span>
| <span data-ttu-id="e97af-120">名前</span><span class="sxs-lookup"><span data-stu-id="e97af-120">Name</span></span>       | <span data-ttu-id="e97af-121">型</span><span class="sxs-lookup"><span data-stu-id="e97af-121">Type</span></span> | <span data-ttu-id="e97af-122">説明</span><span class="sxs-lookup"><span data-stu-id="e97af-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e97af-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e97af-123">Authorization</span></span>  | <span data-ttu-id="e97af-124">string</span><span class="sxs-lookup"><span data-stu-id="e97af-124">string</span></span>  | <span data-ttu-id="e97af-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e97af-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e97af-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e97af-127">Request body</span></span>
<span data-ttu-id="e97af-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e97af-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e97af-129">応答</span><span class="sxs-lookup"><span data-stu-id="e97af-129">Response</span></span>

<span data-ttu-id="e97af-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [application](../resources/application.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e97af-130">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/application.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e97af-131">例</span><span class="sxs-lookup"><span data-stu-id="e97af-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e97af-132">要求</span><span class="sxs-lookup"><span data-stu-id="e97af-132">Request</span></span>
<span data-ttu-id="e97af-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e97af-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "list_application"
}-->
```http
GET https://graph.microsoft.com/beta/applications
```
##### <a name="response"></a><span data-ttu-id="e97af-134">応答</span><span class="sxs-lookup"><span data-stu-id="e97af-134">Response</span></span>
<span data-ttu-id="e97af-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e97af-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1229

{
  "value": [
    {
      "api": {
        "acceptedAccessTokenVersion": 1,
        "publishedPermissionScopes": [
          {
            "adminConsentDescription": "adminConsentDescription-value",
            "adminConsentDisplayName": "adminConsentDisplayName-value",
            "id": "id-value",
            "isEnabled": true,
            "type": "type-value",
            "userConsentDescription": "userConsentDescription-value",
            "userConsentDisplayName": "userConsentDisplayName-value",
            "value": "value-value"
          }
        ]
      },
      "allowPublicClient": true,
      "applicationAliases": [
        "applicationAliases-value"
      ],
      "createdDateTime": "datetime-value",
      "installedClients": {
        "redirectUrls": [
          "redirectUrls-value"
        ]
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List applications",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/application-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
