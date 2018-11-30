---
title: EducationSynchronizationErrors を取得します。
description: '検証中に、テナントの特定の学校のデータの同期プロファイルの同期中に発生したエラーを取得します。 '
ms.openlocfilehash: 5853834187dcf470dff093a21589b3eba798e793
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069883"
---
# <a name="get-educationsynchronizationerrors"></a><span data-ttu-id="26830-103">EducationSynchronizationErrors を取得します。</span><span class="sxs-lookup"><span data-stu-id="26830-103">Get educationSynchronizationErrors</span></span>

<span data-ttu-id="26830-104">検証中に、テナント内の特定の学校データ[の同期プロファイル](../resources/educationsynchronizationprofile.md)の同期中に発生したエラーを取得します。</span><span class="sxs-lookup"><span data-stu-id="26830-104">Get the errors generated during validation and/or during a sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> 

## <a name="permissions"></a><span data-ttu-id="26830-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="26830-105">Permissions</span></span>
<span data-ttu-id="26830-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="26830-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="26830-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="26830-108">Permission type</span></span> | <span data-ttu-id="26830-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="26830-109">Permissions (from least to most privileged)</span></span> |
|:-----------|:------|
| <span data-ttu-id="26830-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="26830-110">Delegated (work or school account)</span></span> | <span data-ttu-id="26830-111">EduAdministration.Read、EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="26830-111">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="26830-112">(個人用の Microsoft アカウントを委任します。</span><span class="sxs-lookup"><span data-stu-id="26830-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="26830-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="26830-113">Not supported.</span></span>|
|<span data-ttu-id="26830-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="26830-114">Application</span></span>| <span data-ttu-id="26830-115">EduAdministration.Read.All、EduAdministration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26830-115">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="26830-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="26830-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/errors
```
## <a name="optional-query-parameters"></a><span data-ttu-id="26830-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="26830-117">Optional query parameters</span></span>
<span data-ttu-id="26830-118">このメソッドは、応答をカスタマイズするために次の[OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートしています: $filter、$orderby、$top、$skip、および $count。</span><span class="sxs-lookup"><span data-stu-id="26830-118">This method supports the following [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response: $filter, $orderby, $top, $skip, and $count.</span></span>

## <a name="request-headers"></a><span data-ttu-id="26830-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="26830-119">Request headers</span></span>
| <span data-ttu-id="26830-120">名前</span><span class="sxs-lookup"><span data-stu-id="26830-120">Name</span></span>       | <span data-ttu-id="26830-121">型</span><span class="sxs-lookup"><span data-stu-id="26830-121">Type</span></span> | <span data-ttu-id="26830-122">説明</span><span class="sxs-lookup"><span data-stu-id="26830-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="26830-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="26830-123">Authorization</span></span>  | <span data-ttu-id="26830-124">string</span><span class="sxs-lookup"><span data-stu-id="26830-124">string</span></span>  | <span data-ttu-id="26830-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="26830-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="26830-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="26830-127">Request body</span></span>
<span data-ttu-id="26830-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="26830-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="26830-129">応答</span><span class="sxs-lookup"><span data-stu-id="26830-129">Response</span></span>
<span data-ttu-id="26830-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の[同期エラー](../resources/educationsynchronizationerror.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="26830-130">If successful, this method returns a `200 OK` response code and a collection of [synchronization error](../resources/educationsynchronizationerror.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26830-131">例</span><span class="sxs-lookup"><span data-stu-id="26830-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="26830-132">要求</span><span class="sxs-lookup"><span data-stu-id="26830-132">Request</span></span>
<span data-ttu-id="26830-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="26830-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_error"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/error
```

##### <a name="response"></a><span data-ttu-id="26830-134">応答</span><span class="sxs-lookup"><span data-stu-id="26830-134">Response</span></span>
<span data-ttu-id="26830-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="26830-135">The following is an example of the response.</span></span> 

><span data-ttu-id="26830-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="26830-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "#microsoft.graph.educationSynchronizationError",
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
