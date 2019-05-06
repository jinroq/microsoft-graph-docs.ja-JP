---
title: 'educationSynchronizationProfile: uploadUrl'
description: テナント内の特定の school データ同期プロファイルについて、ソースファイルを Azure blob ストレージにアップロードするための共有アクセス署名 (SAS) を取得します。 SAS トークンの有効期限は1時間です。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f09e179c8014949be855ef0dc0941cfd374340ee
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33587054"
---
# <a name="educationsynchronizationprofile-uploadurl"></a><span data-ttu-id="33c78-104">educationSynchronizationProfile: uploadUrl</span><span class="sxs-lookup"><span data-stu-id="33c78-104">educationSynchronizationProfile: uploadUrl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33c78-105">テナント内の特定の school データ[同期プロファイル](../resources/educationsynchronizationprofile.md)について、ソースファイルを Azure blob ストレージにアップロードするための共有アクセス署名 (SAS) を取得します。</span><span class="sxs-lookup"><span data-stu-id="33c78-105">Retrieve a shared access signature (SAS) for uploading source files to Azure blob storage for a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="33c78-106">SAS トークンの有効期限は1時間です。</span><span class="sxs-lookup"><span data-stu-id="33c78-106">The SAS token has a validity of one hour.</span></span>

<span data-ttu-id="33c78-107">アップロード URL は、 [CSV データプロバイダー](../resources/educationcsvdataprovider.md)に対してのみ提供されます。</span><span class="sxs-lookup"><span data-stu-id="33c78-107">The upload URL is provided only for the [CSV data provider](../resources/educationcsvdataprovider.md).</span></span>

> <span data-ttu-id="33c78-108">**注:** SAS トークンを使用して blob ストレージにアクセスするには、 [Azure ストレージ sdk](https://github.com/search?q=org%3AAzure+azure-storage)または[azcopy](https://docs.microsoft.com/en-us/azure/storage/storage-use-azcopy)を使用します。</span><span class="sxs-lookup"><span data-stu-id="33c78-108">**Note:** To access the blob storage with the SAS token, use the [Azure storage SDKs](https://github.com/search?q=org%3AAzure+azure-storage) or [AzCopy](https://docs.microsoft.com/en-us/azure/storage/storage-use-azcopy).</span></span>

## <a name="permissions"></a><span data-ttu-id="33c78-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="33c78-109">Permissions</span></span>
<span data-ttu-id="33c78-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="33c78-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="33c78-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="33c78-112">Permission type</span></span> | <span data-ttu-id="33c78-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="33c78-113">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="33c78-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="33c78-114">Delegated (work or school account)</span></span> | <span data-ttu-id="33c78-115">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="33c78-115">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="33c78-116">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="33c78-116">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="33c78-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33c78-117">Not supported.</span></span>|
|<span data-ttu-id="33c78-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="33c78-118">Application</span></span>|<span data-ttu-id="33c78-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33c78-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33c78-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="33c78-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/uploadUrl
```

## <a name="request-headers"></a><span data-ttu-id="33c78-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="33c78-121">Request headers</span></span>
| <span data-ttu-id="33c78-122">名前</span><span class="sxs-lookup"><span data-stu-id="33c78-122">Name</span></span>       | <span data-ttu-id="33c78-123">型</span><span class="sxs-lookup"><span data-stu-id="33c78-123">Type</span></span> | <span data-ttu-id="33c78-124">説明</span><span class="sxs-lookup"><span data-stu-id="33c78-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="33c78-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="33c78-125">Authorization</span></span>  | <span data-ttu-id="33c78-126">string</span><span class="sxs-lookup"><span data-stu-id="33c78-126">string</span></span>  | <span data-ttu-id="33c78-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="33c78-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="33c78-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="33c78-129">Request body</span></span>
<span data-ttu-id="33c78-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="33c78-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="33c78-131">応答</span><span class="sxs-lookup"><span data-stu-id="33c78-131">Response</span></span>
<span data-ttu-id="33c78-132">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[EDUCATIONSYNCHRONIZATIONPROFILE](../resources/educationsynchronizationprofile.md)の SAS URL を返します。</span><span class="sxs-lookup"><span data-stu-id="33c78-132">If successful, this method returns a `200 OK` response code and a SAS URL for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) in the response body.</span></span>

<span data-ttu-id="33c78-133">以前の要求がまだ処理されている場合、この`409 Conflict`メソッドは、 [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md)に対してアップロードが現在ブロックされていることを示すを返します。</span><span class="sxs-lookup"><span data-stu-id="33c78-133">If a previous request is still being processed, this method returns a `409 Conflict` indicating that the upload is presently blocked for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md).</span></span>

## <a name="example"></a><span data-ttu-id="33c78-134">例</span><span class="sxs-lookup"><span data-stu-id="33c78-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="33c78-135">要求</span><span class="sxs-lookup"><span data-stu-id="33c78-135">Request</span></span>
<span data-ttu-id="33c78-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="33c78-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_uploadurl"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/uploadUrl
```

##### <a name="response"></a><span data-ttu-id="33c78-137">応答</span><span class="sxs-lookup"><span data-stu-id="33c78-137">Response</span></span>
<span data-ttu-id="33c78-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="33c78-138">The following is an example of the response.</span></span> 

><span data-ttu-id="33c78-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="33c78-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="33c78-141">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="33c78-141">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="33c78-142">Visual</span><span class="sxs-lookup"><span data-stu-id="33c78-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_educationSynchronizationProfile_uploadurl-Cs-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-uploadurl.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationsynchronizationprofile-uploadurl.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
