---
title: EducationSynchronizationProfile を取得します。
description: 識別子に基づくテナントの学校のデータの同期プロファイルを取得します。
author: mmast-msft
ms.openlocfilehash: 6aa01f8c48bdaad58ae3a6a9c6ba719e91eb23a8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27360852"
---
# <a name="get-an-educationsynchronizationprofile"></a><span data-ttu-id="f488e-103">EducationSynchronizationProfile を取得します。</span><span class="sxs-lookup"><span data-stu-id="f488e-103">Get an educationSynchronizationProfile</span></span>

> <span data-ttu-id="f488e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f488e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f488e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f488e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f488e-106">識別子に基づくテナントの学校のデータ[同期プロファイル](../resources/educationsynchronizationprofile.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="f488e-106">Retrieve a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="f488e-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f488e-107">Permissions</span></span>
<span data-ttu-id="f488e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f488e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f488e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f488e-110">Permission type</span></span> | <span data-ttu-id="f488e-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f488e-111">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="f488e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f488e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f488e-113">EduAdministration.Read、EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f488e-113">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="f488e-114">(個人用の Microsoft アカウントを委任します。</span><span class="sxs-lookup"><span data-stu-id="f488e-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="f488e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f488e-115">Not supported.</span></span>|
|<span data-ttu-id="f488e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f488e-116">Application</span></span>| <span data-ttu-id="f488e-117">EduAdministration.Read.All、EduAdministration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f488e-117">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f488e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f488e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="f488e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f488e-119">Request headers</span></span>
| <span data-ttu-id="f488e-120">名前</span><span class="sxs-lookup"><span data-stu-id="f488e-120">Name</span></span>       | <span data-ttu-id="f488e-121">種類</span><span class="sxs-lookup"><span data-stu-id="f488e-121">Type</span></span> | <span data-ttu-id="f488e-122">説明</span><span class="sxs-lookup"><span data-stu-id="f488e-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f488e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f488e-123">Authorization</span></span>  | <span data-ttu-id="f488e-124">string</span><span class="sxs-lookup"><span data-stu-id="f488e-124">string</span></span>  | <span data-ttu-id="f488e-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f488e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f488e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f488e-127">Request body</span></span>
<span data-ttu-id="f488e-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f488e-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f488e-129">応答</span><span class="sxs-lookup"><span data-stu-id="f488e-129">Response</span></span>
<span data-ttu-id="f488e-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[educationSynchronizationProfile](../resources/educationsynchronizationprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="f488e-130">If successful, this method returns a `200 OK` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f488e-131">例</span><span class="sxs-lookup"><span data-stu-id="f488e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f488e-132">要求</span><span class="sxs-lookup"><span data-stu-id="f488e-132">Request</span></span>
<span data-ttu-id="f488e-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f488e-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationSynchronizationProfile"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```

##### <a name="response"></a><span data-ttu-id="f488e-134">応答</span><span class="sxs-lookup"><span data-stu-id="f488e-134">Response</span></span>
<span data-ttu-id="f488e-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f488e-135">The following is an example of the response.</span></span> 

><span data-ttu-id="f488e-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f488e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "#microsoft.graph.educationSynchronizationProfile",
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
    "licensesToAssign": 
         [
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
