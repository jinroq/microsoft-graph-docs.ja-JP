---
title: iosVppEBook の作成
description: 新しい iosVppEBook オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 753e49af6b00124b18b687decbeee195e2e1ee1d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356071"
---
# <a name="create-iosvppebook"></a><span data-ttu-id="de9fe-103">iosVppEBook の作成</span><span class="sxs-lookup"><span data-stu-id="de9fe-103">Create iosVppEBook</span></span>

> <span data-ttu-id="de9fe-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="de9fe-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="de9fe-105">新しい [iosVppEBook](../resources/intune-books-iosvppebook.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="de9fe-105">Create a new [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="de9fe-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="de9fe-106">Prerequisites</span></span>
<span data-ttu-id="de9fe-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="de9fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de9fe-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="de9fe-109">Permission type</span></span>|<span data-ttu-id="de9fe-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="de9fe-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de9fe-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="de9fe-111">Delegated (work or school account)</span></span>|<span data-ttu-id="de9fe-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de9fe-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="de9fe-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="de9fe-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de9fe-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="de9fe-114">Not supported.</span></span>|
|<span data-ttu-id="de9fe-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="de9fe-115">Application</span></span>|<span data-ttu-id="de9fe-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="de9fe-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de9fe-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="de9fe-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="de9fe-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="de9fe-118">Request headers</span></span>
|<span data-ttu-id="de9fe-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="de9fe-119">Header</span></span>|<span data-ttu-id="de9fe-120">値</span><span class="sxs-lookup"><span data-stu-id="de9fe-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de9fe-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="de9fe-121">Authorization</span></span>|<span data-ttu-id="de9fe-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="de9fe-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de9fe-123">Accept</span><span class="sxs-lookup"><span data-stu-id="de9fe-123">Accept</span></span>|<span data-ttu-id="de9fe-124">application/json</span><span class="sxs-lookup"><span data-stu-id="de9fe-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de9fe-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="de9fe-125">Request body</span></span>
<span data-ttu-id="de9fe-126">要求本文で、iosVppEBook オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="de9fe-126">In the request body, supply a JSON representation for the iosVppEBook object.</span></span>

<span data-ttu-id="de9fe-127">次の表に、iosVppEBook の作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="de9fe-127">The following table shows the properties that are required when you create the iosVppEBook.</span></span>

|<span data-ttu-id="de9fe-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="de9fe-128">Property</span></span>|<span data-ttu-id="de9fe-129">種類</span><span class="sxs-lookup"><span data-stu-id="de9fe-129">Type</span></span>|<span data-ttu-id="de9fe-130">説明</span><span class="sxs-lookup"><span data-stu-id="de9fe-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de9fe-131">ID</span><span class="sxs-lookup"><span data-stu-id="de9fe-131">id</span></span>|<span data-ttu-id="de9fe-132">String</span><span class="sxs-lookup"><span data-stu-id="de9fe-132">String</span></span>|<span data-ttu-id="de9fe-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="de9fe-133">Key of the entity.</span></span> <span data-ttu-id="de9fe-134">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="de9fe-134">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="de9fe-135">displayName</span><span class="sxs-lookup"><span data-stu-id="de9fe-135">displayName</span></span>|<span data-ttu-id="de9fe-136">String</span><span class="sxs-lookup"><span data-stu-id="de9fe-136">String</span></span>|<span data-ttu-id="de9fe-137">電子ブックの名前。</span><span class="sxs-lookup"><span data-stu-id="de9fe-137">Name of the eBook.</span></span> <span data-ttu-id="de9fe-138">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="de9fe-138">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="de9fe-139">説明</span><span class="sxs-lookup"><span data-stu-id="de9fe-139">description</span></span>|<span data-ttu-id="de9fe-140">String</span><span class="sxs-lookup"><span data-stu-id="de9fe-140">String</span></span>|<span data-ttu-id="de9fe-141">説明。</span><span class="sxs-lookup"><span data-stu-id="de9fe-141">Description.</span></span> <span data-ttu-id="de9fe-142">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="de9fe-142">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="de9fe-143">publisher</span><span class="sxs-lookup"><span data-stu-id="de9fe-143">publisher</span></span>|<span data-ttu-id="de9fe-144">String</span><span class="sxs-lookup"><span data-stu-id="de9fe-144">String</span></span>|<span data-ttu-id="de9fe-145">発行元です。</span><span class="sxs-lookup"><span data-stu-id="de9fe-145">Publisher.</span></span> <span data-ttu-id="de9fe-146">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="de9fe-146">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="de9fe-147">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="de9fe-147">publishedDateTime</span></span>|<span data-ttu-id="de9fe-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de9fe-148">DateTimeOffset</span></span>|<span data-ttu-id="de9fe-149">電子ブックが発行された日時。</span><span class="sxs-lookup"><span data-stu-id="de9fe-149">The date and time when the eBook was published.</span></span> <span data-ttu-id="de9fe-150">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="de9fe-150">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="de9fe-151">largeCover</span><span class="sxs-lookup"><span data-stu-id="de9fe-151">largeCover</span></span>|[<span data-ttu-id="de9fe-152">mimeContent</span><span class="sxs-lookup"><span data-stu-id="de9fe-152">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="de9fe-153">ブック カバー。</span><span class="sxs-lookup"><span data-stu-id="de9fe-153">Book cover.</span></span> <span data-ttu-id="de9fe-154">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="de9fe-154">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="de9fe-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="de9fe-155">createdDateTime</span></span>|<span data-ttu-id="de9fe-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de9fe-156">DateTimeOffset</span></span>|<span data-ttu-id="de9fe-157">電子ブック ファイルが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="de9fe-157">The date and time when the eBook file was created.</span></span> <span data-ttu-id="de9fe-158">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="de9fe-158">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="de9fe-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="de9fe-159">lastModifiedDateTime</span></span>|<span data-ttu-id="de9fe-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de9fe-160">DateTimeOffset</span></span>|<span data-ttu-id="de9fe-161">電子ブックが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="de9fe-161">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="de9fe-162">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="de9fe-162">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="de9fe-163">informationUrl</span><span class="sxs-lookup"><span data-stu-id="de9fe-163">informationUrl</span></span>|<span data-ttu-id="de9fe-164">String</span><span class="sxs-lookup"><span data-stu-id="de9fe-164">String</span></span>|<span data-ttu-id="de9fe-165">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="de9fe-165">The more information Url.</span></span> <span data-ttu-id="de9fe-166">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="de9fe-166">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="de9fe-167">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="de9fe-167">privacyInformationUrl</span></span>|<span data-ttu-id="de9fe-168">String</span><span class="sxs-lookup"><span data-stu-id="de9fe-168">String</span></span>|<span data-ttu-id="de9fe-169">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="de9fe-169">The privacy statement Url.</span></span> <span data-ttu-id="de9fe-170">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="de9fe-170">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="de9fe-171">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="de9fe-171">vppTokenId</span></span>|<span data-ttu-id="de9fe-172">Guid</span><span class="sxs-lookup"><span data-stu-id="de9fe-172">Guid</span></span>|<span data-ttu-id="de9fe-173">Vpp トークン ID。</span><span class="sxs-lookup"><span data-stu-id="de9fe-173">The Vpp token ID.</span></span>|
|<span data-ttu-id="de9fe-174">appleId</span><span class="sxs-lookup"><span data-stu-id="de9fe-174">appleId</span></span>|<span data-ttu-id="de9fe-175">String</span><span class="sxs-lookup"><span data-stu-id="de9fe-175">String</span></span>|<span data-ttu-id="de9fe-176">Vpp トークンに関連付けられている Apple ID。</span><span class="sxs-lookup"><span data-stu-id="de9fe-176">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="de9fe-177">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="de9fe-177">vppOrganizationName</span></span>|<span data-ttu-id="de9fe-178">String</span><span class="sxs-lookup"><span data-stu-id="de9fe-178">String</span></span>|<span data-ttu-id="de9fe-179">Vpp トークンの組織の名前。</span><span class="sxs-lookup"><span data-stu-id="de9fe-179">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="de9fe-180">genres</span><span class="sxs-lookup"><span data-stu-id="de9fe-180">genres</span></span>|<span data-ttu-id="de9fe-181">String コレクション</span><span class="sxs-lookup"><span data-stu-id="de9fe-181">String collection</span></span>|<span data-ttu-id="de9fe-182">ジャンル。</span><span class="sxs-lookup"><span data-stu-id="de9fe-182">Genres.</span></span>|
|<span data-ttu-id="de9fe-183">language</span><span class="sxs-lookup"><span data-stu-id="de9fe-183">language</span></span>|<span data-ttu-id="de9fe-184">String</span><span class="sxs-lookup"><span data-stu-id="de9fe-184">String</span></span>|<span data-ttu-id="de9fe-185">言語。</span><span class="sxs-lookup"><span data-stu-id="de9fe-185">Language.</span></span>|
|<span data-ttu-id="de9fe-186">seller</span><span class="sxs-lookup"><span data-stu-id="de9fe-186">seller</span></span>|<span data-ttu-id="de9fe-187">String</span><span class="sxs-lookup"><span data-stu-id="de9fe-187">String</span></span>|<span data-ttu-id="de9fe-188">販売元。</span><span class="sxs-lookup"><span data-stu-id="de9fe-188">Seller.</span></span>|
|<span data-ttu-id="de9fe-189">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="de9fe-189">totalLicenseCount</span></span>|<span data-ttu-id="de9fe-190">Int32</span><span class="sxs-lookup"><span data-stu-id="de9fe-190">Int32</span></span>|<span data-ttu-id="de9fe-191">ライセンスの合計数。</span><span class="sxs-lookup"><span data-stu-id="de9fe-191">Total license count.</span></span>|
|<span data-ttu-id="de9fe-192">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="de9fe-192">usedLicenseCount</span></span>|<span data-ttu-id="de9fe-193">Int32</span><span class="sxs-lookup"><span data-stu-id="de9fe-193">Int32</span></span>|<span data-ttu-id="de9fe-194">使用されているライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="de9fe-194">Used license count.</span></span>|



## <a name="response"></a><span data-ttu-id="de9fe-195">応答</span><span class="sxs-lookup"><span data-stu-id="de9fe-195">Response</span></span>
<span data-ttu-id="de9fe-196">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosVppEBook](../resources/intune-books-iosvppebook.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="de9fe-196">If successful, this method returns a `201 Created` response code and a [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de9fe-197">例</span><span class="sxs-lookup"><span data-stu-id="de9fe-197">Example</span></span>
### <a name="request"></a><span data-ttu-id="de9fe-198">要求</span><span class="sxs-lookup"><span data-stu-id="de9fe-198">Request</span></span>
<span data-ttu-id="de9fe-199">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="de9fe-199">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="de9fe-200">応答</span><span class="sxs-lookup"><span data-stu-id="de9fe-200">Response</span></span>
<span data-ttu-id="de9fe-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="de9fe-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



