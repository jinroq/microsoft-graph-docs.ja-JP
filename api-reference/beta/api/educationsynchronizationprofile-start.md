---
title: EducationSynchronizationProfile にファイルをアップロードした後に同期を開始します。
description: テナントで特定の学校のデータの同期プロファイルをファイルのアップロードを確認します。 検証が成功した場合は、プロファイルの同期が開始されます。 それ以外の場合、エラーおよび警告の応答が含まれます。 応答にエラーが含まれている場合、同期は開始されません。 応答には、警告のみが含まれている場合、は、同期が開始されます。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 1447178e80d30058b415345aea83dce4390e6bcf
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512354"
---
# <a name="start-sync-after-uploading-files-to-an-educationsynchronizationprofile"></a><span data-ttu-id="09ed4-107">EducationSynchronizationProfile にファイルをアップロードした後に同期を開始します。</span><span class="sxs-lookup"><span data-stu-id="09ed4-107">Start sync after uploading files to an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09ed4-108">テナント内の特定の学校データ[同期プロファイル](../resources/educationsynchronizationprofile.md)にファイルがアップロードされたことを確認します。</span><span class="sxs-lookup"><span data-stu-id="09ed4-108">Verify the files uploaded to a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="09ed4-109">検証が成功した場合は、プロファイルの同期が開始されます。</span><span class="sxs-lookup"><span data-stu-id="09ed4-109">If the verification is successful, synchronization will start on the profile.</span></span> <span data-ttu-id="09ed4-110">それ以外の場合、エラーおよび警告の応答が含まれます。</span><span class="sxs-lookup"><span data-stu-id="09ed4-110">Otherwise, the response will contain errors and warnings.</span></span> <span data-ttu-id="09ed4-111">応答にエラーが含まれている場合、同期は開始されません。</span><span class="sxs-lookup"><span data-stu-id="09ed4-111">If the response contains errors, the synchronization will not start.</span></span> <span data-ttu-id="09ed4-112">応答には、警告のみが含まれている場合、は、同期が開始されます。</span><span class="sxs-lookup"><span data-stu-id="09ed4-112">If the response contains only warnings, synchronization will start.</span></span>

> <span data-ttu-id="09ed4-113">**注:** データ プロバイダーが型[educationcsvdataprovider](../resources/educationcsvdataprovider.md)の場合にのみ、このメソッドを使用します。</span><span class="sxs-lookup"><span data-stu-id="09ed4-113">**Note:** Use this method only when the data provider is of type [educationcsvdataprovider](../resources/educationcsvdataprovider.md).</span></span> <span data-ttu-id="09ed4-114">また、プロファイルの状態プロパティは、開始する前に準備する必要があります。</span><span class="sxs-lookup"><span data-stu-id="09ed4-114">Also, the profile's state property needs to be provisioned before it can be started.</span></span> <span data-ttu-id="09ed4-115">State プロパティを確認するには、そのプロファイル オブジェクトをポーリングします。</span><span class="sxs-lookup"><span data-stu-id="09ed4-115">Poll the profile object to check its state property.</span></span>

