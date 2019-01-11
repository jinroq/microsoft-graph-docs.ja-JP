---
title: iosVppEBook の作成
description: 新しい iosVppEBook オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1c8946efab803393c349fb011b714b78a075dd69
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815870"
---
# <a name="create-iosvppebook"></a><span data-ttu-id="bed71-103">iosVppEBook の作成</span><span class="sxs-lookup"><span data-stu-id="bed71-103">Create iosVppEBook</span></span>

> <span data-ttu-id="bed71-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bed71-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bed71-105">新しい [iosVppEBook](../resources/intune-books-iosvppebook.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="bed71-105">Create a new [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bed71-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="bed71-106">Prerequisites</span></span>
<span data-ttu-id="bed71-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bed71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bed71-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bed71-109">Permission type</span></span>|<span data-ttu-id="bed71-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bed71-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bed71-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bed71-111">Delegated (work or school account)</span></span>|<span data-ttu-id="bed71-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bed71-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bed71-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bed71-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bed71-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bed71-114">Not supported.</span></span>|
|<span data-ttu-id="bed71-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bed71-115">Application</span></span>|<span data-ttu-id="bed71-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bed71-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bed71-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bed71-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="bed71-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bed71-118">Request headers</span></span>
|<span data-ttu-id="bed71-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bed71-119">Header</span></span>|<span data-ttu-id="bed71-120">値</span><span class="sxs-lookup"><span data-stu-id="bed71-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bed71-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bed71-121">Authorization</span></span>|<span data-ttu-id="bed71-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="bed71-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bed71-123">Accept</span><span class="sxs-lookup"><span data-stu-id="bed71-123">Accept</span></span>|<span data-ttu-id="bed71-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bed71-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bed71-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="bed71-125">Request body</span></span>
<span data-ttu-id="bed71-126">要求本文で、iosVppEBook オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="bed71-126">In the request body, supply a JSON representation for the iosVppEBook object.</span></span>

<span data-ttu-id="bed71-127">次の表に、iosVppEBook の作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="bed71-127">The following table shows the properties that are required when you create the iosVppEBook.</span></span>

|<span data-ttu-id="bed71-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bed71-128">Property</span></span>|<span data-ttu-id="bed71-129">種類</span><span class="sxs-lookup"><span data-stu-id="bed71-129">Type</span></span>|<span data-ttu-id="bed71-130">説明</span><span class="sxs-lookup"><span data-stu-id="bed71-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bed71-131">ID</span><span class="sxs-lookup"><span data-stu-id="bed71-131">id</span></span>|<span data-ttu-id="bed71-132">String</span><span class="sxs-lookup"><span data-stu-id="bed71-132">String</span></span>|<span data-ttu-id="bed71-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="bed71-133">Key of the entity.</span></span> <span data-ttu-id="bed71-134">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bed71-134">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="bed71-135">displayName</span><span class="sxs-lookup"><span data-stu-id="bed71-135">displayName</span></span>|<span data-ttu-id="bed71-136">String</span><span class="sxs-lookup"><span data-stu-id="bed71-136">String</span></span>|<span data-ttu-id="bed71-137">電子ブックの名前。</span><span class="sxs-lookup"><span data-stu-id="bed71-137">Name of the eBook.</span></span> <span data-ttu-id="bed71-138">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bed71-138">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="bed71-139">説明</span><span class="sxs-lookup"><span data-stu-id="bed71-139">description</span></span>|<span data-ttu-id="bed71-140">String</span><span class="sxs-lookup"><span data-stu-id="bed71-140">String</span></span>|<span data-ttu-id="bed71-141">説明。</span><span class="sxs-lookup"><span data-stu-id="bed71-141">Description.</span></span> <span data-ttu-id="bed71-142">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bed71-142">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="bed71-143">publisher</span><span class="sxs-lookup"><span data-stu-id="bed71-143">publisher</span></span>|<span data-ttu-id="bed71-144">String</span><span class="sxs-lookup"><span data-stu-id="bed71-144">String</span></span>|<span data-ttu-id="bed71-145">発行元です。</span><span class="sxs-lookup"><span data-stu-id="bed71-145">Publisher.</span></span> <span data-ttu-id="bed71-146">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bed71-146">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="bed71-147">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="bed71-147">publishedDateTime</span></span>|<span data-ttu-id="bed71-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bed71-148">DateTimeOffset</span></span>|<span data-ttu-id="bed71-149">電子ブックが発行された日時。</span><span class="sxs-lookup"><span data-stu-id="bed71-149">The date and time when the eBook was published.</span></span> <span data-ttu-id="bed71-150">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bed71-150">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="bed71-151">largeCover</span><span class="sxs-lookup"><span data-stu-id="bed71-151">largeCover</span></span>|[<span data-ttu-id="bed71-152">mimeContent</span><span class="sxs-lookup"><span data-stu-id="bed71-152">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="bed71-153">ブック カバー。</span><span class="sxs-lookup"><span data-stu-id="bed71-153">Book cover.</span></span> <span data-ttu-id="bed71-154">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bed71-154">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="bed71-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bed71-155">createdDateTime</span></span>|<span data-ttu-id="bed71-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bed71-156">DateTimeOffset</span></span>|<span data-ttu-id="bed71-157">電子ブック ファイルが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="bed71-157">The date and time when the eBook file was created.</span></span> <span data-ttu-id="bed71-158">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bed71-158">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="bed71-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bed71-159">lastModifiedDateTime</span></span>|<span data-ttu-id="bed71-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bed71-160">DateTimeOffset</span></span>|<span data-ttu-id="bed71-161">電子ブックが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="bed71-161">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="bed71-162">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bed71-162">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="bed71-163">informationUrl</span><span class="sxs-lookup"><span data-stu-id="bed71-163">informationUrl</span></span>|<span data-ttu-id="bed71-164">String</span><span class="sxs-lookup"><span data-stu-id="bed71-164">String</span></span>|<span data-ttu-id="bed71-165">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="bed71-165">The more information Url.</span></span> <span data-ttu-id="bed71-166">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bed71-166">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="bed71-167">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="bed71-167">privacyInformationUrl</span></span>|<span data-ttu-id="bed71-168">String</span><span class="sxs-lookup"><span data-stu-id="bed71-168">String</span></span>|<span data-ttu-id="bed71-169">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="bed71-169">The privacy statement Url.</span></span> <span data-ttu-id="bed71-170">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="bed71-170">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="bed71-171">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="bed71-171">vppTokenId</span></span>|<span data-ttu-id="bed71-172">Guid</span><span class="sxs-lookup"><span data-stu-id="bed71-172">Guid</span></span>|<span data-ttu-id="bed71-173">Vpp トークン ID。</span><span class="sxs-lookup"><span data-stu-id="bed71-173">The Vpp token ID.</span></span>|
|<span data-ttu-id="bed71-174">appleId</span><span class="sxs-lookup"><span data-stu-id="bed71-174">appleId</span></span>|<span data-ttu-id="bed71-175">String</span><span class="sxs-lookup"><span data-stu-id="bed71-175">String</span></span>|<span data-ttu-id="bed71-176">Vpp トークンに関連付けられている Apple ID。</span><span class="sxs-lookup"><span data-stu-id="bed71-176">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="bed71-177">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="bed71-177">vppOrganizationName</span></span>|<span data-ttu-id="bed71-178">String</span><span class="sxs-lookup"><span data-stu-id="bed71-178">String</span></span>|<span data-ttu-id="bed71-179">Vpp トークンの組織の名前。</span><span class="sxs-lookup"><span data-stu-id="bed71-179">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="bed71-180">genres</span><span class="sxs-lookup"><span data-stu-id="bed71-180">genres</span></span>|<span data-ttu-id="bed71-181">String コレクション</span><span class="sxs-lookup"><span data-stu-id="bed71-181">String collection</span></span>|<span data-ttu-id="bed71-182">ジャンル。</span><span class="sxs-lookup"><span data-stu-id="bed71-182">Genres.</span></span>|
|<span data-ttu-id="bed71-183">language</span><span class="sxs-lookup"><span data-stu-id="bed71-183">language</span></span>|<span data-ttu-id="bed71-184">String</span><span class="sxs-lookup"><span data-stu-id="bed71-184">String</span></span>|<span data-ttu-id="bed71-185">言語。</span><span class="sxs-lookup"><span data-stu-id="bed71-185">Language.</span></span>|
|<span data-ttu-id="bed71-186">seller</span><span class="sxs-lookup"><span data-stu-id="bed71-186">seller</span></span>|<span data-ttu-id="bed71-187">String</span><span class="sxs-lookup"><span data-stu-id="bed71-187">String</span></span>|<span data-ttu-id="bed71-188">販売元。</span><span class="sxs-lookup"><span data-stu-id="bed71-188">Seller.</span></span>|
|<span data-ttu-id="bed71-189">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="bed71-189">totalLicenseCount</span></span>|<span data-ttu-id="bed71-190">Int32</span><span class="sxs-lookup"><span data-stu-id="bed71-190">Int32</span></span>|<span data-ttu-id="bed71-191">ライセンスの合計数。</span><span class="sxs-lookup"><span data-stu-id="bed71-191">Total license count.</span></span>|
|<span data-ttu-id="bed71-192">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="bed71-192">usedLicenseCount</span></span>|<span data-ttu-id="bed71-193">Int32</span><span class="sxs-lookup"><span data-stu-id="bed71-193">Int32</span></span>|<span data-ttu-id="bed71-194">使用されているライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="bed71-194">Used license count.</span></span>|



## <a name="response"></a><span data-ttu-id="bed71-195">応答</span><span class="sxs-lookup"><span data-stu-id="bed71-195">Response</span></span>
<span data-ttu-id="bed71-196">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosVppEBook](../resources/intune-books-iosvppebook.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="bed71-196">If successful, this method returns a `201 Created` response code and a [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bed71-197">例</span><span class="sxs-lookup"><span data-stu-id="bed71-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="bed71-198">要求</span><span class="sxs-lookup"><span data-stu-id="bed71-198">Request</span></span>
<span data-ttu-id="bed71-199">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bed71-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks
Content-type: application/json
Content-length: 792

{
  "@odata.type": "#microsoft.graph.iosVppEBook",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "informationUrl": "https://example.com/informationUrl/",
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "vppTokenId": "9148ac60-ac60-9148-60ac-489160ac4891",
  "appleId": "Apple Id value",
  "vppOrganizationName": "Vpp Organization Name value",
  "genres": [
    "Genres value"
  ],
  "language": "Language value",
  "seller": "Seller value",
  "totalLicenseCount": 1,
  "usedLicenseCount": 0
}
```

### <a name="response"></a><span data-ttu-id="bed71-200">応答</span><span class="sxs-lookup"><span data-stu-id="bed71-200">Response</span></span>
<span data-ttu-id="bed71-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bed71-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 964

{
  "@odata.type": "#microsoft.graph.iosVppEBook",
  "id": "3b9f627e-627e-3b9f-7e62-9f3b7e629f3b",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "informationUrl": "https://example.com/informationUrl/",
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "vppTokenId": "9148ac60-ac60-9148-60ac-489160ac4891",
  "appleId": "Apple Id value",
  "vppOrganizationName": "Vpp Organization Name value",
  "genres": [
    "Genres value"
  ],
  "language": "Language value",
  "seller": "Seller value",
  "totalLicenseCount": 1,
  "usedLicenseCount": 0
}
```



