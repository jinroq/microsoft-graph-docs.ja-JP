---
title: ファイルを educationSynchronizationProfile にアップロードした後、同期を開始する
description: テナント内の特定の school データ同期プロファイルにアップロードされたファイルを確認します。 検証に成功すると、プロファイルの同期が開始されます。 それ以外の場合、応答にはエラーと警告が含まれます。 応答にエラーが含まれている場合、同期は開始されません。 応答に警告のみが含まれている場合は、同期が開始されます。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b0f738f7e122126df2ce3611866e75eb5697b160
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954768"
---
# <a name="start-sync-after-uploading-files-to-an-educationsynchronizationprofile"></a><span data-ttu-id="e4aeb-107">ファイルを educationSynchronizationProfile にアップロードした後、同期を開始する</span><span class="sxs-lookup"><span data-stu-id="e4aeb-107">Start sync after uploading files to an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4aeb-108">テナント内の特定の school データ[同期プロファイル](../resources/educationsynchronizationprofile.md)にアップロードされたファイルを確認します。</span><span class="sxs-lookup"><span data-stu-id="e4aeb-108">Verify the files uploaded to a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="e4aeb-109">検証に成功すると、プロファイルの同期が開始されます。</span><span class="sxs-lookup"><span data-stu-id="e4aeb-109">If the verification is successful, synchronization will start on the profile.</span></span> <span data-ttu-id="e4aeb-110">それ以外の場合、応答にはエラーと警告が含まれます。</span><span class="sxs-lookup"><span data-stu-id="e4aeb-110">Otherwise, the response will contain errors and warnings.</span></span> <span data-ttu-id="e4aeb-111">応答にエラーが含まれている場合、同期は開始されません。</span><span class="sxs-lookup"><span data-stu-id="e4aeb-111">If the response contains errors, the synchronization will not start.</span></span> <span data-ttu-id="e4aeb-112">応答に警告のみが含まれている場合は、同期が開始されます。</span><span class="sxs-lookup"><span data-stu-id="e4aeb-112">If the response contains only warnings, synchronization will start.</span></span>

> <span data-ttu-id="e4aeb-113">**注:** このメソッドは、データプロバイダーの種類が[educationcsvdataprovider](../resources/educationcsvdataprovider.md)の場合にのみ使用します。</span><span class="sxs-lookup"><span data-stu-id="e4aeb-113">**Note:** Use this method only when the data provider is of type [educationcsvdataprovider](../resources/educationcsvdataprovider.md).</span></span> <span data-ttu-id="e4aeb-114">また、プロファイルの state プロパティを開始するには、事前に準備しておく必要があります。</span><span class="sxs-lookup"><span data-stu-id="e4aeb-114">Also, the profile's state property needs to be provisioned before it can be started.</span></span> <span data-ttu-id="e4aeb-115">プロファイルオブジェクトをポーリングして、その state プロパティを確認します。</span><span class="sxs-lookup"><span data-stu-id="e4aeb-115">Poll the profile object to check its state property.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4aeb-116">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e4aeb-116">Permissions</span></span>
<span data-ttu-id="e4aeb-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e4aeb-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e4aeb-119">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e4aeb-119">Permission type</span></span> | <span data-ttu-id="e4aeb-120">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e4aeb-120">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="e4aeb-121">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e4aeb-121">Delegated (work or school account)</span></span> | <span data-ttu-id="e4aeb-122">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4aeb-122">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="e4aeb-123">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="e4aeb-123">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="e4aeb-124">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e4aeb-124">Not supported.</span></span>|
|<span data-ttu-id="e4aeb-125">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e4aeb-125">Application</span></span>|<span data-ttu-id="e4aeb-126">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e4aeb-126">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4aeb-127">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e4aeb-127">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/start
```

## <a name="request-headers"></a><span data-ttu-id="e4aeb-128">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e4aeb-128">Request headers</span></span>
| <span data-ttu-id="e4aeb-129">名前</span><span class="sxs-lookup"><span data-stu-id="e4aeb-129">Name</span></span>       | <span data-ttu-id="e4aeb-130">型</span><span class="sxs-lookup"><span data-stu-id="e4aeb-130">Type</span></span> | <span data-ttu-id="e4aeb-131">説明</span><span class="sxs-lookup"><span data-stu-id="e4aeb-131">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e4aeb-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4aeb-132">Authorization</span></span>  | <span data-ttu-id="e4aeb-133">string</span><span class="sxs-lookup"><span data-stu-id="e4aeb-133">string</span></span>  | <span data-ttu-id="e4aeb-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e4aeb-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e4aeb-136">要求本文</span><span class="sxs-lookup"><span data-stu-id="e4aeb-136">Request body</span></span>
<span data-ttu-id="e4aeb-137">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e4aeb-137">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="e4aeb-138">応答</span><span class="sxs-lookup"><span data-stu-id="e4aeb-138">Response</span></span>
<span data-ttu-id="e4aeb-139">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="e4aeb-139">If successful, this method returns a `200 OK` response code.</span></span> <span data-ttu-id="e4aeb-140">失敗した場合は、 `400 Bad Request`を返します。</span><span class="sxs-lookup"><span data-stu-id="e4aeb-140">If unsuccessful, it returns a `400 Bad Request`.</span></span> <span data-ttu-id="e4aeb-141">応答には、 [educationFileSynchronizationVerificationMessage](../resources/educationfilesynchronizationverificationmessage.md)オブジェクトのコレクションが応答本文の一部として含まれています (エラーまたは警告が検出された場合)。</span><span class="sxs-lookup"><span data-stu-id="e4aeb-141">The response contains a collection of [educationFileSynchronizationVerificationMessage](../resources/educationfilesynchronizationverificationmessage.md) objects as part of the response body if any errors or warnings were found.</span></span>

## <a name="example"></a><span data-ttu-id="e4aeb-142">例</span><span class="sxs-lookup"><span data-stu-id="e4aeb-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e4aeb-143">要求</span><span class="sxs-lookup"><span data-stu-id="e4aeb-143">Request</span></span>
<span data-ttu-id="e4aeb-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e4aeb-144">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e4aeb-145">プロトコル</span><span class="sxs-lookup"><span data-stu-id="e4aeb-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_educationSynchronizationProfile_start"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/start
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e4aeb-146">C#</span><span class="sxs-lookup"><span data-stu-id="e4aeb-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-educationsynchronizationprofile-start-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e4aeb-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="e4aeb-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-educationsynchronizationprofile-start-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e4aeb-148">目的-C</span><span class="sxs-lookup"><span data-stu-id="e4aeb-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-educationsynchronizationprofile-start-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e4aeb-149">Java</span><span class="sxs-lookup"><span data-stu-id="e4aeb-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-educationsynchronizationprofile-start-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e4aeb-150">応答</span><span class="sxs-lookup"><span data-stu-id="e4aeb-150">Response</span></span>
<span data-ttu-id="e4aeb-151">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="e4aeb-151">Here is an example of the response.</span></span> 

><span data-ttu-id="e4aeb-p107">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="e4aeb-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
