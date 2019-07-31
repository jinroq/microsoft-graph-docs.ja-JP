---
title: EducationSynchronizationProfile を更新する
description: テナント内の既存の school data 同期プロファイルのプロパティを更新します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 9535da9fa454b9a416779e5157200a178b647d37
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954815"
---
# <a name="update-an-educationsynchronizationprofile"></a><span data-ttu-id="50c86-103">EducationSynchronizationProfile を更新する</span><span class="sxs-lookup"><span data-stu-id="50c86-103">Update an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50c86-104">テナント内の既存の school data[同期プロファイル](../resources/educationsynchronizationprofile.md)のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="50c86-104">Update properties for an existing school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="50c86-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="50c86-105">Permissions</span></span>
<span data-ttu-id="50c86-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="50c86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="50c86-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="50c86-108">Permission type</span></span> | <span data-ttu-id="50c86-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="50c86-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="50c86-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="50c86-110">Delegated (work or school account)</span></span> | <span data-ttu-id="50c86-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50c86-111">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="50c86-112">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="50c86-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="50c86-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="50c86-113">Not supported.</span></span>|
|<span data-ttu-id="50c86-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="50c86-114">Application</span></span>|<span data-ttu-id="50c86-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="50c86-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50c86-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="50c86-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /synchronizationProfiles
```

## <a name="request-headers"></a><span data-ttu-id="50c86-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="50c86-117">Request headers</span></span>
| <span data-ttu-id="50c86-118">名前</span><span class="sxs-lookup"><span data-stu-id="50c86-118">Name</span></span>       | <span data-ttu-id="50c86-119">型</span><span class="sxs-lookup"><span data-stu-id="50c86-119">Type</span></span> | <span data-ttu-id="50c86-120">説明</span><span class="sxs-lookup"><span data-stu-id="50c86-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="50c86-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="50c86-121">Authorization</span></span>  | <span data-ttu-id="50c86-122">string</span><span class="sxs-lookup"><span data-stu-id="50c86-122">string</span></span>  | <span data-ttu-id="50c86-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="50c86-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="50c86-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="50c86-125">Content-Type</span></span> | <span data-ttu-id="50c86-126">string</span><span class="sxs-lookup"><span data-stu-id="50c86-126">string</span></span> | <span data-ttu-id="50c86-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="50c86-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="50c86-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="50c86-129">Request body</span></span>
<span data-ttu-id="50c86-130">要求本文で、[同期プロファイル](../resources/educationsynchronizationprofile.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="50c86-130">In the request body, supply a JSON representation of the [synchronizationProfile](../resources/educationsynchronizationprofile.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="50c86-131">応答</span><span class="sxs-lookup"><span data-stu-id="50c86-131">Response</span></span>
<span data-ttu-id="50c86-132">成功した場合、このメソッド`202, Accepted`は応答コードと、応答本文で[同期プロファイル](../resources/educationsynchronizationprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="50c86-132">If successful, this method returns a `202, Accepted` response code and a [synchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50c86-133">例</span><span class="sxs-lookup"><span data-stu-id="50c86-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="50c86-134">要求</span><span class="sxs-lookup"><span data-stu-id="50c86-134">Request</span></span>
<span data-ttu-id="50c86-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="50c86-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "update_synchronizationProfile"
}-->
```http
PUT https://graph.microsoft.com/beta/education/synchronizationProfiles
Content-type: application/json

{
    "displayName": "Test Profile",
    "dataProvider": {
        "@odata.type": "microsoft.graph.educationcsvdataprovider",
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
        "@odata.type": "microsoft.graph.educationidentitycreationconfiguration",
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

##### <a name="response"></a><span data-ttu-id="50c86-136">応答</span><span class="sxs-lookup"><span data-stu-id="50c86-136">Response</span></span>
<span data-ttu-id="50c86-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="50c86-137">Here is an example of the response.</span></span> 

><span data-ttu-id="50c86-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="50c86-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSynchronizationProfile",
} -->
```http
HTTP/1.1 202 Accepted
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
