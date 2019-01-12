---
title: EducationSynchronizationProfile を作成します。
description: 'テナントの新しい学校のデータの同期プロファイルの要求を作成します。 プロファイルの状態を取得する状態を照会します。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 9d471766a8492e03809d05d6d0366c8e44d59015
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915761"
---
# <a name="create-an-educationsynchronizationprofile"></a><span data-ttu-id="7da68-104">EducationSynchronizationProfile を作成します。</span><span class="sxs-lookup"><span data-stu-id="7da68-104">Create an educationSynchronizationProfile</span></span>

> <span data-ttu-id="7da68-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7da68-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7da68-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7da68-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7da68-107">テナントの新しい学校のデータ[の同期プロファイル](../resources/educationsynchronizationprofile.md)の要求を作成します。</span><span class="sxs-lookup"><span data-stu-id="7da68-107">Create a request for a new school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="7da68-108">プロファイルの状態を取得する[クエリ状態](educationsynchronizationprofilestatus-get.md)にします。</span><span class="sxs-lookup"><span data-stu-id="7da68-108">[Query the status](educationsynchronizationprofilestatus-get.md) to get the status of the profile.</span></span> 

## <a name="permissions"></a><span data-ttu-id="7da68-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="7da68-109">Permissions</span></span>
<span data-ttu-id="7da68-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7da68-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7da68-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7da68-112">Permission type</span></span> | <span data-ttu-id="7da68-113">Permissions</span><span class="sxs-lookup"><span data-stu-id="7da68-113">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="7da68-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7da68-114">Delegated (work or school account)</span></span> | <span data-ttu-id="7da68-115">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7da68-115">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="7da68-116">(個人用の Microsoft アカウントを委任します。</span><span class="sxs-lookup"><span data-stu-id="7da68-116">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="7da68-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7da68-117">Not supported.</span></span>|
|<span data-ttu-id="7da68-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7da68-118">Application</span></span>|<span data-ttu-id="7da68-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7da68-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7da68-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7da68-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles
```

## <a name="request-headers"></a><span data-ttu-id="7da68-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7da68-121">Request headers</span></span>
| <span data-ttu-id="7da68-122">名前</span><span class="sxs-lookup"><span data-stu-id="7da68-122">Name</span></span>       | <span data-ttu-id="7da68-123">種類</span><span class="sxs-lookup"><span data-stu-id="7da68-123">Type</span></span> | <span data-ttu-id="7da68-124">説明</span><span class="sxs-lookup"><span data-stu-id="7da68-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7da68-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7da68-125">Authorization</span></span>  | <span data-ttu-id="7da68-126">string</span><span class="sxs-lookup"><span data-stu-id="7da68-126">string</span></span>  | <span data-ttu-id="7da68-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="7da68-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7da68-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7da68-129">Content-Type</span></span> | <span data-ttu-id="7da68-130">string</span><span class="sxs-lookup"><span data-stu-id="7da68-130">string</span></span> | <span data-ttu-id="7da68-131">アプリケーションまたは json。</span><span class="sxs-lookup"><span data-stu-id="7da68-131">Application/json.</span></span> <span data-ttu-id="7da68-132">必須。</span><span class="sxs-lookup"><span data-stu-id="7da68-132">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7da68-133">要求本文</span><span class="sxs-lookup"><span data-stu-id="7da68-133">Request body</span></span>
<span data-ttu-id="7da68-134">要求の本文には、 [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="7da68-134">In the request body, supply a JSON representation of the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7da68-135">応答</span><span class="sxs-lookup"><span data-stu-id="7da68-135">Response</span></span>
<span data-ttu-id="7da68-136">かどうかは成功すると、このメソッドが返されます、`202, Accepted`応答コードおよび応答の本文内の[educationSynchronizationProfile](../resources/educationsynchronizationprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="7da68-136">If successful, this method returns a `202, Accepted` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7da68-137">例</span><span class="sxs-lookup"><span data-stu-id="7da68-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7da68-138">要求</span><span class="sxs-lookup"><span data-stu-id="7da68-138">Request</span></span>
<span data-ttu-id="7da68-139">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7da68-139">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="7da68-140">応答</span><span class="sxs-lookup"><span data-stu-id="7da68-140">Response</span></span>
<span data-ttu-id="7da68-141">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7da68-141">The following is an example of the response.</span></span> 

><span data-ttu-id="7da68-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="7da68-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "#microsoft.graph.educationSynchronizationProfile",
} -->
```http
HTTP/1.1 201 Created
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
