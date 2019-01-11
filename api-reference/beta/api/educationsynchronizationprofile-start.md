---
title: EducationSynchronizationProfile にファイルをアップロードした後に同期を開始します。
description: テナントで特定の学校のデータの同期プロファイルをファイルのアップロードを確認します。 検証が成功した場合は、プロファイルの同期が開始されます。 それ以外の場合、エラーおよび警告の応答が含まれます。 応答にエラーが含まれている場合、同期は開始されません。 応答には、警告のみが含まれている場合、は、同期が開始されます。
localization_priority: Normal
ms.openlocfilehash: 465ab6a807fc6af10067d048459c440c7c567361
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866739"
---
# <a name="start-sync-after-uploading-files-to-an-educationsynchronizationprofile"></a><span data-ttu-id="11d60-107">EducationSynchronizationProfile にファイルをアップロードした後に同期を開始します。</span><span class="sxs-lookup"><span data-stu-id="11d60-107">Start sync after uploading files to an educationSynchronizationProfile</span></span>

> <span data-ttu-id="11d60-108">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="11d60-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="11d60-109">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="11d60-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="11d60-110">テナント内の特定の学校データ[同期プロファイル](../resources/educationsynchronizationprofile.md)にファイルがアップロードされたことを確認します。</span><span class="sxs-lookup"><span data-stu-id="11d60-110">Verify the files uploaded to a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="11d60-111">検証が成功した場合は、プロファイルの同期が開始されます。</span><span class="sxs-lookup"><span data-stu-id="11d60-111">If the verification is successful, synchronization will start on the profile.</span></span> <span data-ttu-id="11d60-112">それ以外の場合、エラーおよび警告の応答が含まれます。</span><span class="sxs-lookup"><span data-stu-id="11d60-112">Otherwise, the response will contain errors and warnings.</span></span> <span data-ttu-id="11d60-113">応答にエラーが含まれている場合、同期は開始されません。</span><span class="sxs-lookup"><span data-stu-id="11d60-113">If the response contains errors, the synchronization will not start.</span></span> <span data-ttu-id="11d60-114">応答には、警告のみが含まれている場合、は、同期が開始されます。</span><span class="sxs-lookup"><span data-stu-id="11d60-114">If the response contains only warnings, synchronization will start.</span></span>

> <span data-ttu-id="11d60-115">**注:** データ プロバイダーが型[educationcsvdataprovider](../resources/educationcsvdataprovider.md)の場合にのみ、このメソッドを使用します。</span><span class="sxs-lookup"><span data-stu-id="11d60-115">**Note:** Use this method only when the data provider is of type [educationcsvdataprovider](../resources/educationcsvdataprovider.md).</span></span> <span data-ttu-id="11d60-116">また、プロファイルの状態プロパティは、開始する前に準備する必要があります。</span><span class="sxs-lookup"><span data-stu-id="11d60-116">Also, the profile's state property needs to be provisioned before it can be started.</span></span> <span data-ttu-id="11d60-117">State プロパティを確認するには、そのプロファイル オブジェクトをポーリングします。</span><span class="sxs-lookup"><span data-stu-id="11d60-117">Poll the profile object to check its state property.</span></span>

## <a name="permissions"></a><span data-ttu-id="11d60-118">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="11d60-118">Permissions</span></span>
<span data-ttu-id="11d60-p105">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="11d60-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="11d60-121">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="11d60-121">Permission type</span></span> | <span data-ttu-id="11d60-122">Permissions</span><span class="sxs-lookup"><span data-stu-id="11d60-122">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="11d60-123">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="11d60-123">Delegated (work or school account)</span></span> | <span data-ttu-id="11d60-124">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="11d60-124">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="11d60-125">(個人用の Microsoft アカウントを委任します。</span><span class="sxs-lookup"><span data-stu-id="11d60-125">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="11d60-126">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="11d60-126">Not supported.</span></span>|
|<span data-ttu-id="11d60-127">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="11d60-127">Application</span></span>|<span data-ttu-id="11d60-128">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="11d60-128">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11d60-129">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="11d60-129">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/start
```

## <a name="request-headers"></a><span data-ttu-id="11d60-130">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="11d60-130">Request headers</span></span>
| <span data-ttu-id="11d60-131">名前</span><span class="sxs-lookup"><span data-stu-id="11d60-131">Name</span></span>       | <span data-ttu-id="11d60-132">種類</span><span class="sxs-lookup"><span data-stu-id="11d60-132">Type</span></span> | <span data-ttu-id="11d60-133">説明</span><span class="sxs-lookup"><span data-stu-id="11d60-133">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="11d60-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="11d60-134">Authorization</span></span>  | <span data-ttu-id="11d60-135">string</span><span class="sxs-lookup"><span data-stu-id="11d60-135">string</span></span>  | <span data-ttu-id="11d60-p106">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="11d60-p106">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="11d60-138">要求本文</span><span class="sxs-lookup"><span data-stu-id="11d60-138">Request body</span></span>
<span data-ttu-id="11d60-139">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="11d60-139">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="11d60-140">応答</span><span class="sxs-lookup"><span data-stu-id="11d60-140">Response</span></span>
<span data-ttu-id="11d60-141">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="11d60-141">If successful, this method returns a `200 OK` response code.</span></span> <span data-ttu-id="11d60-142">失敗した場合、返されます、 `400 Bad Request`。</span><span class="sxs-lookup"><span data-stu-id="11d60-142">If unsuccessful, it returns a `400 Bad Request`.</span></span> <span data-ttu-id="11d60-143">応答には、エラーや警告が検出された場合、応答の本体の一部として[educationFileSynchronizationVerificationMessage](../resources/educationfilesynchronizationverificationmessage.md)オブジェクトのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="11d60-143">The response contains a collection of [educationFileSynchronizationVerificationMessage](../resources/educationfilesynchronizationverificationmessage.md) objects as part of the response body if any errors or warnings were found.</span></span>

## <a name="example"></a><span data-ttu-id="11d60-144">例</span><span class="sxs-lookup"><span data-stu-id="11d60-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="11d60-145">要求</span><span class="sxs-lookup"><span data-stu-id="11d60-145">Request</span></span>
<span data-ttu-id="11d60-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="11d60-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_start"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/start
```

##### <a name="response"></a><span data-ttu-id="11d60-147">応答</span><span class="sxs-lookup"><span data-stu-id="11d60-147">Response</span></span>
<span data-ttu-id="11d60-148">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="11d60-148">Here is an example of the response.</span></span> 

><span data-ttu-id="11d60-p108">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="11d60-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
