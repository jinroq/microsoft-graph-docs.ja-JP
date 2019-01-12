---
title: iosVppEBook の作成
description: 新しい iosVppEBook オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 96fb518c3ecc9434aaa1c0bd4da1cf18271a8a57
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930006"
---
# <a name="create-iosvppebook"></a><span data-ttu-id="20678-103">iosVppEBook の作成</span><span class="sxs-lookup"><span data-stu-id="20678-103">Create iosVppEBook</span></span>

> <span data-ttu-id="20678-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="20678-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="20678-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="20678-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="20678-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="20678-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="20678-107">新しい [iosVppEBook](../resources/intune-books-iosvppebook.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="20678-107">Create a new [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="20678-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="20678-108">Prerequisites</span></span>
<span data-ttu-id="20678-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="20678-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20678-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="20678-111">Permission type</span></span>|<span data-ttu-id="20678-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="20678-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20678-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="20678-113">Delegated (work or school account)</span></span>|<span data-ttu-id="20678-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20678-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="20678-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="20678-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20678-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="20678-116">Not supported.</span></span>|
|<span data-ttu-id="20678-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="20678-117">Application</span></span>|<span data-ttu-id="20678-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="20678-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20678-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="20678-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="20678-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="20678-120">Request headers</span></span>
|<span data-ttu-id="20678-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="20678-121">Header</span></span>|<span data-ttu-id="20678-122">値</span><span class="sxs-lookup"><span data-stu-id="20678-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20678-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="20678-123">Authorization</span></span>|<span data-ttu-id="20678-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="20678-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20678-125">Accept</span><span class="sxs-lookup"><span data-stu-id="20678-125">Accept</span></span>|<span data-ttu-id="20678-126">application/json</span><span class="sxs-lookup"><span data-stu-id="20678-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20678-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="20678-127">Request body</span></span>
<span data-ttu-id="20678-128">要求本文で、iosVppEBook オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="20678-128">In the request body, supply a JSON representation for the iosVppEBook object.</span></span>

<span data-ttu-id="20678-129">次の表に、iosVppEBook の作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="20678-129">The following table shows the properties that are required when you create the iosVppEBook.</span></span>

|<span data-ttu-id="20678-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="20678-130">Property</span></span>|<span data-ttu-id="20678-131">型</span><span class="sxs-lookup"><span data-stu-id="20678-131">Type</span></span>|<span data-ttu-id="20678-132">説明</span><span class="sxs-lookup"><span data-stu-id="20678-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20678-133">ID</span><span class="sxs-lookup"><span data-stu-id="20678-133">id</span></span>|<span data-ttu-id="20678-134">String</span><span class="sxs-lookup"><span data-stu-id="20678-134">String</span></span>|<span data-ttu-id="20678-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="20678-135">Key of the entity.</span></span> <span data-ttu-id="20678-136">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="20678-136">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="20678-137">displayName</span><span class="sxs-lookup"><span data-stu-id="20678-137">displayName</span></span>|<span data-ttu-id="20678-138">String</span><span class="sxs-lookup"><span data-stu-id="20678-138">String</span></span>|<span data-ttu-id="20678-139">電子ブックの名前。</span><span class="sxs-lookup"><span data-stu-id="20678-139">Name of the eBook.</span></span> <span data-ttu-id="20678-140">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="20678-140">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="20678-141">説明</span><span class="sxs-lookup"><span data-stu-id="20678-141">description</span></span>|<span data-ttu-id="20678-142">String</span><span class="sxs-lookup"><span data-stu-id="20678-142">String</span></span>|<span data-ttu-id="20678-143">説明。</span><span class="sxs-lookup"><span data-stu-id="20678-143">Description.</span></span> <span data-ttu-id="20678-144">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="20678-144">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="20678-145">publisher</span><span class="sxs-lookup"><span data-stu-id="20678-145">publisher</span></span>|<span data-ttu-id="20678-146">String</span><span class="sxs-lookup"><span data-stu-id="20678-146">String</span></span>|<span data-ttu-id="20678-147">発行元です。</span><span class="sxs-lookup"><span data-stu-id="20678-147">Publisher.</span></span> <span data-ttu-id="20678-148">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="20678-148">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="20678-149">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="20678-149">publishedDateTime</span></span>|<span data-ttu-id="20678-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20678-150">DateTimeOffset</span></span>|<span data-ttu-id="20678-151">電子ブックが発行された日時。</span><span class="sxs-lookup"><span data-stu-id="20678-151">The date and time when the eBook was published.</span></span> <span data-ttu-id="20678-152">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="20678-152">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="20678-153">largeCover</span><span class="sxs-lookup"><span data-stu-id="20678-153">largeCover</span></span>|[<span data-ttu-id="20678-154">mimeContent</span><span class="sxs-lookup"><span data-stu-id="20678-154">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="20678-155">ブック カバー。</span><span class="sxs-lookup"><span data-stu-id="20678-155">Book cover.</span></span> <span data-ttu-id="20678-156">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="20678-156">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="20678-157">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="20678-157">createdDateTime</span></span>|<span data-ttu-id="20678-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20678-158">DateTimeOffset</span></span>|<span data-ttu-id="20678-159">電子ブック ファイルが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="20678-159">The date and time when the eBook file was created.</span></span> <span data-ttu-id="20678-160">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="20678-160">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="20678-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="20678-161">lastModifiedDateTime</span></span>|<span data-ttu-id="20678-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20678-162">DateTimeOffset</span></span>|<span data-ttu-id="20678-163">電子ブックが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="20678-163">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="20678-164">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="20678-164">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="20678-165">informationUrl</span><span class="sxs-lookup"><span data-stu-id="20678-165">informationUrl</span></span>|<span data-ttu-id="20678-166">String</span><span class="sxs-lookup"><span data-stu-id="20678-166">String</span></span>|<span data-ttu-id="20678-167">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="20678-167">The more information Url.</span></span> <span data-ttu-id="20678-168">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="20678-168">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="20678-169">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="20678-169">privacyInformationUrl</span></span>|<span data-ttu-id="20678-170">String</span><span class="sxs-lookup"><span data-stu-id="20678-170">String</span></span>|<span data-ttu-id="20678-171">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="20678-171">The privacy statement Url.</span></span> <span data-ttu-id="20678-172">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="20678-172">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="20678-173">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="20678-173">vppTokenId</span></span>|<span data-ttu-id="20678-174">Guid</span><span class="sxs-lookup"><span data-stu-id="20678-174">Guid</span></span>|<span data-ttu-id="20678-175">Vpp トークン ID。</span><span class="sxs-lookup"><span data-stu-id="20678-175">The Vpp token ID.</span></span>|
|<span data-ttu-id="20678-176">appleId</span><span class="sxs-lookup"><span data-stu-id="20678-176">appleId</span></span>|<span data-ttu-id="20678-177">String</span><span class="sxs-lookup"><span data-stu-id="20678-177">String</span></span>|<span data-ttu-id="20678-178">Vpp トークンに関連付けられている Apple ID。</span><span class="sxs-lookup"><span data-stu-id="20678-178">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="20678-179">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="20678-179">vppOrganizationName</span></span>|<span data-ttu-id="20678-180">String</span><span class="sxs-lookup"><span data-stu-id="20678-180">String</span></span>|<span data-ttu-id="20678-181">Vpp トークンの組織の名前。</span><span class="sxs-lookup"><span data-stu-id="20678-181">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="20678-182">genres</span><span class="sxs-lookup"><span data-stu-id="20678-182">genres</span></span>|<span data-ttu-id="20678-183">String コレクション</span><span class="sxs-lookup"><span data-stu-id="20678-183">String collection</span></span>|<span data-ttu-id="20678-184">ジャンル。</span><span class="sxs-lookup"><span data-stu-id="20678-184">Genres.</span></span>|
|<span data-ttu-id="20678-185">language</span><span class="sxs-lookup"><span data-stu-id="20678-185">language</span></span>|<span data-ttu-id="20678-186">String</span><span class="sxs-lookup"><span data-stu-id="20678-186">String</span></span>|<span data-ttu-id="20678-187">言語。</span><span class="sxs-lookup"><span data-stu-id="20678-187">Language.</span></span>|
|<span data-ttu-id="20678-188">seller</span><span class="sxs-lookup"><span data-stu-id="20678-188">seller</span></span>|<span data-ttu-id="20678-189">String</span><span class="sxs-lookup"><span data-stu-id="20678-189">String</span></span>|<span data-ttu-id="20678-190">販売元。</span><span class="sxs-lookup"><span data-stu-id="20678-190">Seller.</span></span>|
|<span data-ttu-id="20678-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="20678-191">totalLicenseCount</span></span>|<span data-ttu-id="20678-192">Int32</span><span class="sxs-lookup"><span data-stu-id="20678-192">Int32</span></span>|<span data-ttu-id="20678-193">ライセンスの合計数。</span><span class="sxs-lookup"><span data-stu-id="20678-193">Total license count.</span></span>|
|<span data-ttu-id="20678-194">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="20678-194">usedLicenseCount</span></span>|<span data-ttu-id="20678-195">Int32</span><span class="sxs-lookup"><span data-stu-id="20678-195">Int32</span></span>|<span data-ttu-id="20678-196">使用されているライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="20678-196">Used license count.</span></span>|



## <a name="response"></a><span data-ttu-id="20678-197">応答</span><span class="sxs-lookup"><span data-stu-id="20678-197">Response</span></span>
<span data-ttu-id="20678-198">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosVppEBook](../resources/intune-books-iosvppebook.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="20678-198">If successful, this method returns a `201 Created` response code and a [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20678-199">例</span><span class="sxs-lookup"><span data-stu-id="20678-199">Example</span></span>
### <a name="request"></a><span data-ttu-id="20678-200">要求</span><span class="sxs-lookup"><span data-stu-id="20678-200">Request</span></span>
<span data-ttu-id="20678-201">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="20678-201">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks
Content-type: application/json
Content-length: 856

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

### <a name="response"></a><span data-ttu-id="20678-202">応答</span><span class="sxs-lookup"><span data-stu-id="20678-202">Response</span></span>
<span data-ttu-id="20678-p113">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="20678-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





