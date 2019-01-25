---
title: EducationSynchronizationProfile を作成します。
description: 'テナントの新しい学校のデータの同期プロファイルの要求を作成します。 プロファイルの状態を取得する状態を照会します。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: efc9b76405b57d0e47d645d0e7b00dc9425ba71b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520817"
---
# <a name="create-an-educationsynchronizationprofile"></a><span data-ttu-id="7b1c8-104">EducationSynchronizationProfile を作成します。</span><span class="sxs-lookup"><span data-stu-id="7b1c8-104">Create an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b1c8-105">テナントの新しい学校のデータ[の同期プロファイル](../resources/educationsynchronizationprofile.md)の要求を作成します。</span><span class="sxs-lookup"><span data-stu-id="7b1c8-105">Create a request for a new school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="7b1c8-106">プロファイルの状態を取得する[クエリ状態](educationsynchronizationprofilestatus-get.md)にします。</span><span class="sxs-lookup"><span data-stu-id="7b1c8-106">[Query the status](educationsynchronizationprofilestatus-get.md) to get the status of the profile.</span></span> 

## <a name="permissions"></a><span data-ttu-id="7b1c8-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7b1c8-107">Permissions</span></span>
<span data-ttu-id="7b1c8-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7b1c8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7b1c8-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7b1c8-110">Permission type</span></span> | <span data-ttu-id="7b1c8-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7b1c8-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="7b1c8-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7b1c8-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7b1c8-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7b1c8-113">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="7b1c8-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7b1c8-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="7b1c8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7b1c8-115">Not supported.</span></span>|
|<span data-ttu-id="7b1c8-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7b1c8-116">Application</span></span>|<span data-ttu-id="7b1c8-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7b1c8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b1c8-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7b1c8-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles
```

## <a name="request-headers"></a><span data-ttu-id="7b1c8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7b1c8-119">Request headers</span></span>
| <span data-ttu-id="7b1c8-120">名前</span><span class="sxs-lookup"><span data-stu-id="7b1c8-120">Name</span></span>       | <span data-ttu-id="7b1c8-121">型</span><span class="sxs-lookup"><span data-stu-id="7b1c8-121">Type</span></span> | <span data-ttu-id="7b1c8-122">説明</span><span class="sxs-lookup"><span data-stu-id="7b1c8-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7b1c8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7b1c8-123">Authorization</span></span>  | <span data-ttu-id="7b1c8-124">string</span><span class="sxs-lookup"><span data-stu-id="7b1c8-124">string</span></span>  | <span data-ttu-id="7b1c8-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7b1c8-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7b1c8-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7b1c8-127">Content-Type</span></span> | <span data-ttu-id="7b1c8-128">string</span><span class="sxs-lookup"><span data-stu-id="7b1c8-128">string</span></span> | <span data-ttu-id="7b1c8-129">application/json</span><span class="sxs-lookup"><span data-stu-id="7b1c8-129">Application/json.</span></span> <span data-ttu-id="7b1c8-130">必須です。</span><span class="sxs-lookup"><span data-stu-id="7b1c8-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7b1c8-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="7b1c8-131">Request body</span></span>
<span data-ttu-id="7b1c8-132">要求の本文には、 [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="7b1c8-132">In the request body, supply a JSON representation of the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7b1c8-133">応答</span><span class="sxs-lookup"><span data-stu-id="7b1c8-133">Response</span></span>
<span data-ttu-id="7b1c8-134">かどうかは成功すると、このメソッドが返されます、`202, Accepted`応答コードおよび応答の本文内の[educationSynchronizationProfile](../resources/educationsynchronizationprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="7b1c8-134">If successful, this method returns a `202, Accepted` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b1c8-135">例</span><span class="sxs-lookup"><span data-stu-id="7b1c8-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7b1c8-136">要求</span><span class="sxs-lookup"><span data-stu-id="7b1c8-136">Request</span></span>
<span data-ttu-id="7b1c8-137">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7b1c8-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_educationSynchronizationProfile"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles
Content-type: application/json

{
    "displayName": "Test Profile",
    "dataProvider": {
        "@odata.type": "microsoft.graph.educationCsvDataProvider",
        "customizations": {
            "student": {
                "optionalPropertiesToSync": [
                    "State ID",
                    "Middle Name"
                ]
            }
        }
    },
    "identitySynchronizationConfiguration": {
        "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration",
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
            "appliesTo": "teacher",
            "skuIds": [
                "6fd2c87f-b296-42f0-b197-1e91e994b900"
            ]
        },
        {
            "appliesTo": "student",
            "skuIds": [
                "6fd2c87f-b296-42f0-b197-1e91e994b900"
            ]
        }
    ]
}
```

##### <a name="response"></a><span data-ttu-id="7b1c8-138">応答</span><span class="sxs-lookup"><span data-stu-id="7b1c8-138">Response</span></span>
<span data-ttu-id="7b1c8-139">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7b1c8-139">The following is an example of the response.</span></span> 

><span data-ttu-id="7b1c8-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7b1c8-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSynchronizationProfile",
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "displayName": "Test Profile",
    "state": "provisioning",
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
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
