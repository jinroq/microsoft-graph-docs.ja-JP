---
title: oAuth2Permissiongrant を取得する
description: oAuth2Permissiongrant オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
ms.openlocfilehash: 2b389e7f811444b9dc9fb1d9c2f619006611e11e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32540157"
---
# <a name="get-oauth2permissiongrant"></a><span data-ttu-id="e03ff-103">oAuth2Permissiongrant を取得する</span><span class="sxs-lookup"><span data-stu-id="e03ff-103">Get oAuth2Permissiongrant</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e03ff-104">oAuth2Permissiongrant オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="e03ff-104">Retrieve the properties and relationships of oAuth2Permissiongrant object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e03ff-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e03ff-105">Permissions</span></span>
<span data-ttu-id="e03ff-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e03ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e03ff-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e03ff-108">Permission type</span></span>      | <span data-ttu-id="e03ff-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e03ff-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e03ff-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e03ff-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e03ff-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e03ff-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e03ff-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e03ff-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e03ff-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e03ff-113">Not supported.</span></span>    |
|<span data-ttu-id="e03ff-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e03ff-114">Application</span></span> | <span data-ttu-id="e03ff-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e03ff-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e03ff-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e03ff-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /oAuth2Permissiongrants/{id}
GET /users/{id | userPrincipalName}/oAuth2Permissiongrants/{id}
GET /drive/root/createdByUser/oAuth2Permissiongrants/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e03ff-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e03ff-117">Optional query parameters</span></span>
<span data-ttu-id="e03ff-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e03ff-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e03ff-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e03ff-119">Request headers</span></span>
| <span data-ttu-id="e03ff-120">名前</span><span class="sxs-lookup"><span data-stu-id="e03ff-120">Name</span></span>       | <span data-ttu-id="e03ff-121">型</span><span class="sxs-lookup"><span data-stu-id="e03ff-121">Type</span></span> | <span data-ttu-id="e03ff-122">説明</span><span class="sxs-lookup"><span data-stu-id="e03ff-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e03ff-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e03ff-123">Authorization</span></span>  | <span data-ttu-id="e03ff-124">string</span><span class="sxs-lookup"><span data-stu-id="e03ff-124">string</span></span>  | <span data-ttu-id="e03ff-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e03ff-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e03ff-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e03ff-127">Request body</span></span>
<span data-ttu-id="e03ff-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e03ff-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e03ff-129">応答</span><span class="sxs-lookup"><span data-stu-id="e03ff-129">Response</span></span>

<span data-ttu-id="e03ff-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[oAuth2Permissiongrant](../resources/oauth2permissiongrant.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e03ff-130">If successful, this method returns a `200 OK` response code and [oAuth2Permissiongrant](../resources/oauth2permissiongrant.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e03ff-131">例</span><span class="sxs-lookup"><span data-stu-id="e03ff-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e03ff-132">要求</span><span class="sxs-lookup"><span data-stu-id="e03ff-132">Request</span></span>
<span data-ttu-id="e03ff-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e03ff-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_oAuth2Permissiongrant"
}-->
```http
GET https://graph.microsoft.com/beta/oAuth2Permissiongrants/{id}
```
##### <a name="response"></a><span data-ttu-id="e03ff-134">応答</span><span class="sxs-lookup"><span data-stu-id="e03ff-134">Response</span></span>
<span data-ttu-id="e03ff-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e03ff-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oAuth2Permissiongrant"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 200

{
  "clientId": "clientId-value",
  "consentType": "consentType-value",
  "expiryTime": "2016-10-19T10:37:00Z",
  "id": "id-value",
  "principalId": "principalId-value",
  "resourceId": "resourceId-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get oAuth2Permissiongrant",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/oauth2permissiongrant-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
