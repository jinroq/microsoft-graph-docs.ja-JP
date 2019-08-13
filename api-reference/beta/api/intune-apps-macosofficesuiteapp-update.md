---
title: macOSOfficeSuiteApp の更新
description: macOSOfficeSuiteApp オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 50d680eef88ec6ecb95795d898822e5c5dc8f7bd
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36336979"
---
# <a name="update-macosofficesuiteapp"></a><span data-ttu-id="27905-103">macOSOfficeSuiteApp の更新</span><span class="sxs-lookup"><span data-stu-id="27905-103">Update macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="27905-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27905-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27905-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="27905-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27905-106">[macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="27905-106">Update the properties of a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27905-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="27905-107">Prerequisites</span></span>
<span data-ttu-id="27905-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="27905-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27905-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="27905-110">Permission type</span></span>|<span data-ttu-id="27905-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="27905-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27905-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="27905-112">Delegated (work or school account)</span></span>|<span data-ttu-id="27905-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27905-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="27905-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="27905-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27905-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27905-115">Not supported.</span></span>|
|<span data-ttu-id="27905-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="27905-116">Application</span></span>|<span data-ttu-id="27905-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27905-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="27905-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="27905-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="27905-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="27905-119">Request headers</span></span>
|<span data-ttu-id="27905-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="27905-120">Header</span></span>|<span data-ttu-id="27905-121">値</span><span class="sxs-lookup"><span data-stu-id="27905-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27905-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="27905-122">Authorization</span></span>|<span data-ttu-id="27905-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="27905-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27905-124">承諾</span><span class="sxs-lookup"><span data-stu-id="27905-124">Accept</span></span>|<span data-ttu-id="27905-125">application/json</span><span class="sxs-lookup"><span data-stu-id="27905-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27905-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="27905-126">Request body</span></span>
<span data-ttu-id="27905-127">要求本文で、[macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="27905-127">In the request body, supply a JSON representation for the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

<span data-ttu-id="27905-128">次の表に、[macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="27905-128">The following table shows the properties that are required when you create the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span></span>

|<span data-ttu-id="27905-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="27905-129">Property</span></span>|<span data-ttu-id="27905-130">型</span><span class="sxs-lookup"><span data-stu-id="27905-130">Type</span></span>|<span data-ttu-id="27905-131">説明</span><span class="sxs-lookup"><span data-stu-id="27905-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27905-132">id</span><span class="sxs-lookup"><span data-stu-id="27905-132">id</span></span>|<span data-ttu-id="27905-133">文字列</span><span class="sxs-lookup"><span data-stu-id="27905-133">String</span></span>|<span data-ttu-id="27905-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="27905-134">Key of the entity.</span></span> <span data-ttu-id="27905-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27905-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27905-136">displayName</span><span class="sxs-lookup"><span data-stu-id="27905-136">displayName</span></span>|<span data-ttu-id="27905-137">文字列</span><span class="sxs-lookup"><span data-stu-id="27905-137">String</span></span>|<span data-ttu-id="27905-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="27905-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="27905-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27905-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27905-140">description</span><span class="sxs-lookup"><span data-stu-id="27905-140">description</span></span>|<span data-ttu-id="27905-141">String</span><span class="sxs-lookup"><span data-stu-id="27905-141">String</span></span>|<span data-ttu-id="27905-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="27905-142">The description of the app.</span></span> <span data-ttu-id="27905-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27905-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27905-144">publisher</span><span class="sxs-lookup"><span data-stu-id="27905-144">publisher</span></span>|<span data-ttu-id="27905-145">String</span><span class="sxs-lookup"><span data-stu-id="27905-145">String</span></span>|<span data-ttu-id="27905-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="27905-146">The publisher of the app.</span></span> <span data-ttu-id="27905-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27905-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27905-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="27905-148">largeIcon</span></span>|[<span data-ttu-id="27905-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="27905-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="27905-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="27905-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="27905-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27905-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27905-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="27905-152">createdDateTime</span></span>|<span data-ttu-id="27905-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27905-153">DateTimeOffset</span></span>|<span data-ttu-id="27905-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="27905-154">The date and time the app was created.</span></span> <span data-ttu-id="27905-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27905-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27905-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="27905-156">lastModifiedDateTime</span></span>|<span data-ttu-id="27905-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27905-157">DateTimeOffset</span></span>|<span data-ttu-id="27905-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="27905-158">The date and time the app was last modified.</span></span> <span data-ttu-id="27905-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27905-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27905-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="27905-160">isFeatured</span></span>|<span data-ttu-id="27905-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="27905-161">Boolean</span></span>|<span data-ttu-id="27905-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27905-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27905-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="27905-163">privacyInformationUrl</span></span>|<span data-ttu-id="27905-164">String</span><span class="sxs-lookup"><span data-stu-id="27905-164">String</span></span>|<span data-ttu-id="27905-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="27905-165">The privacy statement Url.</span></span> <span data-ttu-id="27905-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27905-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27905-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="27905-167">informationUrl</span></span>|<span data-ttu-id="27905-168">String</span><span class="sxs-lookup"><span data-stu-id="27905-168">String</span></span>|<span data-ttu-id="27905-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="27905-169">The more information Url.</span></span> <span data-ttu-id="27905-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27905-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27905-171">owner</span><span class="sxs-lookup"><span data-stu-id="27905-171">owner</span></span>|<span data-ttu-id="27905-172">String</span><span class="sxs-lookup"><span data-stu-id="27905-172">String</span></span>|<span data-ttu-id="27905-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="27905-173">The owner of the app.</span></span> <span data-ttu-id="27905-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27905-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27905-175">developer</span><span class="sxs-lookup"><span data-stu-id="27905-175">developer</span></span>|<span data-ttu-id="27905-176">String</span><span class="sxs-lookup"><span data-stu-id="27905-176">String</span></span>|<span data-ttu-id="27905-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="27905-177">The developer of the app.</span></span> <span data-ttu-id="27905-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27905-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27905-179">notes</span><span class="sxs-lookup"><span data-stu-id="27905-179">notes</span></span>|<span data-ttu-id="27905-180">String</span><span class="sxs-lookup"><span data-stu-id="27905-180">String</span></span>|<span data-ttu-id="27905-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="27905-181">Notes for the app.</span></span> <span data-ttu-id="27905-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27905-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27905-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="27905-183">uploadState</span></span>|<span data-ttu-id="27905-184">Int32</span><span class="sxs-lookup"><span data-stu-id="27905-184">Int32</span></span>|<span data-ttu-id="27905-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="27905-185">The upload state.</span></span> <span data-ttu-id="27905-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27905-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27905-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="27905-187">publishingState</span></span>|[<span data-ttu-id="27905-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="27905-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="27905-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="27905-189">The publishing state for the app.</span></span> <span data-ttu-id="27905-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="27905-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="27905-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="27905-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="27905-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="27905-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="27905-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="27905-193">isAssigned</span></span>|<span data-ttu-id="27905-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="27905-194">Boolean</span></span>|<span data-ttu-id="27905-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="27905-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="27905-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27905-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27905-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="27905-197">roleScopeTagIds</span></span>|<span data-ttu-id="27905-198">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="27905-198">String collection</span></span>|<span data-ttu-id="27905-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="27905-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="27905-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27905-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27905-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="27905-201">dependentAppCount</span></span>|<span data-ttu-id="27905-202">Int32</span><span class="sxs-lookup"><span data-stu-id="27905-202">Int32</span></span>|<span data-ttu-id="27905-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="27905-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="27905-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27905-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="27905-205">応答</span><span class="sxs-lookup"><span data-stu-id="27905-205">Response</span></span>
<span data-ttu-id="27905-206">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="27905-206">If successful, this method returns a `200 OK` response code and an updated [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27905-207">例</span><span class="sxs-lookup"><span data-stu-id="27905-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="27905-208">要求</span><span class="sxs-lookup"><span data-stu-id="27905-208">Request</span></span>
<span data-ttu-id="27905-209">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="27905-209">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 718

{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
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
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1
}
```

### <a name="response"></a><span data-ttu-id="27905-210">応答</span><span class="sxs-lookup"><span data-stu-id="27905-210">Response</span></span>
<span data-ttu-id="27905-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="27905-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 890

{
  "@odata.type": "#microsoft.graph.macOSOfficeSuiteApp",
  "id": "bf39e35d-e35d-bf39-5de3-39bf5de339bf",
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
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "dependentAppCount": 1
}
```






