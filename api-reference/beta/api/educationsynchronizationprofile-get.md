---
title: EducationSynchronizationProfile を取得する
description: 識別子に基づいて、テナント内の学校データ同期プロファイルを取得します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 52d40288237b417138d7ad54a290fc4529f3e10f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954868"
---
# <a name="get-an-educationsynchronizationprofile"></a><span data-ttu-id="44508-103">EducationSynchronizationProfile を取得する</span><span class="sxs-lookup"><span data-stu-id="44508-103">Get an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44508-104">識別子に基づいて、テナント内の学校データ[同期プロファイル](../resources/educationsynchronizationprofile.md)を取得します。</span><span class="sxs-lookup"><span data-stu-id="44508-104">Retrieve a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="44508-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="44508-105">Permissions</span></span>
<span data-ttu-id="44508-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="44508-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="44508-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="44508-108">Permission type</span></span> | <span data-ttu-id="44508-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="44508-109">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="44508-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="44508-110">Delegated (work or school account)</span></span> | <span data-ttu-id="44508-111">EduAdministration、EduAdministration</span><span class="sxs-lookup"><span data-stu-id="44508-111">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="44508-112">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="44508-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="44508-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="44508-113">Not supported.</span></span>|
|<span data-ttu-id="44508-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="44508-114">Application</span></span>| <span data-ttu-id="44508-115">EduAdministration、EduAdministration のいずれかを取得します。</span><span class="sxs-lookup"><span data-stu-id="44508-115">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="44508-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="44508-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="44508-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="44508-117">Request headers</span></span>
| <span data-ttu-id="44508-118">名前</span><span class="sxs-lookup"><span data-stu-id="44508-118">Name</span></span>       | <span data-ttu-id="44508-119">型</span><span class="sxs-lookup"><span data-stu-id="44508-119">Type</span></span> | <span data-ttu-id="44508-120">説明</span><span class="sxs-lookup"><span data-stu-id="44508-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="44508-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="44508-121">Authorization</span></span>  | <span data-ttu-id="44508-122">string</span><span class="sxs-lookup"><span data-stu-id="44508-122">string</span></span>  | <span data-ttu-id="44508-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="44508-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="44508-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="44508-125">Request body</span></span>
<span data-ttu-id="44508-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="44508-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="44508-127">応答</span><span class="sxs-lookup"><span data-stu-id="44508-127">Response</span></span>
<span data-ttu-id="44508-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[educationSynchronizationProfile](../resources/educationsynchronizationprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="44508-128">If successful, this method returns a `200 OK` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44508-129">例</span><span class="sxs-lookup"><span data-stu-id="44508-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="44508-130">要求</span><span class="sxs-lookup"><span data-stu-id="44508-130">Request</span></span>
<span data-ttu-id="44508-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="44508-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationSynchronizationProfile"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```

##### <a name="response"></a><span data-ttu-id="44508-132">応答</span><span class="sxs-lookup"><span data-stu-id="44508-132">Response</span></span>
<span data-ttu-id="44508-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="44508-133">The following is an example of the response.</span></span> 

><span data-ttu-id="44508-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="44508-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