## <a name="permissions"></a><span data-ttu-id="09ed4-116">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="09ed4-116">Permissions</span></span>
<span data-ttu-id="09ed4-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="09ed4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="09ed4-119">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="09ed4-119">Permission type</span></span> | <span data-ttu-id="09ed4-120">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="09ed4-120">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="09ed4-121">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="09ed4-121">Delegated (work or school account)</span></span> | <span data-ttu-id="09ed4-122">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="09ed4-122">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="09ed4-123">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="09ed4-123">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="09ed4-124">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09ed4-124">Not supported.</span></span>|
|<span data-ttu-id="09ed4-125">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="09ed4-125">Application</span></span>|<span data-ttu-id="09ed4-126">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09ed4-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="09ed4-127">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="09ed4-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/start
```

## <a name="request-headers"></a><span data-ttu-id="09ed4-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="09ed4-128">Request headers</span></span>
| <span data-ttu-id="09ed4-129">名前</span><span class="sxs-lookup"><span data-stu-id="09ed4-129">Name</span></span>       | <span data-ttu-id="09ed4-130">型</span><span class="sxs-lookup"><span data-stu-id="09ed4-130">Type</span></span> | <span data-ttu-id="09ed4-131">説明</span><span class="sxs-lookup"><span data-stu-id="09ed4-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="09ed4-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="09ed4-132">Authorization</span></span>  | <span data-ttu-id="09ed4-133">string</span><span class="sxs-lookup"><span data-stu-id="09ed4-133">string</span></span>  | <span data-ttu-id="09ed4-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="09ed4-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="09ed4-136">要求本文</span><span class="sxs-lookup"><span data-stu-id="09ed4-136">Request body</span></span>
<span data-ttu-id="09ed4-137">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="09ed4-137">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="09ed4-138">応答</span><span class="sxs-lookup"><span data-stu-id="09ed4-138">Response</span></span>
<span data-ttu-id="09ed4-139">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="09ed4-139">If successful, this method returns a `200 OK` response code.</span></span> <span data-ttu-id="09ed4-140">失敗した場合、返されます、 `400 Bad Request`。</span><span class="sxs-lookup"><span data-stu-id="09ed4-140">If unsuccessful, it returns a `400 Bad Request`.</span></span> <span data-ttu-id="09ed4-141">応答には、エラーや警告が検出された場合、応答の本体の一部として[educationFileSynchronizationVerificationMessage](../resources/educationfilesynchronizationverificationmessage.md)オブジェクトのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="09ed4-141">The response contains a collection of [educationFileSynchronizationVerificationMessage](../resources/educationfilesynchronizationverificationmessage.md) objects as part of the response body if any errors or warnings were found.</span></span>

## <a name="example"></a><span data-ttu-id="09ed4-142">例</span><span class="sxs-lookup"><span data-stu-id="09ed4-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="09ed4-143">要求</span><span class="sxs-lookup"><span data-stu-id="09ed4-143">Request</span></span>
<span data-ttu-id="09ed4-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="09ed4-144">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_start"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/start
```

##### <a name="response"></a><span data-ttu-id="09ed4-145">応答</span><span class="sxs-lookup"><span data-stu-id="09ed4-145">Response</span></span>
<span data-ttu-id="09ed4-146">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="09ed4-146">Here is an example of the response.</span></span> 

><span data-ttu-id="09ed4-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="09ed4-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationFileSynchronizationVerificationMessage",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2105

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/Collection(microsoft.graph.verificationMessage)",
    "value": [
        {
            "type": "Error",
            "fileName": "section.csv",
            "description": "5 row(s) have missing data for the field - SIS ID"
        },
        {
            "type": "Error",
            "fileName": "section.csv",
            "description": "5 row(s) have an invalid format for the field - SIS ID"
        },
        {
            "type": "Warning",
            "fileName": "student.csv",
            "description": "3 duplicates found in column SIS ID which requires values to be Unique."
        },
        {
            "type": "Warning",
            "fileName": "student.csv",
            "description": "3 duplicates found in column Username which requires values to be Unique."
        },
        {
            "type": "Error",
            "fileName": "studentenrollment.csv",
            "description": "125 row(s) have referenced data not found in source. Field - Section SIS ID"
        },
        {
            "type": "Error",
            "fileName": "studentenrollment.csv",
            "description": "35 row(s) have referenced data not found in source. Field - SIS ID"
        },
        {
            "type": "Warning",
            "fileName": "teacher.csv",
            "description": "3 duplicates found in column SIS ID which requires values to be Unique."
        },
        {
            "type": "Warning",
            "fileName": "teacher.csv",
            "description": "3 duplicates found in column Username which requires values to be Unique."
        },
        {
            "type": "Error",
            "fileName": "teacherroster.csv",
            "description": "10 row(s) have referenced data not found in source. Field - Section SIS ID"
        },
        {
            "type": "Error",
            "fileName": "teacherroster.csv",
            "description": "91 row(s) have referenced data not found in source. Field - SIS ID"
        }
    ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-start.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
