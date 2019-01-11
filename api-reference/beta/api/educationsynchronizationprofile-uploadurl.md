---
title: 'educationSynchronizationProfile: uploadUrl'
description: テナントで特定の学校のデータの同期プロファイルの Azure blob ストレージにソース ファイルをアップロードする共有アクセス署名 (SAS) を取得します。 SAS トークンには、1 時間の有効期限が。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 2f6b10bda218bafbe18698defed138c39a45cc7b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894146"
---
# <a name="educationsynchronizationprofile-uploadurl"></a><span data-ttu-id="f71b3-104">educationSynchronizationProfile: uploadUrl</span><span class="sxs-lookup"><span data-stu-id="f71b3-104">educationSynchronizationProfile: uploadUrl</span></span>

> <span data-ttu-id="f71b3-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f71b3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f71b3-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f71b3-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f71b3-107">テナント内の特定の学校データ[の同期プロファイル](../resources/educationsynchronizationprofile.md)の Azure blob ストレージにソース ファイルをアップロードするには、共有アクセス署名 (SAS) を取得します。</span><span class="sxs-lookup"><span data-stu-id="f71b3-107">Retrieve a shared access signature (SAS) for uploading source files to Azure blob storage for a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="f71b3-108">SAS トークンには、1 時間の有効期限が。</span><span class="sxs-lookup"><span data-stu-id="f71b3-108">The SAS token has a validity of one hour.</span></span>

<span data-ttu-id="f71b3-109">アップロードのみの[CSV データ プロバイダー](../resources/educationcsvdataprovider.md)の URL が用意されています。</span><span class="sxs-lookup"><span data-stu-id="f71b3-109">The upload URL is provided only for the [CSV data provider](../resources/educationcsvdataprovider.md).</span></span>

> <span data-ttu-id="f71b3-110">**注:** SAS のトークンを使用して blob ストレージにアクセスするには、 [Azure ストレージの Sdk](https://github.com/search?q=org%3AAzure+azure-storage)または[AzCopy](https://docs.microsoft.com/en-us/azure/storage/storage-use-azcopy)を使用します。</span><span class="sxs-lookup"><span data-stu-id="f71b3-110">**Note:** To access the blob storage with the SAS token, use the [Azure storage SDKs](https://github.com/search?q=org%3AAzure+azure-storage) or [AzCopy](https://docs.microsoft.com/en-us/azure/storage/storage-use-azcopy).</span></span>

## <a name="permissions"></a><span data-ttu-id="f71b3-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f71b3-111">Permissions</span></span>
<span data-ttu-id="f71b3-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f71b3-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f71b3-114">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f71b3-114">Permission type</span></span> | <span data-ttu-id="f71b3-115">Permissions</span><span class="sxs-lookup"><span data-stu-id="f71b3-115">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="f71b3-116">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f71b3-116">Delegated (work or school account)</span></span> | <span data-ttu-id="f71b3-117">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f71b3-117">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="f71b3-118">(個人用の Microsoft アカウントを委任します。</span><span class="sxs-lookup"><span data-stu-id="f71b3-118">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="f71b3-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f71b3-119">Not supported.</span></span>|
|<span data-ttu-id="f71b3-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f71b3-120">Application</span></span>|<span data-ttu-id="f71b3-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f71b3-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f71b3-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f71b3-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/uploadUrl
```

## <a name="request-headers"></a><span data-ttu-id="f71b3-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f71b3-123">Request headers</span></span>
| <span data-ttu-id="f71b3-124">名前</span><span class="sxs-lookup"><span data-stu-id="f71b3-124">Name</span></span>       | <span data-ttu-id="f71b3-125">種類</span><span class="sxs-lookup"><span data-stu-id="f71b3-125">Type</span></span> | <span data-ttu-id="f71b3-126">説明</span><span class="sxs-lookup"><span data-stu-id="f71b3-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f71b3-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="f71b3-127">Authorization</span></span>  | <span data-ttu-id="f71b3-128">string</span><span class="sxs-lookup"><span data-stu-id="f71b3-128">string</span></span>  | <span data-ttu-id="f71b3-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f71b3-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f71b3-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="f71b3-131">Request body</span></span>
<span data-ttu-id="f71b3-132">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f71b3-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f71b3-133">応答</span><span class="sxs-lookup"><span data-stu-id="f71b3-133">Response</span></span>
<span data-ttu-id="f71b3-134">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[educationSynchronizationProfile](../resources/educationsynchronizationprofile.md)の SA の URL です。</span><span class="sxs-lookup"><span data-stu-id="f71b3-134">If successful, this method returns a `200 OK` response code and a SAS URL for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) in the response body.</span></span>

<span data-ttu-id="f71b3-135">かどうかは前の要求が処理中、このメソッドが返されます、 `409 Conflict` [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md)のアップロードが現在ブロックされていることを示します。</span><span class="sxs-lookup"><span data-stu-id="f71b3-135">If a previous request is still being processed, this method returns a `409 Conflict` indicating that the upload is presently blocked for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md).</span></span>

## <a name="example"></a><span data-ttu-id="f71b3-136">例</span><span class="sxs-lookup"><span data-stu-id="f71b3-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f71b3-137">要求</span><span class="sxs-lookup"><span data-stu-id="f71b3-137">Request</span></span>
<span data-ttu-id="f71b3-138">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f71b3-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_uploadurl"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/uploadUrl
```

##### <a name="response"></a><span data-ttu-id="f71b3-139">応答</span><span class="sxs-lookup"><span data-stu-id="f71b3-139">Response</span></span>
<span data-ttu-id="f71b3-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f71b3-140">The following is an example of the response.</span></span> 

><span data-ttu-id="f71b3-p106">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f71b3-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
