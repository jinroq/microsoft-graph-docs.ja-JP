---
title: windowsPhone81StoreApp を作成する
description: 新しい windowsPhone81StoreApp オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f825a8504b8b0cedfd8ffd4e482f29f0dbc38dc
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30974315"
---
# <a name="create-windowsphone81storeapp"></a><span data-ttu-id="0f665-103">windowsPhone81StoreApp を作成する</span><span class="sxs-lookup"><span data-stu-id="0f665-103">Create windowsPhone81StoreApp</span></span>

> <span data-ttu-id="0f665-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0f665-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f665-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0f665-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f665-106">新しい[windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0f665-106">Create a new [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f665-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="0f665-107">Prerequisites</span></span>
<span data-ttu-id="0f665-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0f665-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f665-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0f665-110">Permission type</span></span>|<span data-ttu-id="0f665-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0f665-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f665-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0f665-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0f665-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f665-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0f665-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0f665-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f665-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0f665-115">Not supported.</span></span>|
|<span data-ttu-id="0f665-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0f665-116">Application</span></span>|<span data-ttu-id="0f665-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0f665-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f665-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0f665-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="0f665-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0f665-119">Request headers</span></span>
|<span data-ttu-id="0f665-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0f665-120">Header</span></span>|<span data-ttu-id="0f665-121">値</span><span class="sxs-lookup"><span data-stu-id="0f665-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f665-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f665-122">Authorization</span></span>|<span data-ttu-id="0f665-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0f665-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f665-124">承諾</span><span class="sxs-lookup"><span data-stu-id="0f665-124">Accept</span></span>|<span data-ttu-id="0f665-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0f665-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f665-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0f665-126">Request body</span></span>
<span data-ttu-id="0f665-127">要求本文で、windowsPhone81StoreApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0f665-127">In the request body, supply a JSON representation for the windowsPhone81StoreApp object.</span></span>

<span data-ttu-id="0f665-128">次の表に、windowsPhone81StoreApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0f665-128">The following table shows the properties that are required when you create the windowsPhone81StoreApp.</span></span>

|<span data-ttu-id="0f665-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0f665-129">Property</span></span>|<span data-ttu-id="0f665-130">型</span><span class="sxs-lookup"><span data-stu-id="0f665-130">Type</span></span>|<span data-ttu-id="0f665-131">説明</span><span class="sxs-lookup"><span data-stu-id="0f665-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f665-132">id</span><span class="sxs-lookup"><span data-stu-id="0f665-132">id</span></span>|<span data-ttu-id="0f665-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="0f665-133">String</span></span>|<span data-ttu-id="0f665-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0f665-134">Key of the entity.</span></span> <span data-ttu-id="0f665-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0f665-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f665-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0f665-136">displayName</span></span>|<span data-ttu-id="0f665-137">String</span><span class="sxs-lookup"><span data-stu-id="0f665-137">String</span></span>|<span data-ttu-id="0f665-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="0f665-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="0f665-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0f665-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f665-140">description</span><span class="sxs-lookup"><span data-stu-id="0f665-140">description</span></span>|<span data-ttu-id="0f665-141">String</span><span class="sxs-lookup"><span data-stu-id="0f665-141">String</span></span>|<span data-ttu-id="0f665-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="0f665-142">The description of the app.</span></span> <span data-ttu-id="0f665-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0f665-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f665-144">publisher</span><span class="sxs-lookup"><span data-stu-id="0f665-144">publisher</span></span>|<span data-ttu-id="0f665-145">String</span><span class="sxs-lookup"><span data-stu-id="0f665-145">String</span></span>|<span data-ttu-id="0f665-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="0f665-146">The publisher of the app.</span></span> <span data-ttu-id="0f665-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0f665-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f665-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="0f665-148">largeIcon</span></span>|[<span data-ttu-id="0f665-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0f665-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0f665-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="0f665-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="0f665-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0f665-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f665-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0f665-152">createdDateTime</span></span>|<span data-ttu-id="0f665-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f665-153">DateTimeOffset</span></span>|<span data-ttu-id="0f665-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="0f665-154">The date and time the app was created.</span></span> <span data-ttu-id="0f665-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0f665-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f665-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f665-156">lastModifiedDateTime</span></span>|<span data-ttu-id="0f665-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f665-157">DateTimeOffset</span></span>|<span data-ttu-id="0f665-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="0f665-158">The date and time the app was last modified.</span></span> <span data-ttu-id="0f665-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0f665-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f665-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="0f665-160">isFeatured</span></span>|<span data-ttu-id="0f665-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f665-161">Boolean</span></span>|<span data-ttu-id="0f665-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0f665-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f665-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="0f665-163">privacyInformationUrl</span></span>|<span data-ttu-id="0f665-164">String</span><span class="sxs-lookup"><span data-stu-id="0f665-164">String</span></span>|<span data-ttu-id="0f665-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="0f665-165">The privacy statement Url.</span></span> <span data-ttu-id="0f665-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0f665-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f665-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="0f665-167">informationUrl</span></span>|<span data-ttu-id="0f665-168">String</span><span class="sxs-lookup"><span data-stu-id="0f665-168">String</span></span>|<span data-ttu-id="0f665-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="0f665-169">The more information Url.</span></span> <span data-ttu-id="0f665-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0f665-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f665-171">owner</span><span class="sxs-lookup"><span data-stu-id="0f665-171">owner</span></span>|<span data-ttu-id="0f665-172">String</span><span class="sxs-lookup"><span data-stu-id="0f665-172">String</span></span>|<span data-ttu-id="0f665-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="0f665-173">The owner of the app.</span></span> <span data-ttu-id="0f665-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0f665-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f665-175">developer</span><span class="sxs-lookup"><span data-stu-id="0f665-175">developer</span></span>|<span data-ttu-id="0f665-176">String</span><span class="sxs-lookup"><span data-stu-id="0f665-176">String</span></span>|<span data-ttu-id="0f665-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="0f665-177">The developer of the app.</span></span> <span data-ttu-id="0f665-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0f665-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f665-179">notes</span><span class="sxs-lookup"><span data-stu-id="0f665-179">notes</span></span>|<span data-ttu-id="0f665-180">String</span><span class="sxs-lookup"><span data-stu-id="0f665-180">String</span></span>|<span data-ttu-id="0f665-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="0f665-181">Notes for the app.</span></span> <span data-ttu-id="0f665-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0f665-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f665-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="0f665-183">uploadState</span></span>|<span data-ttu-id="0f665-184">Int32</span><span class="sxs-lookup"><span data-stu-id="0f665-184">Int32</span></span>|<span data-ttu-id="0f665-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="0f665-185">The upload state.</span></span> <span data-ttu-id="0f665-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0f665-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f665-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="0f665-187">publishingState</span></span>|[<span data-ttu-id="0f665-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="0f665-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="0f665-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="0f665-189">The publishing state for the app.</span></span> <span data-ttu-id="0f665-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="0f665-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="0f665-191">[mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="0f665-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="0f665-192">使用可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="0f665-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="0f665-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="0f665-193">isAssigned</span></span>|<span data-ttu-id="0f665-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f665-194">Boolean</span></span>|<span data-ttu-id="0f665-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="0f665-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="0f665-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0f665-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f665-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0f665-197">roleScopeTagIds</span></span>|<span data-ttu-id="0f665-198">String collection</span><span class="sxs-lookup"><span data-stu-id="0f665-198">String collection</span></span>|<span data-ttu-id="0f665-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="0f665-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="0f665-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0f665-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0f665-201">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="0f665-201">appStoreUrl</span></span>|<span data-ttu-id="0f665-202">String</span><span class="sxs-lookup"><span data-stu-id="0f665-202">String</span></span>|<span data-ttu-id="0f665-203">Windows Phone 8.1 アプリストアの URL。</span><span class="sxs-lookup"><span data-stu-id="0f665-203">The Windows Phone 8.1 app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="0f665-204">応答</span><span class="sxs-lookup"><span data-stu-id="0f665-204">Response</span></span>
<span data-ttu-id="0f665-205">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0f665-205">If successful, this method returns a `201 Created` response code and a [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f665-206">例</span><span class="sxs-lookup"><span data-stu-id="0f665-206">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f665-207">要求</span><span class="sxs-lookup"><span data-stu-id="0f665-207">Request</span></span>
<span data-ttu-id="0f665-208">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0f665-208">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 748

{
  "@odata.type": "#microsoft.graph.windowsPhone81StoreApp",
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
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="0f665-209">応答</span><span class="sxs-lookup"><span data-stu-id="0f665-209">Response</span></span>
<span data-ttu-id="0f665-p118">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0f665-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 920

{
  "@odata.type": "#microsoft.graph.windowsPhone81StoreApp",
  "id": "f68ce6a1-e6a1-f68c-a1e6-8cf6a1e68cf6",
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
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```




