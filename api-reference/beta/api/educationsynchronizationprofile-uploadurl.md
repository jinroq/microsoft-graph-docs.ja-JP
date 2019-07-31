---
title: 'educationSynchronizationProfile: uploadUrl'
description: テナント内の特定の school データ同期プロファイルについて、ソースファイルを Azure blob ストレージにアップロードするための共有アクセス署名 (SAS) を取得します。 SAS トークンの有効期限は1時間です。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b635ed344870b5e23707dc301f016c9e85f77c18
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954754"
---
# <a name="educationsynchronizationprofile-uploadurl"></a><span data-ttu-id="44c57-104">educationSynchronizationProfile: uploadUrl</span><span class="sxs-lookup"><span data-stu-id="44c57-104">educationSynchronizationProfile: uploadUrl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44c57-105">テナント内の特定の school データ[同期プロファイル](../resources/educationsynchronizationprofile.md)について、ソースファイルを Azure blob ストレージにアップロードするための共有アクセス署名 (SAS) を取得します。</span><span class="sxs-lookup"><span data-stu-id="44c57-105">Retrieve a shared access signature (SAS) for uploading source files to Azure blob storage for a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="44c57-106">SAS トークンの有効期限は1時間です。</span><span class="sxs-lookup"><span data-stu-id="44c57-106">The SAS token has a validity of one hour.</span></span>

<span data-ttu-id="44c57-107">アップロード URL は、 [CSV データプロバイダー](../resources/educationcsvdataprovider.md)に対してのみ提供されます。</span><span class="sxs-lookup"><span data-stu-id="44c57-107">The upload URL is provided only for the [CSV data provider](../resources/educationcsvdataprovider.md).</span></span>

> <span data-ttu-id="44c57-108">**注:** SAS トークンを使用して blob ストレージにアクセスするには、 [Azure ストレージ sdk](https://github.com/search?q=org%3AAzure+azure-storage)または[azcopy](https://docs.microsoft.com/en-us/azure/storage/storage-use-azcopy)を使用します。</span><span class="sxs-lookup"><span data-stu-id="44c57-108">**Note:** To access the blob storage with the SAS token, use the [Azure storage SDKs](https://github.com/search?q=org%3AAzure+azure-storage) or [AzCopy](https://docs.microsoft.com/en-us/azure/storage/storage-use-azcopy).</span></span>

## <a name="permissions"></a><span data-ttu-id="44c57-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="44c57-109">Permissions</span></span>
<span data-ttu-id="44c57-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="44c57-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="44c57-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="44c57-112">Permission type</span></span> | <span data-ttu-id="44c57-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="44c57-113">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="44c57-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="44c57-114">Delegated (work or school account)</span></span> | <span data-ttu-id="44c57-115">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44c57-115">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="44c57-116">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="44c57-116">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="44c57-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="44c57-117">Not supported.</span></span>|
|<span data-ttu-id="44c57-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="44c57-118">Application</span></span>|<span data-ttu-id="44c57-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="44c57-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="44c57-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="44c57-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/uploadUrl
```

## <a name="request-headers"></a><span data-ttu-id="44c57-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="44c57-121">Request headers</span></span>
| <span data-ttu-id="44c57-122">名前</span><span class="sxs-lookup"><span data-stu-id="44c57-122">Name</span></span>       | <span data-ttu-id="44c57-123">型</span><span class="sxs-lookup"><span data-stu-id="44c57-123">Type</span></span> | <span data-ttu-id="44c57-124">説明</span><span class="sxs-lookup"><span data-stu-id="44c57-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="44c57-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="44c57-125">Authorization</span></span>  | <span data-ttu-id="44c57-126">string</span><span class="sxs-lookup"><span data-stu-id="44c57-126">string</span></span>  | <span data-ttu-id="44c57-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="44c57-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="44c57-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="44c57-129">Request body</span></span>
<span data-ttu-id="44c57-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="44c57-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="44c57-131">応答</span><span class="sxs-lookup"><span data-stu-id="44c57-131">Response</span></span>
<span data-ttu-id="44c57-132">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[EDUCATIONSYNCHRONIZATIONPROFILE](../resources/educationsynchronizationprofile.md)の SAS URL を返します。</span><span class="sxs-lookup"><span data-stu-id="44c57-132">If successful, this method returns a `200 OK` response code and a SAS URL for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) in the response body.</span></span>

<span data-ttu-id="44c57-133">以前の要求がまだ処理されている場合、この`409 Conflict`メソッドは、 [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md)に対してアップロードが現在ブロックされていることを示すを返します。</span><span class="sxs-lookup"><span data-stu-id="44c57-133">If a previous request is still being processed, this method returns a `409 Conflict` indicating that the upload is presently blocked for the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md).</span></span>

## <a name="example"></a><span data-ttu-id="44c57-134">例</span><span class="sxs-lookup"><span data-stu-id="44c57-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="44c57-135">要求</span><span class="sxs-lookup"><span data-stu-id="44c57-135">Request</span></span>
<span data-ttu-id="44c57-136">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="44c57-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="44c57-137">プロトコル</span><span class="sxs-lookup"><span data-stu-id="44c57-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_uploadurl"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/uploadUrl
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="44c57-138">C#</span><span class="sxs-lookup"><span data-stu-id="44c57-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsynchronizationprofile-uploadurl-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="44c57-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="44c57-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsynchronizationprofile-uploadurl-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="44c57-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="44c57-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsynchronizationprofile-uploadurl-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="44c57-141">Java</span><span class="sxs-lookup"><span data-stu-id="44c57-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationsynchronizationprofile-uploadurl-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="44c57-142">応答</span><span class="sxs-lookup"><span data-stu-id="44c57-142">Response</span></span>
<span data-ttu-id="44c57-143">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="44c57-143">The following is an example of the response.</span></span> 

><span data-ttu-id="44c57-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="44c57-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
