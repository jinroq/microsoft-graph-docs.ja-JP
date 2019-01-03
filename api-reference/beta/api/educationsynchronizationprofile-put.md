---
title: EducationSynchronizationProfile を更新します。
description: テナント内の既存校のデータの同期プロファイルのプロパティを更新します。
author: mmast-msft
ms.openlocfilehash: 17bf46eb4ebd6783f7bafba828ff1bcb7ad5ac48
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361468"
---
# <a name="update-an-educationsynchronizationprofile"></a><span data-ttu-id="eede1-103">EducationSynchronizationProfile を更新します。</span><span class="sxs-lookup"><span data-stu-id="eede1-103">Update an educationSynchronizationProfile</span></span>

> <span data-ttu-id="eede1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="eede1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eede1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eede1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eede1-106">テナント内の既存校のデータ[の同期プロファイル](../resources/educationsynchronizationprofile.md)のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="eede1-106">Update properties for an existing school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="eede1-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="eede1-107">Permissions</span></span>
<span data-ttu-id="eede1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eede1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eede1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="eede1-110">Permission type</span></span> | <span data-ttu-id="eede1-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="eede1-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="eede1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="eede1-112">Delegated (work or school account)</span></span> | <span data-ttu-id="eede1-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="eede1-113">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="eede1-114">(個人用の Microsoft アカウントを委任します。</span><span class="sxs-lookup"><span data-stu-id="eede1-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="eede1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eede1-115">Not supported.</span></span>|
|<span data-ttu-id="eede1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="eede1-116">Application</span></span>|<span data-ttu-id="eede1-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eede1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eede1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="eede1-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /synchronizationProfiles
```

## <a name="request-headers"></a><span data-ttu-id="eede1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eede1-119">Request headers</span></span>
| <span data-ttu-id="eede1-120">名前</span><span class="sxs-lookup"><span data-stu-id="eede1-120">Name</span></span>       | <span data-ttu-id="eede1-121">種類</span><span class="sxs-lookup"><span data-stu-id="eede1-121">Type</span></span> | <span data-ttu-id="eede1-122">説明</span><span class="sxs-lookup"><span data-stu-id="eede1-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="eede1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="eede1-123">Authorization</span></span>  | <span data-ttu-id="eede1-124">string</span><span class="sxs-lookup"><span data-stu-id="eede1-124">string</span></span>  | <span data-ttu-id="eede1-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="eede1-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="eede1-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eede1-127">Content-Type</span></span> | <span data-ttu-id="eede1-128">string</span><span class="sxs-lookup"><span data-stu-id="eede1-128">string</span></span> | <span data-ttu-id="eede1-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="eede1-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eede1-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="eede1-131">Request body</span></span>
<span data-ttu-id="eede1-132">要求の本文には、 [synchronizationProfile](../resources/educationsynchronizationprofile.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="eede1-132">In the request body, supply a JSON representation of the [synchronizationProfile](../resources/educationsynchronizationprofile.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="eede1-133">応答</span><span class="sxs-lookup"><span data-stu-id="eede1-133">Response</span></span>
<span data-ttu-id="eede1-134">かどうかは成功すると、このメソッドが返されます、`202, Accepted`応答コードおよび応答の本文に[synchronizationProfile](../resources/educationsynchronizationprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="eede1-134">If successful, this method returns a `202, Accepted` response code and a [synchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eede1-135">例</span><span class="sxs-lookup"><span data-stu-id="eede1-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eede1-136">要求</span><span class="sxs-lookup"><span data-stu-id="eede1-136">Request</span></span>
<span data-ttu-id="eede1-137">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="eede1-137">Here is an example of the request.</span></span>
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
        "@odata.type": "#microsoft.graph.educationcsvdataprovider",
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
        "@odata.type": "#microsoft.graph.educationidentitycreationconfiguration",
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

##### <a name="response"></a><span data-ttu-id="eede1-138">応答</span><span class="sxs-lookup"><span data-stu-id="eede1-138">Response</span></span>
<span data-ttu-id="eede1-139">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="eede1-139">Here is an example of the response.</span></span> 

><span data-ttu-id="eede1-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="eede1-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "#microsoft.graph.educationSynchronizationProfile",
} -->
```http
HTTP/1.1 202 Accepted
Content-type: application/json

{
    "displayName": "Test Profile",
    "state": "provisioning",
    "id": "86904b1e-c7d0-4ead-b13a-98f11fc400ee",
    "dataProvider": {
        "@odata.type": "#microsoft.graph.educationCsvDataProvider",
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
```