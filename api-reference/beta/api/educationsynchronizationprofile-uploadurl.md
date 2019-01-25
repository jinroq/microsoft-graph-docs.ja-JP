---
title: 'educationSynchronizationProfile: uploadUrl'
description: テナントで特定の学校のデータの同期プロファイルの Azure blob ストレージにソース ファイルをアップロードする共有アクセス署名 (SAS) を取得します。 SAS トークンには、1 時間の有効期限が。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 74f37f5653147691c408cf83e3039920957352c7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511598"
---
# <a name="educationsynchronizationprofile-uploadurl"></a><span data-ttu-id="ce7ff-104">educationSynchronizationProfile: uploadUrl</span><span class="sxs-lookup"><span data-stu-id="ce7ff-104">educationSynchronizationProfile: uploadUrl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce7ff-105">テナント内の特定の学校データ[の同期プロファイル](../resources/educationsynchronizationprofile.md)の Azure blob ストレージにソース ファイルをアップロードするには、共有アクセス署名 (SAS) を取得します。</span><span class="sxs-lookup"><span data-stu-id="ce7ff-105">Retrieve a shared access signature (SAS) for uploading source files to Azure blob storage for a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="ce7ff-106">SAS トークンには、1 時間の有効期限が。</span><span class="sxs-lookup"><span data-stu-id="ce7ff-106">The SAS token has a validity of one hour.</span></span>

<span data-ttu-id="ce7ff-107">アップロードのみの[CSV データ プロバイダー](../resources/educationcsvdataprovider.md)の URL が用意されています。</span><span class="sxs-lookup"><span data-stu-id="ce7ff-107">The upload URL is provided only for the [CSV data provider](../resources/educationcsvdataprovider.md).</span></span>

> <span data-ttu-id="ce7ff-108">**注:** SAS のトークンを使用して blob ストレージにアクセスするには、 [Azure ストレージの Sdk](https://github.com/search?q=org%3AAzure+azure-storage)または[AzCopy](https://docs.microsoft.com/en-us/azure/storage/storage-use-azcopy)を使用します。</span><span class="sxs-lookup"><span data-stu-id="ce7ff-108">**Note:** To access the blob storage with the SAS token, use the [Azure storage SDKs](https://github.com/search?q=org%3AAzure+azure-storage) or [AzCopy](https://docs.microsoft.com/en-us/azure/storage/storage-use-azcopy).</span></span>

## <a name="permissions"></a><span data-ttu-id="ce7ff-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ce7ff-109">Permissions</span></span>
<span data-ttu-id="ce7ff-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ce7ff-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ce7ff-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ce7ff-112">Permission type</span></span> | <span data-ttu-id="ce7ff-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ce7ff-113">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="ce7ff-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ce7ff-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ce7ff-115">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ce7ff-115">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="ce7ff-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ce7ff-116">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="ce7ff-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce7ff-117">Not supported.</span></span>|
|<span data-ttu-id="ce7ff-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ce7ff-118">Application</span></span>|<span data-ttu-id="ce7ff-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce7ff-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce7ff-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ce7ff-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/uploadUrl
```

## <a name="request-headers"></a><span data-ttu-id="ce7ff-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ce7ff-121">Request headers</span></span>
| <span data-ttu-id="ce7ff-122">名前</span><span class="sxs-lookup"><span data-stu-id="ce7ff-122">Name</span></span>       | <span data-ttu-id="ce7ff-123">型</span><span class="sxs-lookup"><span data-stu-id="ce7ff-123">Type</span></span> | <span data-ttu-id="ce7ff-124">説明</span><span class="sxs-lookup"><span data-stu-id="ce7ff-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ce7ff-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce7ff-125">Authorization</span></span>  | <span data-ttu-id="ce7ff-126">string</span><span class="sxs-lookup"><span data-stu-id="ce7ff-126">string</span></span>  | <span data-ttu-id="ce7ff-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ce7ff-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ce7ff-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="ce7ff-129">Request body</span></span>
<span data-ttu-id="ce7ff-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ce7ff-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="ce7ff-131">応答</span><span class="sxs-lookup"><span data-stu-id="ce7ff-131">Response</span></span>
<span data-ttu-id="ce7ff-132">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[educationSynchronizationProfile](../resources/educationsynchronizationprofile.md)の SA の URL です。</span><span class="sxs-lookup"><span data-stu-id="ce7ff-132">If successful, this method returns a `200 OK` response code and a SAS URL for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) in the response body.</span></span>

<span data-ttu-id="ce7ff-133">かどうかは前の要求が処理中、このメソッドが返されます、 `409 Conflict` [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md)のアップロードが現在ブロックされていることを示します。</span><span class="sxs-lookup"><span data-stu-id="ce7ff-133">If a previous request is still being processed, this method returns a `409 Conflict` indicating that the upload is presently blocked for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md).</span></span>

## <a name="example"></a><span data-ttu-id="ce7ff-134">例</span><span class="sxs-lookup"><span data-stu-id="ce7ff-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ce7ff-135">要求</span><span class="sxs-lookup"><span data-stu-id="ce7ff-135">Request</span></span>
<span data-ttu-id="ce7ff-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ce7ff-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_uploadurl"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/uploadUrl
```

##### <a name="response"></a><span data-ttu-id="ce7ff-137">応答</span><span class="sxs-lookup"><span data-stu-id="ce7ff-137">Response</span></span>
<span data-ttu-id="ce7ff-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ce7ff-138">The following is an example of the response.</span></span> 

><span data-ttu-id="ce7ff-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ce7ff-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "String",
} -->
```http
HTTP/1.1 201 OK
Content-type: application/json
Content-length: 314

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#String",
    "value": "https://sdsstorage.blob.core.windows.net/86904b1e-c7d0-4ead-b13a-98f11fc400ee?sv=2015-07-08&sr=c&si=SharedAccessPolicy_20170704044441&sig=CH65vxxqXETCkQNH0Lfsu31cUo0s0XcEEo0OE2YiL6Q%3D&se=2017-07-04T08%3A43%3A01Z&sp=w"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-uploadurl.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
