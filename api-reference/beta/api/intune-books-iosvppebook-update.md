---
title: iosVppEBook の更新
description: iosVppEBook オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 75923333d699e4cd8cd24a223231d3b720aea542
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36328453"
---
# <a name="update-iosvppebook"></a><span data-ttu-id="38084-103">iosVppEBook の更新</span><span class="sxs-lookup"><span data-stu-id="38084-103">Update iosVppEBook</span></span>

> <span data-ttu-id="38084-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="38084-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="38084-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="38084-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38084-106">[iosVppEBook](../resources/intune-books-iosvppebook.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="38084-106">Update the properties of a [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38084-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="38084-107">Prerequisites</span></span>
<span data-ttu-id="38084-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="38084-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38084-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="38084-110">Permission type</span></span>|<span data-ttu-id="38084-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="38084-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38084-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="38084-112">Delegated (work or school account)</span></span>|<span data-ttu-id="38084-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38084-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="38084-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="38084-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38084-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="38084-115">Not supported.</span></span>|
|<span data-ttu-id="38084-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="38084-116">Application</span></span>|<span data-ttu-id="38084-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38084-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="38084-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="38084-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="request-headers"></a><span data-ttu-id="38084-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="38084-119">Request headers</span></span>
|<span data-ttu-id="38084-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="38084-120">Header</span></span>|<span data-ttu-id="38084-121">値</span><span class="sxs-lookup"><span data-stu-id="38084-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38084-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="38084-122">Authorization</span></span>|<span data-ttu-id="38084-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="38084-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38084-124">承諾</span><span class="sxs-lookup"><span data-stu-id="38084-124">Accept</span></span>|<span data-ttu-id="38084-125">application/json</span><span class="sxs-lookup"><span data-stu-id="38084-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38084-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="38084-126">Request body</span></span>
<span data-ttu-id="38084-127">要求本文で、[iosVppEBook](../resources/intune-books-iosvppebook.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="38084-127">In the request body, supply a JSON representation for the [iosVppEBook](../resources/intune-books-iosvppebook.md) object.</span></span>

<span data-ttu-id="38084-128">次の表に、[iosVppEBook](../resources/intune-books-iosvppebook.md) の作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="38084-128">The following table shows the properties that are required when you create the [iosVppEBook](../resources/intune-books-iosvppebook.md).</span></span>

|<span data-ttu-id="38084-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="38084-129">Property</span></span>|<span data-ttu-id="38084-130">型</span><span class="sxs-lookup"><span data-stu-id="38084-130">Type</span></span>|<span data-ttu-id="38084-131">説明</span><span class="sxs-lookup"><span data-stu-id="38084-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38084-132">id</span><span class="sxs-lookup"><span data-stu-id="38084-132">id</span></span>|<span data-ttu-id="38084-133">文字列</span><span class="sxs-lookup"><span data-stu-id="38084-133">String</span></span>|<span data-ttu-id="38084-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="38084-134">Key of the entity.</span></span> <span data-ttu-id="38084-135">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="38084-135">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="38084-136">displayName</span><span class="sxs-lookup"><span data-stu-id="38084-136">displayName</span></span>|<span data-ttu-id="38084-137">String</span><span class="sxs-lookup"><span data-stu-id="38084-137">String</span></span>|<span data-ttu-id="38084-138">電子ブックの名前。</span><span class="sxs-lookup"><span data-stu-id="38084-138">Name of the eBook.</span></span> <span data-ttu-id="38084-139">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="38084-139">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="38084-140">description</span><span class="sxs-lookup"><span data-stu-id="38084-140">description</span></span>|<span data-ttu-id="38084-141">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="38084-141">String</span></span>|<span data-ttu-id="38084-142">説明。</span><span class="sxs-lookup"><span data-stu-id="38084-142">Description.</span></span> <span data-ttu-id="38084-143">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="38084-143">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="38084-144">publisher</span><span class="sxs-lookup"><span data-stu-id="38084-144">publisher</span></span>|<span data-ttu-id="38084-145">String</span><span class="sxs-lookup"><span data-stu-id="38084-145">String</span></span>|<span data-ttu-id="38084-146">発行元。</span><span class="sxs-lookup"><span data-stu-id="38084-146">Publisher.</span></span> <span data-ttu-id="38084-147">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="38084-147">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="38084-148">publishedDateTime</span><span class="sxs-lookup"><span data-stu-id="38084-148">publishedDateTime</span></span>|<span data-ttu-id="38084-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38084-149">DateTimeOffset</span></span>|<span data-ttu-id="38084-150">電子ブックが発行された日時。</span><span class="sxs-lookup"><span data-stu-id="38084-150">The date and time when the eBook was published.</span></span> <span data-ttu-id="38084-151">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="38084-151">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="38084-152">largeCover</span><span class="sxs-lookup"><span data-stu-id="38084-152">largeCover</span></span>|[<span data-ttu-id="38084-153">mimeContent</span><span class="sxs-lookup"><span data-stu-id="38084-153">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="38084-154">ブック カバー。</span><span class="sxs-lookup"><span data-stu-id="38084-154">Book cover.</span></span> <span data-ttu-id="38084-155">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="38084-155">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="38084-156">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="38084-156">createdDateTime</span></span>|<span data-ttu-id="38084-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38084-157">DateTimeOffset</span></span>|<span data-ttu-id="38084-158">電子ブック ファイルが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="38084-158">The date and time when the eBook file was created.</span></span> <span data-ttu-id="38084-159">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="38084-159">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="38084-160">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="38084-160">lastModifiedDateTime</span></span>|<span data-ttu-id="38084-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38084-161">DateTimeOffset</span></span>|<span data-ttu-id="38084-162">電子ブックが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="38084-162">The date and time when the eBook was last modified.</span></span> <span data-ttu-id="38084-163">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="38084-163">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="38084-164">informationUrl</span><span class="sxs-lookup"><span data-stu-id="38084-164">informationUrl</span></span>|<span data-ttu-id="38084-165">String</span><span class="sxs-lookup"><span data-stu-id="38084-165">String</span></span>|<span data-ttu-id="38084-166">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="38084-166">The more information Url.</span></span> <span data-ttu-id="38084-167">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="38084-167">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="38084-168">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="38084-168">privacyInformationUrl</span></span>|<span data-ttu-id="38084-169">String</span><span class="sxs-lookup"><span data-stu-id="38084-169">String</span></span>|<span data-ttu-id="38084-170">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="38084-170">The privacy statement Url.</span></span> <span data-ttu-id="38084-171">[managedEBook](../resources/intune-books-managedebook.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="38084-171">Inherited from [managedEBook](../resources/intune-books-managedebook.md)</span></span>|
|<span data-ttu-id="38084-172">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="38084-172">vppTokenId</span></span>|<span data-ttu-id="38084-173">Guid</span><span class="sxs-lookup"><span data-stu-id="38084-173">Guid</span></span>|<span data-ttu-id="38084-174">Vpp トークン ID。</span><span class="sxs-lookup"><span data-stu-id="38084-174">The Vpp token ID.</span></span>|
|<span data-ttu-id="38084-175">appleId</span><span class="sxs-lookup"><span data-stu-id="38084-175">appleId</span></span>|<span data-ttu-id="38084-176">文字列</span><span class="sxs-lookup"><span data-stu-id="38084-176">String</span></span>|<span data-ttu-id="38084-177">Vpp トークンに関連付けられている Apple ID。</span><span class="sxs-lookup"><span data-stu-id="38084-177">The Apple ID associated with Vpp token.</span></span>|
|<span data-ttu-id="38084-178">vppOrganizationName</span><span class="sxs-lookup"><span data-stu-id="38084-178">vppOrganizationName</span></span>|<span data-ttu-id="38084-179">String</span><span class="sxs-lookup"><span data-stu-id="38084-179">String</span></span>|<span data-ttu-id="38084-180">Vpp トークンの組織の名前。</span><span class="sxs-lookup"><span data-stu-id="38084-180">The Vpp token's organization name.</span></span>|
|<span data-ttu-id="38084-181">genres</span><span class="sxs-lookup"><span data-stu-id="38084-181">genres</span></span>|<span data-ttu-id="38084-182">String コレクション</span><span class="sxs-lookup"><span data-stu-id="38084-182">String collection</span></span>|<span data-ttu-id="38084-183">ジャンル。</span><span class="sxs-lookup"><span data-stu-id="38084-183">Genres.</span></span>|
|<span data-ttu-id="38084-184">language</span><span class="sxs-lookup"><span data-stu-id="38084-184">language</span></span>|<span data-ttu-id="38084-185">String</span><span class="sxs-lookup"><span data-stu-id="38084-185">String</span></span>|<span data-ttu-id="38084-186">言語。</span><span class="sxs-lookup"><span data-stu-id="38084-186">Language.</span></span>|
|<span data-ttu-id="38084-187">seller</span><span class="sxs-lookup"><span data-stu-id="38084-187">seller</span></span>|<span data-ttu-id="38084-188">String</span><span class="sxs-lookup"><span data-stu-id="38084-188">String</span></span>|<span data-ttu-id="38084-189">販売元。</span><span class="sxs-lookup"><span data-stu-id="38084-189">Seller.</span></span>|
|<span data-ttu-id="38084-190">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="38084-190">totalLicenseCount</span></span>|<span data-ttu-id="38084-191">Int32</span><span class="sxs-lookup"><span data-stu-id="38084-191">Int32</span></span>|<span data-ttu-id="38084-192">ライセンスの合計数。</span><span class="sxs-lookup"><span data-stu-id="38084-192">Total license count.</span></span>|
|<span data-ttu-id="38084-193">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="38084-193">usedLicenseCount</span></span>|<span data-ttu-id="38084-194">Int32</span><span class="sxs-lookup"><span data-stu-id="38084-194">Int32</span></span>|<span data-ttu-id="38084-195">使用されているライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="38084-195">Used license count.</span></span>|
|<span data-ttu-id="38084-196">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="38084-196">roleScopeTagIds</span></span>|<span data-ttu-id="38084-197">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="38084-197">String collection</span></span>|<span data-ttu-id="38084-198">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="38084-198">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="38084-199">応答</span><span class="sxs-lookup"><span data-stu-id="38084-199">Response</span></span>
<span data-ttu-id="38084-200">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [iosVppEBook](../resources/intune-books-iosvppebook.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="38084-200">If successful, this method returns a `200 OK` response code and an updated [iosVppEBook](../resources/intune-books-iosvppebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38084-201">例</span><span class="sxs-lookup"><span data-stu-id="38084-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="38084-202">要求</span><span class="sxs-lookup"><span data-stu-id="38084-202">Request</span></span>
<span data-ttu-id="38084-203">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="38084-203">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}
Content-type: application/json
Content-length: 854

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
  "usedLicenseCount": 0,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="38084-204">応答</span><span class="sxs-lookup"><span data-stu-id="38084-204">Response</span></span>
<span data-ttu-id="38084-p112">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="38084-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1026

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
  "usedLicenseCount": 0,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```






