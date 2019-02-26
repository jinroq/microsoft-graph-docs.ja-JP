---
title: Create microsoftStoreForBusinessApp
description: 新しい microsoftStoreForBusinessApp オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6386c767e4140ccc9e138403a90f3002ca681c1e
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264387"
---
# <a name="create-microsoftstoreforbusinessapp"></a><span data-ttu-id="f2a48-103">Create microsoftStoreForBusinessApp</span><span class="sxs-lookup"><span data-stu-id="f2a48-103">Create microsoftStoreForBusinessApp</span></span>

> <span data-ttu-id="f2a48-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f2a48-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2a48-105">新しい [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f2a48-105">Create a new [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f2a48-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="f2a48-106">Prerequisites</span></span>
<span data-ttu-id="f2a48-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f2a48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f2a48-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f2a48-109">Permission type</span></span>|<span data-ttu-id="f2a48-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f2a48-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2a48-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f2a48-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f2a48-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2a48-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f2a48-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f2a48-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2a48-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f2a48-114">Not supported.</span></span>|
|<span data-ttu-id="f2a48-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f2a48-115">Application</span></span>|<span data-ttu-id="f2a48-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f2a48-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2a48-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f2a48-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="f2a48-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f2a48-118">Request headers</span></span>
|<span data-ttu-id="f2a48-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f2a48-119">Header</span></span>|<span data-ttu-id="f2a48-120">値</span><span class="sxs-lookup"><span data-stu-id="f2a48-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2a48-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2a48-121">Authorization</span></span>|<span data-ttu-id="f2a48-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f2a48-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2a48-123">承諾</span><span class="sxs-lookup"><span data-stu-id="f2a48-123">Accept</span></span>|<span data-ttu-id="f2a48-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f2a48-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2a48-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="f2a48-125">Request body</span></span>
<span data-ttu-id="f2a48-126">要求本文で、microsoftStoreForBusinessApp オブジェクト用の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f2a48-126">In the request body, supply a JSON representation for the microsoftStoreForBusinessApp object.</span></span>

<span data-ttu-id="f2a48-127">次の表に、microsoftStoreForBusinessApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f2a48-127">The following table shows the properties that are required when you create the microsoftStoreForBusinessApp.</span></span>

|<span data-ttu-id="f2a48-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f2a48-128">Property</span></span>|<span data-ttu-id="f2a48-129">型</span><span class="sxs-lookup"><span data-stu-id="f2a48-129">Type</span></span>|<span data-ttu-id="f2a48-130">説明</span><span class="sxs-lookup"><span data-stu-id="f2a48-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2a48-131">id</span><span class="sxs-lookup"><span data-stu-id="f2a48-131">id</span></span>|<span data-ttu-id="f2a48-132">文字列</span><span class="sxs-lookup"><span data-stu-id="f2a48-132">String</span></span>|<span data-ttu-id="f2a48-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f2a48-133">Key of the entity.</span></span> <span data-ttu-id="f2a48-134">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f2a48-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a48-135">displayName</span><span class="sxs-lookup"><span data-stu-id="f2a48-135">displayName</span></span>|<span data-ttu-id="f2a48-136">String</span><span class="sxs-lookup"><span data-stu-id="f2a48-136">String</span></span>|<span data-ttu-id="f2a48-137">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="f2a48-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f2a48-138">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f2a48-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a48-139">説明</span><span class="sxs-lookup"><span data-stu-id="f2a48-139">description</span></span>|<span data-ttu-id="f2a48-140">文字列</span><span class="sxs-lookup"><span data-stu-id="f2a48-140">String</span></span>|<span data-ttu-id="f2a48-141">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="f2a48-141">The description of the app.</span></span> <span data-ttu-id="f2a48-142">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f2a48-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a48-143">publisher</span><span class="sxs-lookup"><span data-stu-id="f2a48-143">publisher</span></span>|<span data-ttu-id="f2a48-144">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f2a48-144">String</span></span>|<span data-ttu-id="f2a48-145">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="f2a48-145">The publisher of the app.</span></span> <span data-ttu-id="f2a48-146">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f2a48-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a48-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f2a48-147">largeIcon</span></span>|[<span data-ttu-id="f2a48-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f2a48-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f2a48-149">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="f2a48-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f2a48-150">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f2a48-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a48-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f2a48-151">createdDateTime</span></span>|<span data-ttu-id="f2a48-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2a48-152">DateTimeOffset</span></span>|<span data-ttu-id="f2a48-153">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="f2a48-153">The date and time the app was created.</span></span> <span data-ttu-id="f2a48-154">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f2a48-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a48-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2a48-155">lastModifiedDateTime</span></span>|<span data-ttu-id="f2a48-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2a48-156">DateTimeOffset</span></span>|<span data-ttu-id="f2a48-157">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="f2a48-157">The date and time the app was last modified.</span></span> <span data-ttu-id="f2a48-158">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f2a48-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a48-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f2a48-159">isFeatured</span></span>|<span data-ttu-id="f2a48-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2a48-160">Boolean</span></span>|<span data-ttu-id="f2a48-161">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f2a48-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a48-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f2a48-162">privacyInformationUrl</span></span>|<span data-ttu-id="f2a48-163">String</span><span class="sxs-lookup"><span data-stu-id="f2a48-163">String</span></span>|<span data-ttu-id="f2a48-164">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="f2a48-164">The privacy statement Url.</span></span> <span data-ttu-id="f2a48-165">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f2a48-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a48-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f2a48-166">informationUrl</span></span>|<span data-ttu-id="f2a48-167">String</span><span class="sxs-lookup"><span data-stu-id="f2a48-167">String</span></span>|<span data-ttu-id="f2a48-168">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="f2a48-168">The more information Url.</span></span> <span data-ttu-id="f2a48-169">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f2a48-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a48-170">owner</span><span class="sxs-lookup"><span data-stu-id="f2a48-170">owner</span></span>|<span data-ttu-id="f2a48-171">String</span><span class="sxs-lookup"><span data-stu-id="f2a48-171">String</span></span>|<span data-ttu-id="f2a48-172">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="f2a48-172">The owner of the app.</span></span> <span data-ttu-id="f2a48-173">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f2a48-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a48-174">developer</span><span class="sxs-lookup"><span data-stu-id="f2a48-174">developer</span></span>|<span data-ttu-id="f2a48-175">String</span><span class="sxs-lookup"><span data-stu-id="f2a48-175">String</span></span>|<span data-ttu-id="f2a48-176">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="f2a48-176">The developer of the app.</span></span> <span data-ttu-id="f2a48-177">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f2a48-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a48-178">notes</span><span class="sxs-lookup"><span data-stu-id="f2a48-178">notes</span></span>|<span data-ttu-id="f2a48-179">String</span><span class="sxs-lookup"><span data-stu-id="f2a48-179">String</span></span>|<span data-ttu-id="f2a48-180">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="f2a48-180">Notes for the app.</span></span> <span data-ttu-id="f2a48-181">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f2a48-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f2a48-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="f2a48-182">publishingState</span></span>|[<span data-ttu-id="f2a48-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f2a48-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f2a48-184">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="f2a48-184">The publishing state for the app.</span></span> <span data-ttu-id="f2a48-185">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="f2a48-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f2a48-186">[mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="f2a48-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="f2a48-187">可能な値は `notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="f2a48-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f2a48-188">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="f2a48-188">usedLicenseCount</span></span>|<span data-ttu-id="f2a48-189">Int32</span><span class="sxs-lookup"><span data-stu-id="f2a48-189">Int32</span></span>|<span data-ttu-id="f2a48-190">使用中の、ビジネス向け Microsoft Store ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="f2a48-190">The number of Microsoft Store for Business licenses in use.</span></span>|
|<span data-ttu-id="f2a48-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="f2a48-191">totalLicenseCount</span></span>|<span data-ttu-id="f2a48-192">Int32</span><span class="sxs-lookup"><span data-stu-id="f2a48-192">Int32</span></span>|<span data-ttu-id="f2a48-193">ビジネス向け Microsoft Store ライセンスの合計数。</span><span class="sxs-lookup"><span data-stu-id="f2a48-193">The total number of Microsoft Store for Business licenses.</span></span>|
|<span data-ttu-id="f2a48-194">productKey</span><span class="sxs-lookup"><span data-stu-id="f2a48-194">productKey</span></span>|<span data-ttu-id="f2a48-195">String</span><span class="sxs-lookup"><span data-stu-id="f2a48-195">String</span></span>|<span data-ttu-id="f2a48-196">アプリのプロダクト キー</span><span class="sxs-lookup"><span data-stu-id="f2a48-196">The app product key</span></span>|
|<span data-ttu-id="f2a48-197">licenseType</span><span class="sxs-lookup"><span data-stu-id="f2a48-197">licenseType</span></span>|[<span data-ttu-id="f2a48-198">microsoft storeforbusinesslicensetype</span><span class="sxs-lookup"><span data-stu-id="f2a48-198">microsoftStoreForBusinessLicenseType</span></span>](../resources/intune-apps-microsoftstoreforbusinesslicensetype.md)|<span data-ttu-id="f2a48-199">アプリライセンスの種類。</span><span class="sxs-lookup"><span data-stu-id="f2a48-199">The app license type.</span></span> <span data-ttu-id="f2a48-200">使用可能な値は、`offline`、`online` です。</span><span class="sxs-lookup"><span data-stu-id="f2a48-200">Possible values are: `offline`, `online`.</span></span>|
|<span data-ttu-id="f2a48-201">packageIdentityName</span><span class="sxs-lookup"><span data-stu-id="f2a48-201">packageIdentityName</span></span>|<span data-ttu-id="f2a48-202">String</span><span class="sxs-lookup"><span data-stu-id="f2a48-202">String</span></span>|<span data-ttu-id="f2a48-203">アプリ パッケージの識別子</span><span class="sxs-lookup"><span data-stu-id="f2a48-203">The app package identifier</span></span>|



## <a name="response"></a><span data-ttu-id="f2a48-204">応答</span><span class="sxs-lookup"><span data-stu-id="f2a48-204">Response</span></span>
<span data-ttu-id="f2a48-205">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f2a48-205">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessApp](../resources/intune-apps-microsoftstoreforbusinessapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2a48-206">例</span><span class="sxs-lookup"><span data-stu-id="f2a48-206">Example</span></span>

### <a name="request"></a><span data-ttu-id="f2a48-207">要求</span><span class="sxs-lookup"><span data-stu-id="f2a48-207">Request</span></span>
<span data-ttu-id="f2a48-208">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f2a48-208">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 769

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```

### <a name="response"></a><span data-ttu-id="f2a48-209">応答</span><span class="sxs-lookup"><span data-stu-id="f2a48-209">Response</span></span>
<span data-ttu-id="f2a48-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f2a48-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 941

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessApp",
  "id": "f33358bc-58bc-f333-bc58-33f3bc5833f3",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "productKey": "Product Key value",
  "licenseType": "online",
  "packageIdentityName": "Package Identity Name value"
}
```



