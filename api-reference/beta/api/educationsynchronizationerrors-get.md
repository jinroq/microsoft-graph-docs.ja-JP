---
title: EducationSynchronizationErrors を取得する
description: '検証中に生成されたエラー、またはテナント内の特定の school データ同期プロファイルの同期中に発生したエラーを取得します。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 49fcbd63aec89c9d1b97c79237a10b934a19ac27
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35441346"
---
# <a name="get-educationsynchronizationerrors"></a><span data-ttu-id="e616f-103">EducationSynchronizationErrors を取得する</span><span class="sxs-lookup"><span data-stu-id="e616f-103">Get educationSynchronizationErrors</span></span>

<span data-ttu-id="e616f-104">検証中に生成されたエラー、またはテナント内の特定の school データ[同期プロファイル](../resources/educationsynchronizationprofile.md)の同期中に発生したエラーを取得します。</span><span class="sxs-lookup"><span data-stu-id="e616f-104">Get the errors generated during validation and/or during a sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> 

## <a name="permissions"></a><span data-ttu-id="e616f-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e616f-105">Permissions</span></span>
<span data-ttu-id="e616f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e616f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e616f-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e616f-108">Permission type</span></span> | <span data-ttu-id="e616f-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e616f-109">Permissions (from least to most privileged)</span></span> |
|:-----------|:------|
| <span data-ttu-id="e616f-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e616f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e616f-111">EduAdministration、EduAdministration</span><span class="sxs-lookup"><span data-stu-id="e616f-111">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="e616f-112">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="e616f-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="e616f-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e616f-113">Not supported.</span></span>|
|<span data-ttu-id="e616f-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e616f-114">Application</span></span>| <span data-ttu-id="e616f-115">EduAdministration、EduAdministration のいずれかを取得します。</span><span class="sxs-lookup"><span data-stu-id="e616f-115">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e616f-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e616f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/errors
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e616f-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e616f-117">Optional query parameters</span></span>
<span data-ttu-id="e616f-118">このメソッドは、応答をカスタマイズするために、次の[OData クエリパラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートしています。 $filter、$orderby、$top、$skip、$count。</span><span class="sxs-lookup"><span data-stu-id="e616f-118">This method supports the following [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response: $filter, $orderby, $top, $skip, and $count.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e616f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e616f-119">Request headers</span></span>
| <span data-ttu-id="e616f-120">名前</span><span class="sxs-lookup"><span data-stu-id="e616f-120">Name</span></span>       | <span data-ttu-id="e616f-121">型</span><span class="sxs-lookup"><span data-stu-id="e616f-121">Type</span></span> | <span data-ttu-id="e616f-122">説明</span><span class="sxs-lookup"><span data-stu-id="e616f-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e616f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e616f-123">Authorization</span></span>  | <span data-ttu-id="e616f-124">string</span><span class="sxs-lookup"><span data-stu-id="e616f-124">string</span></span>  | <span data-ttu-id="e616f-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e616f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e616f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e616f-127">Request body</span></span>
<span data-ttu-id="e616f-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e616f-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e616f-129">応答</span><span class="sxs-lookup"><span data-stu-id="e616f-129">Response</span></span>
<span data-ttu-id="e616f-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[同期エラー](../resources/educationsynchronizationerror.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e616f-130">If successful, this method returns a `200 OK` response code and a collection of [synchronization error](../resources/educationsynchronizationerror.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e616f-131">例</span><span class="sxs-lookup"><span data-stu-id="e616f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e616f-132">要求</span><span class="sxs-lookup"><span data-stu-id="e616f-132">Request</span></span>
<span data-ttu-id="e616f-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e616f-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e616f-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e616f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_error"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/errors
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e616f-135">C#</span><span class="sxs-lookup"><span data-stu-id="e616f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsynchronizationprofile-error-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e616f-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="e616f-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsynchronizationprofile-error-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e616f-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="e616f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsynchronizationprofile-error-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e616f-138">応答</span><span class="sxs-lookup"><span data-stu-id="e616f-138">Response</span></span>
<span data-ttu-id="e616f-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e616f-139">The following is an example of the response.</span></span> 

><span data-ttu-id="e616f-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e616f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.educationSynchronizationError",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1568

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles('{id}')/errors",
    "@odata.count": 14,
    "value": [
        {
            "entryType": "Student",
            "errorCode": "UnsynchronizableChange",
            "errorMessage": "Student cannot be updated as no matching entry in Active Directory was found for Student.  Verify the identity matching criteria for the profile.",
            "joiningValue": "richard.2wilson@testschool.edu",
            "recordedDateTime": "2017-07-05T00:52:45Z",
            "reportableIdentifier": "richard.2wilson"
        },
        {
            "entryType": "Teacher",
            "errorCode": "UnsynchronizableChange",
            "errorMessage": "Teacher cannot be updated as no matching entry in Active Directory was found for Teacher.  Verify the identity matching criteria for the profile.",
            "joiningValue": "alberto2.dorsey@testschool.edu",
            "recordedDateTime": "2017-07-05T00:52:57Z",
            "reportableIdentifier": "alberto2.dorsey"
        },
        {
            "entryType": "Teacher",
            "errorCode": "UnsynchronizableChange",
            "errorMessage": "Teacher cannot be updated as no matching entry in Active Directory was found for Teacher.  Verify the identity matching criteria for the profile.",
            "joiningValue": "madeline2.bullock@testschool.edu",
            "recordedDateTime": "2017-07-05T00:52:57Z",
            "reportableIdentifier": "madeline2.bullock"
        }
    ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
