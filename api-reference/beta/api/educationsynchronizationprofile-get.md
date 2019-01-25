---
title: EducationSynchronizationProfile を取得します。
description: 識別子に基づくテナントの学校のデータの同期プロファイルを取得します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 47757956db9e93bb13f4167ef330c7b79d7851b1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530182"
---
# <a name="get-an-educationsynchronizationprofile"></a><span data-ttu-id="50621-103">EducationSynchronizationProfile を取得します。</span><span class="sxs-lookup"><span data-stu-id="50621-103">Get an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50621-104">識別子に基づくテナントの学校のデータ[同期プロファイル](../resources/educationsynchronizationprofile.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="50621-104">Retrieve a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="50621-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="50621-105">Permissions</span></span>
<span data-ttu-id="50621-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="50621-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="50621-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="50621-108">Permission type</span></span> | <span data-ttu-id="50621-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="50621-109">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="50621-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="50621-110">Delegated (work or school account)</span></span> | <span data-ttu-id="50621-111">EduAdministration.Read、EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50621-111">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="50621-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="50621-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="50621-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="50621-113">Not supported.</span></span>|
|<span data-ttu-id="50621-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="50621-114">Application</span></span>| <span data-ttu-id="50621-115">EduAdministration.Read.All、EduAdministration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50621-115">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="50621-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="50621-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="50621-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="50621-117">Request headers</span></span>
| <span data-ttu-id="50621-118">名前</span><span class="sxs-lookup"><span data-stu-id="50621-118">Name</span></span>       | <span data-ttu-id="50621-119">型</span><span class="sxs-lookup"><span data-stu-id="50621-119">Type</span></span> | <span data-ttu-id="50621-120">説明</span><span class="sxs-lookup"><span data-stu-id="50621-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="50621-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="50621-121">Authorization</span></span>  | <span data-ttu-id="50621-122">string</span><span class="sxs-lookup"><span data-stu-id="50621-122">string</span></span>  | <span data-ttu-id="50621-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="50621-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="50621-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="50621-125">Request body</span></span>
<span data-ttu-id="50621-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="50621-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="50621-127">応答</span><span class="sxs-lookup"><span data-stu-id="50621-127">Response</span></span>
<span data-ttu-id="50621-128">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[educationSynchronizationProfile](../resources/educationsynchronizationprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="50621-128">If successful, this method returns a `200 OK` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50621-129">例</span><span class="sxs-lookup"><span data-stu-id="50621-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="50621-130">要求</span><span class="sxs-lookup"><span data-stu-id="50621-130">Request</span></span>
<span data-ttu-id="50621-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="50621-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationSynchronizationProfile"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```

##### <a name="response"></a><span data-ttu-id="50621-132">応答</span><span class="sxs-lookup"><span data-stu-id="50621-132">Response</span></span>
<span data-ttu-id="50621-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="50621-133">The following is an example of the response.</span></span> 

><span data-ttu-id="50621-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="50621-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSynchronizationProfile",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2487

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles/$entity",
    "displayName": "Test Profile",
    "state": "provisioned",
    "id": "86904b1e-c7d0-4ead-b13a-98f11fc400ee",
    "dataProvider": {
        "@odata.type": "microsoft.graph.educationCsvDataProvider",
        "customizations": {
            "student": {
                "optionalPropertiesToSync": [
                    "State ID",
                    "Middle Name"
                ],
                "synchronizationStartDate": "0001-01-01T00:00:00Z",
                "isSyncDeferred": false,
                "allowDisplayNameUpdate": false
            },
            "teacher": {
                "optionalPropertiesToSync": [
                    "State ID",
                    "Teacher Number",
                    "Status",
                    "Middle Name",
                    "Secondary Email",
                    "Title",
                    "Qualification"
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
    "licensesToAssign": 
         [
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
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
