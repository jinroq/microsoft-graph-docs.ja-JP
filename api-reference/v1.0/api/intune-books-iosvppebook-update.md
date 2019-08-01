---
title: iosVppEBook の更新
description: iosVppEBook オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d68b8ba149b4b5f8b63029df98769d37a5fdd8c7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001881"
---
# <a name="update-iosvppebook"></a><span data-ttu-id="ef7c4-103">iosVppEBook の更新</span><span class="sxs-lookup"><span data-stu-id="ef7c4-103">Update iosVppEBook</span></span>

> <span data-ttu-id="ef7c4-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ef7c4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ef7c4-105">[iosVppEBook](../resources/intune-books-iosvppebook.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ef7c4-105">Update the properties of a [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ef7c4-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="ef7c4-106">Prerequisites</span></span>
<span data-ttu-id="ef7c4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ef7c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef7c4-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ef7c4-109">Permission type</span></span>|<span data-ttu-id="ef7c4-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ef7c4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef7c4-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ef7c4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ef7c4-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef7c4-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ef7c4-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ef7c4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef7c4-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ef7c4-114">Not supported.</span></span>|
|<span data-ttu-id="ef7c4-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ef7c4-115">Application</span></span>|<span data-ttu-id="ef7c4-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ef7c4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef7c4-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ef7c4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="request-headers"></a><span data-ttu-id="ef7c4-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ef7c4-118">Request headers</span></span>
|<span data-ttu-id="ef7c4-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ef7c4-119">Header</span></span>|<span data-ttu-id="ef7c4-120">値</span><span class="sxs-lookup"><span data-stu-id="ef7c4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef7c4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef7c4-121">Authorization</span></span>|<span data-ttu-id="ef7c4-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ef7c4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef7c4-123">承諾</span><span class="sxs-lookup"><span data-stu-id="ef7c4-123">Accept</span></span>|<span data-ttu-id="ef7c4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ef7c4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef7c4-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="ef7c4-125">Request body</span></span>
<span data-ttu-id="ef7c4-126">要求本文で、[iosVppEBook](../resources/intune-books-iosvppebook.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ef7c4-126">In the request body, supply a JSON representation for the [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

<span data-ttu-id="ef7c4-127">次の表に、[iosVppEBook](../resources/intune-books-iosvppebook.md) の作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ef7c4-127">The following table shows the properties that are required when you create the [iosVppEBook](../resources/intune-books-iosvppebook.md).</span></span>

|<span data-ttu-id="ef7c4-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ef7c4-128">Property</span></span>|<span data-ttu-id="ef7c4-129">型</span><span class="sxs-lookup"><span data-stu-id="ef7c4-129">Type</span></span>|<span data-ttu-id="ef7c4-130">説明</span><span class="sxs-lookup"><span data-stu-id="ef7c4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef7c4-131">id</span><span class="sxs-lookup"><span data-stu-id="ef7c4-131">id</span></span>|<span data-ttu-id="ef7c4-132">文字列</span><span class="sxs-lookup"><span data-stu-id="ef7c4-132">String</span></span>|<span data-ttu-id="ef7c4-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ef7c4-133">Key of the entity.</span></span> <span data-ttu-id="ef7c4-134">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ef7c4-134">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="ef7c4-135">displayName</span><span class="sxs-lookup"><span data-stu-id="ef7c4-135">displayName</span></span>|<span data-ttu-id="ef7c4-136">String</span><span class="sxs-lookup"><span data-stu-id="ef7c4-136">String</span></span>|<span data-ttu-id="ef7c4-137">電子ブックの名前。</span><span class="sxs-lookup"><span data-stu-id="ef7c4-137">Name of the eBook.</span></span> <span data-ttu-id="ef7c4-138">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ef7c4-138">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="ef7c4-139">description</span><span class="sxs-lookup"><span data-stu-id="ef7c4-139">description</span></span>|<span data-ttu-id="ef7c4-140">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ef7c4-140">String</span></span>|<span data-ttu-id="ef7c4-141">説明。</span><span class="sxs-lookup"><span data-stu-id="ef7c4-141">Description.</span></span> <span data-ttu-id="ef7c4-142">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ef7c4-142">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="ef7c4-143">publisher</span><span class="sxs-lookup"><span data-stu-id="ef7c4-143">publisher</span></span>|<span data-ttu-id="ef7c4-144">String</span><span class="sxs-lookup"><span data-stu-id="ef7c4-144">String</span></span>|<span data-ttu-id="ef7c4-145">発行元。</span><span class="sxs-lookup"><span data-stu-id="ef7c4-145">Publisher.</span></span> <span data-ttu-id="ef7c4-146">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ef7c4-146">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="ef7c4-147">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="ef7c4-147">publishedDateTime</span></span>|<span data-ttu-id="ef7c4-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef7c4-148">DateTimeOffset</span></span>|<span data-ttu-id="ef7c4-149">電子ブックが発行された日時。</span><span class="sxs-lookup"><span data-stu-id="ef7c4-149">The date and time when the eBook was published.</span></span> <span data-ttu-id="ef7c4-150">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ef7c4-150">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="ef7c4-151">largeCover</span><span class="sxs-lookup"><span data-stu-id="ef7c4-151">largeCover</span></span>|[<span data-ttu-id="ef7c4-152">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ef7c4-152">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ef7c4-153">ブック カバー。</span><span class="sxs-lookup"><span data-stu-id="ef7c4-153">Book cover.</span></span> <span data-ttu-id="ef7c4-154">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ef7c4-154">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="ef7c4-155">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ef7c4-155">createdDateTime</span></span>|<span data-ttu-id="ef7c4-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef7c4-156">DateTimeOffset</span></span>|<span data-ttu-id="ef7c4-157">電子ブック ファイルが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="ef7c4-157">The date and time when the eBook file was created.</span></span> <span data-ttu-id="ef7c4-158">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ef7c4-158">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="ef7c4-159">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ef7c4-159">lastModifiedDateTime</span></span>|<span data-ttu-id="ef7c4-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef7c4-160">DateTimeOffset</span></span>|<span data-ttu-id="ef7c4-161">電子ブックが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="ef7c4-161">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="ef7c4-162">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ef7c4-162">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="ef7c4-163">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ef7c4-163">informationUrl</span></span>|<span data-ttu-id="ef7c4-164">String</span><span class="sxs-lookup"><span data-stu-id="ef7c4-164">String</span></span>|<span data-ttu-id="ef7c4-165">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="ef7c4-165">The more information Url.</span></span> <span data-ttu-id="ef7c4-166">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ef7c4-166">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="ef7c4-167">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ef7c4-167">privacyInformationUrl</span></span>|<span data-ttu-id="ef7c4-168">String</span><span class="sxs-lookup"><span data-stu-id="ef7c4-168">String</span></span>|<span data-ttu-id="ef7c4-169">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="ef7c4-169">The privacy statement Url.</span></span> <span data-ttu-id="ef7c4-170">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ef7c4-170">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="ef7c4-171">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="ef7c4-171">vppTokenId</span></span>|<span data-ttu-id="ef7c4-172">Guid</span><span class="sxs-lookup"><span data-stu-id="ef7c4-172">Guid</span></span>|<span data-ttu-id="ef7c4-173">Vpp トークン ID。</span><span class="sxs-lookup"><span data-stu-id="ef7c4-173">The Vpp token ID.</span></span>|
|<span data-ttu-id="ef7c4-174">appleId</span><span class="sxs-lookup"><span data-stu-id="ef7c4-174">appleId</span></span>|<span data-ttu-id="ef7c4-175">文字列</span><span class="sxs-lookup"><span data-stu-id="ef7c4-175">String</span></span>|<span data-ttu-id="ef7c4-176">Vpp トークンに関連付けられている Apple ID。</span><span class="sxs-lookup"><span data-stu-id="ef7c4-176">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="ef7c4-177">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="ef7c4-177">vppOrganizationName</span></span>|<span data-ttu-id="ef7c4-178">String</span><span class="sxs-lookup"><span data-stu-id="ef7c4-178">String</span></span>|<span data-ttu-id="ef7c4-179">Vpp トークンの組織の名前。</span><span class="sxs-lookup"><span data-stu-id="ef7c4-179">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="ef7c4-180">genres</span><span class="sxs-lookup"><span data-stu-id="ef7c4-180">genres</span></span>|<span data-ttu-id="ef7c4-181">String コレクション</span><span class="sxs-lookup"><span data-stu-id="ef7c4-181">String collection</span></span>|<span data-ttu-id="ef7c4-182">ジャンル。</span><span class="sxs-lookup"><span data-stu-id="ef7c4-182">Genres.</span></span>|
|<span data-ttu-id="ef7c4-183">language</span><span class="sxs-lookup"><span data-stu-id="ef7c4-183">language</span></span>|<span data-ttu-id="ef7c4-184">String</span><span class="sxs-lookup"><span data-stu-id="ef7c4-184">String</span></span>|<span data-ttu-id="ef7c4-185">言語。</span><span class="sxs-lookup"><span data-stu-id="ef7c4-185">Language.</span></span>|
|<span data-ttu-id="ef7c4-186">seller</span><span class="sxs-lookup"><span data-stu-id="ef7c4-186">seller</span></span>|<span data-ttu-id="ef7c4-187">String</span><span class="sxs-lookup"><span data-stu-id="ef7c4-187">String</span></span>|<span data-ttu-id="ef7c4-188">販売元。</span><span class="sxs-lookup"><span data-stu-id="ef7c4-188">Seller.</span></span>|
|<span data-ttu-id="ef7c4-189">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="ef7c4-189">totalLicenseCount</span></span>|<span data-ttu-id="ef7c4-190">Int32</span><span class="sxs-lookup"><span data-stu-id="ef7c4-190">Int32</span></span>|<span data-ttu-id="ef7c4-191">ライセンスの合計数。</span><span class="sxs-lookup"><span data-stu-id="ef7c4-191">Total license count.</span></span>|
|<span data-ttu-id="ef7c4-192">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="ef7c4-192">usedLicenseCount</span></span>|<span data-ttu-id="ef7c4-193">Int32</span><span class="sxs-lookup"><span data-stu-id="ef7c4-193">Int32</span></span>|<span data-ttu-id="ef7c4-194">使用されているライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="ef7c4-194">Used license count.</span></span>|



## <a name="response"></a><span data-ttu-id="ef7c4-195">応答</span><span class="sxs-lookup"><span data-stu-id="ef7c4-195">Response</span></span>
<span data-ttu-id="ef7c4-196">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [iosVppEBook](../resources/intune-books-iosvppebook.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ef7c4-196">If successful, this method returns a `200 OK` response code and an updated [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef7c4-197">例</span><span class="sxs-lookup"><span data-stu-id="ef7c4-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="ef7c4-198">要求</span><span class="sxs-lookup"><span data-stu-id="ef7c4-198">Request</span></span>
<span data-ttu-id="ef7c4-199">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ef7c4-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}
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

### <a name="response"></a><span data-ttu-id="ef7c4-200">応答</span><span class="sxs-lookup"><span data-stu-id="ef7c4-200">Response</span></span>
<span data-ttu-id="ef7c4-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ef7c4-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



