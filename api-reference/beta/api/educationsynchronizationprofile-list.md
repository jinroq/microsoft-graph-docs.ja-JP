---
title: リスト educationSynchronizationProfiles
description: テナント内の学校データ同期プロファイルのコレクションを取得します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 1907b0ef08473a79d66e79fcb4751b281e9a18ad
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457465"
---
# <a name="list-educationsynchronizationprofiles"></a><span data-ttu-id="975d0-103">リスト educationSynchronizationProfiles</span><span class="sxs-lookup"><span data-stu-id="975d0-103">List educationSynchronizationProfiles</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="975d0-104">テナント内の学校データ[同期プロファイル](../resources/educationsynchronizationprofile.md)のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="975d0-104">Retrieve the collection of school data [synchronization profiles](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="975d0-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="975d0-105">Permissions</span></span>
<span data-ttu-id="975d0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="975d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="975d0-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="975d0-108">Permission type</span></span> | <span data-ttu-id="975d0-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="975d0-109">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="975d0-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="975d0-110">Delegated (work or school account)</span></span> | <span data-ttu-id="975d0-111">EduAdministration、EduAdministration</span><span class="sxs-lookup"><span data-stu-id="975d0-111">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="975d0-112">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="975d0-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="975d0-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="975d0-113">Not supported.</span></span>|
|<span data-ttu-id="975d0-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="975d0-114">Application</span></span>|<span data-ttu-id="975d0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="975d0-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="975d0-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="975d0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles
```

## <a name="optional-query-parameters"></a><span data-ttu-id="975d0-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="975d0-117">Optional query parameters</span></span>
<span data-ttu-id="975d0-118">このメソッドは、応答をカスタマイズするために、次の[OData クエリパラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートしています。 $filter、$orderby、$top、$skip、$count。</span><span class="sxs-lookup"><span data-stu-id="975d0-118">This method supports the following [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response: $filter, $orderby, $top, $skip, and $count.</span></span>

## <a name="request-headers"></a><span data-ttu-id="975d0-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="975d0-119">Request headers</span></span>
| <span data-ttu-id="975d0-120">名前</span><span class="sxs-lookup"><span data-stu-id="975d0-120">Name</span></span>       | <span data-ttu-id="975d0-121">型</span><span class="sxs-lookup"><span data-stu-id="975d0-121">Type</span></span> | <span data-ttu-id="975d0-122">説明</span><span class="sxs-lookup"><span data-stu-id="975d0-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="975d0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="975d0-123">Authorization</span></span>  | <span data-ttu-id="975d0-124">string</span><span class="sxs-lookup"><span data-stu-id="975d0-124">string</span></span>  | <span data-ttu-id="975d0-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="975d0-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="975d0-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="975d0-127">Request body</span></span>
<span data-ttu-id="975d0-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="975d0-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="975d0-129">応答</span><span class="sxs-lookup"><span data-stu-id="975d0-129">Response</span></span>
<span data-ttu-id="975d0-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[educationSynchronizationProfile](../resources/educationsynchronizationprofile.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="975d0-130">If successful, this method returns a `200 OK` response code and a collection of [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="975d0-131">例</span><span class="sxs-lookup"><span data-stu-id="975d0-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="975d0-132">要求</span><span class="sxs-lookup"><span data-stu-id="975d0-132">Request</span></span>
<span data-ttu-id="975d0-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="975d0-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "list_synchronizationProfile"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles
```

##### <a name="response"></a><span data-ttu-id="975d0-134">応答</span><span class="sxs-lookup"><span data-stu-id="975d0-134">Response</span></span>
<span data-ttu-id="975d0-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="975d0-135">The following is an example of the response.</span></span> 

><span data-ttu-id="975d0-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="975d0-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSynchronizationProfile",
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
            "@odata.type": "microsoft.graph.educationCsvDataProvider",
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
            "@odata.type": "microsoft.graph.educationIdentityCreationConfiguration",
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
                "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment",                
                "appliesTo": "teacher",
                "skuIds": [
                    "6fd2c87f-b296-42f0-b197-1e91e994b900"
                ]
            },
            {
                "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment",
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
