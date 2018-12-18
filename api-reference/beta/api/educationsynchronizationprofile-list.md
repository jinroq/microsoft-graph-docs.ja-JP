---
title: リスト educationSynchronizationProfiles
description: テナントの学校のデータの同期プロファイルのコレクションを取得します。
author: mmast-msft
ms.openlocfilehash: d7ee2b643259eec6c9106ab6ff89245ab79a3044
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303102"
---
# <a name="list-educationsynchronizationprofiles"></a><span data-ttu-id="8dd2f-103">リスト educationSynchronizationProfiles</span><span class="sxs-lookup"><span data-stu-id="8dd2f-103">List educationSynchronizationProfiles</span></span>

> <span data-ttu-id="8dd2f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8dd2f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8dd2f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8dd2f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8dd2f-106">テナントの学校のデータ[の同期プロファイル](../resources/educationsynchronizationprofile.md)のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="8dd2f-106">Retrieve the collection of school data [synchronization profiles](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="8dd2f-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8dd2f-107">Permissions</span></span>
<span data-ttu-id="8dd2f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8dd2f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8dd2f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8dd2f-110">Permission type</span></span> | <span data-ttu-id="8dd2f-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8dd2f-111">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="8dd2f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8dd2f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8dd2f-113">EduAdministration.Read、EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8dd2f-113">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="8dd2f-114">(個人用の Microsoft アカウントを委任します。</span><span class="sxs-lookup"><span data-stu-id="8dd2f-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="8dd2f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8dd2f-115">Not supported.</span></span>|
|<span data-ttu-id="8dd2f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8dd2f-116">Application</span></span>|<span data-ttu-id="8dd2f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8dd2f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8dd2f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8dd2f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8dd2f-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8dd2f-119">Optional query parameters</span></span>
<span data-ttu-id="8dd2f-120">このメソッドは、応答をカスタマイズするために次の[OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートしています: $filter、$orderby、$top、$skip、および $count。</span><span class="sxs-lookup"><span data-stu-id="8dd2f-120">This method supports the following [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response: $filter, $orderby, $top, $skip, and $count.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8dd2f-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8dd2f-121">Request headers</span></span>
| <span data-ttu-id="8dd2f-122">名前</span><span class="sxs-lookup"><span data-stu-id="8dd2f-122">Name</span></span>       | <span data-ttu-id="8dd2f-123">種類</span><span class="sxs-lookup"><span data-stu-id="8dd2f-123">Type</span></span> | <span data-ttu-id="8dd2f-124">説明</span><span class="sxs-lookup"><span data-stu-id="8dd2f-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8dd2f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8dd2f-125">Authorization</span></span>  | <span data-ttu-id="8dd2f-126">string</span><span class="sxs-lookup"><span data-stu-id="8dd2f-126">string</span></span>  | <span data-ttu-id="8dd2f-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="8dd2f-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8dd2f-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="8dd2f-129">Request body</span></span>
<span data-ttu-id="8dd2f-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8dd2f-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8dd2f-131">応答</span><span class="sxs-lookup"><span data-stu-id="8dd2f-131">Response</span></span>
<span data-ttu-id="8dd2f-132">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[educationSynchronizationProfile](../resources/educationsynchronizationprofile.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="8dd2f-132">If successful, this method returns a `200 OK` response code and a collection of [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8dd2f-133">例</span><span class="sxs-lookup"><span data-stu-id="8dd2f-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8dd2f-134">要求</span><span class="sxs-lookup"><span data-stu-id="8dd2f-134">Request</span></span>
<span data-ttu-id="8dd2f-135">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8dd2f-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "list_synchronizationProfile"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles
```

##### <a name="response"></a><span data-ttu-id="8dd2f-136">応答</span><span class="sxs-lookup"><span data-stu-id="8dd2f-136">Response</span></span>
<span data-ttu-id="8dd2f-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8dd2f-137">The following is an example of the response.</span></span> 

><span data-ttu-id="8dd2f-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="8dd2f-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "#microsoft.graph.educationSynchronizationProfile",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 3296

{
    "value": [
    {
        "displayName": "Test Profile",
        "state": "provisioned",
        "id": "15e9b9fa-de85-492e-aa44-550c40de626e",
        "dataProvider": {
            "@odata.type": "#microsoft.graph.educationCsvDataProvider",
            "customizations": {
                "school": {
                    "optionalPropertiesToSync": [
                        "School NCES_ID",
                        "State ID",
                        "GradeLow",
                        "GradeHigh",
                        "Principal Name"
                    ],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                },
                "section": {
                    "optionalPropertiesToSync": [],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                },
                "student": {
                    "optionalPropertiesToSync": [
                        "State ID",
                        "Email",
                        "Middle Name"
                    ],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                },
                "teacher": {
                    "optionalPropertiesToSync": [
                        "Teacher Number",
                        "Middle Name"
                    ],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                },
                "studentEnrollment": {
                    "optionalPropertiesToSync": [],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                },
                "teacherRoster": {
                    "optionalPropertiesToSync": [],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                }
            }
        },
        "identitySynchronizationConfiguration": {
            "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration",
            "userDomains": [
                {
                    "appliesTo": "student",
                    "name": "testschool.edu"
                },
                {
                    "appliesTo": "teacher",
                    "name": "testschool.edu"
                }
            ]
        },
        "licensesToAssign": [
            {
                "@odata.type": "#microsoft.graph.educationSynchronizationLicenseAssignment",                
                "appliesTo": "teacher",
                "skuIds": [
                    "6fd2c87f-b296-42f0-b197-1e91e994b900"
                ]
            },
            {
                "@odata.type": "#microsoft.graph.educationSynchronizationLicenseAssignment",
                "appliesTo": "student",
                "skuIds": [
                    "6fd2c87f-b296-42f0-b197-1e91e994b900"
                ]
            }
        ]
    }
  ]
}
```