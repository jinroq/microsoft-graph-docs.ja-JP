---
title: iosVppEBook の作成
description: 新しい iosVppEBook オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 267ee13b37657d18a3123cec15eb3ea88d70a47d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36015839"
---
# <a name="create-iosvppebook"></a><span data-ttu-id="67fe3-103">iosVppEBook の作成</span><span class="sxs-lookup"><span data-stu-id="67fe3-103">Create iosVppEBook</span></span>

> <span data-ttu-id="67fe3-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="67fe3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67fe3-105">新しい [iosVppEBook](../resources/intune-books-iosvppebook.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="67fe3-105">Create a new [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67fe3-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="67fe3-106">Prerequisites</span></span>
<span data-ttu-id="67fe3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="67fe3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67fe3-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="67fe3-109">Permission type</span></span>|<span data-ttu-id="67fe3-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="67fe3-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67fe3-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="67fe3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="67fe3-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67fe3-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="67fe3-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="67fe3-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67fe3-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67fe3-114">Not supported.</span></span>|
|<span data-ttu-id="67fe3-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="67fe3-115">Application</span></span>|<span data-ttu-id="67fe3-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67fe3-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67fe3-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="67fe3-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks
```

## <a name="request-headers"></a><span data-ttu-id="67fe3-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="67fe3-118">Request headers</span></span>
|<span data-ttu-id="67fe3-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="67fe3-119">Header</span></span>|<span data-ttu-id="67fe3-120">値</span><span class="sxs-lookup"><span data-stu-id="67fe3-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67fe3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="67fe3-121">Authorization</span></span>|<span data-ttu-id="67fe3-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="67fe3-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67fe3-123">承諾</span><span class="sxs-lookup"><span data-stu-id="67fe3-123">Accept</span></span>|<span data-ttu-id="67fe3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="67fe3-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67fe3-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="67fe3-125">Request body</span></span>
<span data-ttu-id="67fe3-126">要求本文で、iosVppEBook オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="67fe3-126">In the request body, supply a JSON representation for the iosVppEBook object.</span></span>

<span data-ttu-id="67fe3-127">次の表に、iosVppEBook の作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="67fe3-127">The following table shows the properties that are required when you create the iosVppEBook.</span></span>

|<span data-ttu-id="67fe3-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="67fe3-128">Property</span></span>|<span data-ttu-id="67fe3-129">型</span><span class="sxs-lookup"><span data-stu-id="67fe3-129">Type</span></span>|<span data-ttu-id="67fe3-130">説明</span><span class="sxs-lookup"><span data-stu-id="67fe3-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67fe3-131">id</span><span class="sxs-lookup"><span data-stu-id="67fe3-131">id</span></span>|<span data-ttu-id="67fe3-132">文字列</span><span class="sxs-lookup"><span data-stu-id="67fe3-132">String</span></span>|<span data-ttu-id="67fe3-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="67fe3-133">Key of the entity.</span></span> <span data-ttu-id="67fe3-134">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67fe3-134">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="67fe3-135">displayName</span><span class="sxs-lookup"><span data-stu-id="67fe3-135">displayName</span></span>|<span data-ttu-id="67fe3-136">String</span><span class="sxs-lookup"><span data-stu-id="67fe3-136">String</span></span>|<span data-ttu-id="67fe3-137">電子ブックの名前。</span><span class="sxs-lookup"><span data-stu-id="67fe3-137">Name of the eBook.</span></span> <span data-ttu-id="67fe3-138">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67fe3-138">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="67fe3-139">description</span><span class="sxs-lookup"><span data-stu-id="67fe3-139">description</span></span>|<span data-ttu-id="67fe3-140">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="67fe3-140">String</span></span>|<span data-ttu-id="67fe3-141">説明。</span><span class="sxs-lookup"><span data-stu-id="67fe3-141">Description.</span></span> <span data-ttu-id="67fe3-142">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67fe3-142">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="67fe3-143">publisher</span><span class="sxs-lookup"><span data-stu-id="67fe3-143">publisher</span></span>|<span data-ttu-id="67fe3-144">String</span><span class="sxs-lookup"><span data-stu-id="67fe3-144">String</span></span>|<span data-ttu-id="67fe3-145">発行元。</span><span class="sxs-lookup"><span data-stu-id="67fe3-145">Publisher.</span></span> <span data-ttu-id="67fe3-146">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67fe3-146">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="67fe3-147">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="67fe3-147">publishedDateTime</span></span>|<span data-ttu-id="67fe3-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67fe3-148">DateTimeOffset</span></span>|<span data-ttu-id="67fe3-149">電子ブックが発行された日時。</span><span class="sxs-lookup"><span data-stu-id="67fe3-149">The date and time when the eBook was published.</span></span> <span data-ttu-id="67fe3-150">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67fe3-150">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="67fe3-151">largeCover</span><span class="sxs-lookup"><span data-stu-id="67fe3-151">largeCover</span></span>|[<span data-ttu-id="67fe3-152">mimeContent</span><span class="sxs-lookup"><span data-stu-id="67fe3-152">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="67fe3-153">ブック カバー。</span><span class="sxs-lookup"><span data-stu-id="67fe3-153">Book cover.</span></span> <span data-ttu-id="67fe3-154">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67fe3-154">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="67fe3-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="67fe3-155">createdDateTime</span></span>|<span data-ttu-id="67fe3-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67fe3-156">DateTimeOffset</span></span>|<span data-ttu-id="67fe3-157">電子ブック ファイルが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="67fe3-157">The date and time when the eBook file was created.</span></span> <span data-ttu-id="67fe3-158">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67fe3-158">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="67fe3-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="67fe3-159">lastModifiedDateTime</span></span>|<span data-ttu-id="67fe3-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67fe3-160">DateTimeOffset</span></span>|<span data-ttu-id="67fe3-161">電子ブックが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="67fe3-161">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="67fe3-162">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67fe3-162">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="67fe3-163">informationUrl</span><span class="sxs-lookup"><span data-stu-id="67fe3-163">informationUrl</span></span>|<span data-ttu-id="67fe3-164">String</span><span class="sxs-lookup"><span data-stu-id="67fe3-164">String</span></span>|<span data-ttu-id="67fe3-165">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="67fe3-165">The more information Url.</span></span> <span data-ttu-id="67fe3-166">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67fe3-166">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="67fe3-167">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="67fe3-167">privacyInformationUrl</span></span>|<span data-ttu-id="67fe3-168">String</span><span class="sxs-lookup"><span data-stu-id="67fe3-168">String</span></span>|<span data-ttu-id="67fe3-169">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="67fe3-169">The privacy statement Url.</span></span> <span data-ttu-id="67fe3-170">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67fe3-170">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="67fe3-171">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="67fe3-171">vppTokenId</span></span>|<span data-ttu-id="67fe3-172">Guid</span><span class="sxs-lookup"><span data-stu-id="67fe3-172">Guid</span></span>|<span data-ttu-id="67fe3-173">Vpp トークン ID。</span><span class="sxs-lookup"><span data-stu-id="67fe3-173">The Vpp token ID.</span></span>|
|<span data-ttu-id="67fe3-174">appleId</span><span class="sxs-lookup"><span data-stu-id="67fe3-174">appleId</span></span>|<span data-ttu-id="67fe3-175">文字列</span><span class="sxs-lookup"><span data-stu-id="67fe3-175">String</span></span>|<span data-ttu-id="67fe3-176">Vpp トークンに関連付けられている Apple ID。</span><span class="sxs-lookup"><span data-stu-id="67fe3-176">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="67fe3-177">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="67fe3-177">vppOrganizationName</span></span>|<span data-ttu-id="67fe3-178">String</span><span class="sxs-lookup"><span data-stu-id="67fe3-178">String</span></span>|<span data-ttu-id="67fe3-179">Vpp トークンの組織の名前。</span><span class="sxs-lookup"><span data-stu-id="67fe3-179">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="67fe3-180">genres</span><span class="sxs-lookup"><span data-stu-id="67fe3-180">genres</span></span>|<span data-ttu-id="67fe3-181">String コレクション</span><span class="sxs-lookup"><span data-stu-id="67fe3-181">String collection</span></span>|<span data-ttu-id="67fe3-182">ジャンル。</span><span class="sxs-lookup"><span data-stu-id="67fe3-182">Genres.</span></span>|
|<span data-ttu-id="67fe3-183">language</span><span class="sxs-lookup"><span data-stu-id="67fe3-183">language</span></span>|<span data-ttu-id="67fe3-184">String</span><span class="sxs-lookup"><span data-stu-id="67fe3-184">String</span></span>|<span data-ttu-id="67fe3-185">言語。</span><span class="sxs-lookup"><span data-stu-id="67fe3-185">Language.</span></span>|
|<span data-ttu-id="67fe3-186">seller</span><span class="sxs-lookup"><span data-stu-id="67fe3-186">seller</span></span>|<span data-ttu-id="67fe3-187">String</span><span class="sxs-lookup"><span data-stu-id="67fe3-187">String</span></span>|<span data-ttu-id="67fe3-188">販売元。</span><span class="sxs-lookup"><span data-stu-id="67fe3-188">Seller.</span></span>|
|<span data-ttu-id="67fe3-189">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="67fe3-189">totalLicenseCount</span></span>|<span data-ttu-id="67fe3-190">Int32</span><span class="sxs-lookup"><span data-stu-id="67fe3-190">Int32</span></span>|<span data-ttu-id="67fe3-191">ライセンスの合計数。</span><span class="sxs-lookup"><span data-stu-id="67fe3-191">Total license count.</span></span>|
|<span data-ttu-id="67fe3-192">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="67fe3-192">usedLicenseCount</span></span>|<span data-ttu-id="67fe3-193">Int32</span><span class="sxs-lookup"><span data-stu-id="67fe3-193">Int32</span></span>|<span data-ttu-id="67fe3-194">使用されているライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="67fe3-194">Used license count.</span></span>|



## <a name="response"></a><span data-ttu-id="67fe3-195">応答</span><span class="sxs-lookup"><span data-stu-id="67fe3-195">Response</span></span>
<span data-ttu-id="67fe3-196">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosVppEBook](../resources/intune-books-iosvppebook.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="67fe3-196">If successful, this method returns a `201 Created` response code and a [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67fe3-197">例</span><span class="sxs-lookup"><span data-stu-id="67fe3-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="67fe3-198">要求</span><span class="sxs-lookup"><span data-stu-id="67fe3-198">Request</span></span>
<span data-ttu-id="67fe3-199">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="67fe3-199">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="67fe3-200">応答</span><span class="sxs-lookup"><span data-stu-id="67fe3-200">Response</span></span>
<span data-ttu-id="67fe3-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="67fe3-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



