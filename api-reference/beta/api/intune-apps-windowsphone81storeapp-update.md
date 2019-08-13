---
title: WindowsPhone81StoreApp の更新
description: WindowsPhone81StoreApp オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c8a85388bce5c9a678b97059e24f7bd83039ae83
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36328677"
---
# <a name="update-windowsphone81storeapp"></a><span data-ttu-id="6c958-103">WindowsPhone81StoreApp の更新</span><span class="sxs-lookup"><span data-stu-id="6c958-103">Update windowsPhone81StoreApp</span></span>

> <span data-ttu-id="6c958-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c958-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c958-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6c958-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c958-106">[WindowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6c958-106">Update the properties of a [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c958-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="6c958-107">Prerequisites</span></span>
<span data-ttu-id="6c958-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6c958-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c958-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6c958-110">Permission type</span></span>|<span data-ttu-id="6c958-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6c958-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c958-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6c958-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6c958-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c958-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6c958-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6c958-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c958-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c958-115">Not supported.</span></span>|
|<span data-ttu-id="6c958-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6c958-116">Application</span></span>|<span data-ttu-id="6c958-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c958-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c958-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6c958-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="6c958-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6c958-119">Request headers</span></span>
|<span data-ttu-id="6c958-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6c958-120">Header</span></span>|<span data-ttu-id="6c958-121">値</span><span class="sxs-lookup"><span data-stu-id="6c958-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c958-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c958-122">Authorization</span></span>|<span data-ttu-id="6c958-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6c958-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c958-124">承諾</span><span class="sxs-lookup"><span data-stu-id="6c958-124">Accept</span></span>|<span data-ttu-id="6c958-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6c958-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c958-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="6c958-126">Request body</span></span>
<span data-ttu-id="6c958-127">要求本文で、 [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6c958-127">In the request body, supply a JSON representation for the [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object.</span></span>

<span data-ttu-id="6c958-128">次の表に、 [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6c958-128">The following table shows the properties that are required when you create the [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md).</span></span>

|<span data-ttu-id="6c958-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c958-129">Property</span></span>|<span data-ttu-id="6c958-130">型</span><span class="sxs-lookup"><span data-stu-id="6c958-130">Type</span></span>|<span data-ttu-id="6c958-131">説明</span><span class="sxs-lookup"><span data-stu-id="6c958-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c958-132">id</span><span class="sxs-lookup"><span data-stu-id="6c958-132">id</span></span>|<span data-ttu-id="6c958-133">文字列</span><span class="sxs-lookup"><span data-stu-id="6c958-133">String</span></span>|<span data-ttu-id="6c958-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6c958-134">Key of the entity.</span></span> <span data-ttu-id="6c958-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6c958-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6c958-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6c958-136">displayName</span></span>|<span data-ttu-id="6c958-137">文字列</span><span class="sxs-lookup"><span data-stu-id="6c958-137">String</span></span>|<span data-ttu-id="6c958-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="6c958-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="6c958-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6c958-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6c958-140">description</span><span class="sxs-lookup"><span data-stu-id="6c958-140">description</span></span>|<span data-ttu-id="6c958-141">String</span><span class="sxs-lookup"><span data-stu-id="6c958-141">String</span></span>|<span data-ttu-id="6c958-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="6c958-142">The description of the app.</span></span> <span data-ttu-id="6c958-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6c958-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6c958-144">publisher</span><span class="sxs-lookup"><span data-stu-id="6c958-144">publisher</span></span>|<span data-ttu-id="6c958-145">String</span><span class="sxs-lookup"><span data-stu-id="6c958-145">String</span></span>|<span data-ttu-id="6c958-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="6c958-146">The publisher of the app.</span></span> <span data-ttu-id="6c958-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6c958-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6c958-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="6c958-148">largeIcon</span></span>|[<span data-ttu-id="6c958-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="6c958-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="6c958-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="6c958-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="6c958-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6c958-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6c958-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6c958-152">createdDateTime</span></span>|<span data-ttu-id="6c958-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c958-153">DateTimeOffset</span></span>|<span data-ttu-id="6c958-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="6c958-154">The date and time the app was created.</span></span> <span data-ttu-id="6c958-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6c958-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6c958-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6c958-156">lastModifiedDateTime</span></span>|<span data-ttu-id="6c958-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6c958-157">DateTimeOffset</span></span>|<span data-ttu-id="6c958-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="6c958-158">The date and time the app was last modified.</span></span> <span data-ttu-id="6c958-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6c958-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6c958-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="6c958-160">isFeatured</span></span>|<span data-ttu-id="6c958-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c958-161">Boolean</span></span>|<span data-ttu-id="6c958-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6c958-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6c958-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="6c958-163">privacyInformationUrl</span></span>|<span data-ttu-id="6c958-164">String</span><span class="sxs-lookup"><span data-stu-id="6c958-164">String</span></span>|<span data-ttu-id="6c958-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="6c958-165">The privacy statement Url.</span></span> <span data-ttu-id="6c958-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6c958-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6c958-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="6c958-167">informationUrl</span></span>|<span data-ttu-id="6c958-168">String</span><span class="sxs-lookup"><span data-stu-id="6c958-168">String</span></span>|<span data-ttu-id="6c958-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="6c958-169">The more information Url.</span></span> <span data-ttu-id="6c958-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6c958-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6c958-171">owner</span><span class="sxs-lookup"><span data-stu-id="6c958-171">owner</span></span>|<span data-ttu-id="6c958-172">String</span><span class="sxs-lookup"><span data-stu-id="6c958-172">String</span></span>|<span data-ttu-id="6c958-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="6c958-173">The owner of the app.</span></span> <span data-ttu-id="6c958-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6c958-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6c958-175">developer</span><span class="sxs-lookup"><span data-stu-id="6c958-175">developer</span></span>|<span data-ttu-id="6c958-176">String</span><span class="sxs-lookup"><span data-stu-id="6c958-176">String</span></span>|<span data-ttu-id="6c958-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="6c958-177">The developer of the app.</span></span> <span data-ttu-id="6c958-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6c958-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6c958-179">notes</span><span class="sxs-lookup"><span data-stu-id="6c958-179">notes</span></span>|<span data-ttu-id="6c958-180">String</span><span class="sxs-lookup"><span data-stu-id="6c958-180">String</span></span>|<span data-ttu-id="6c958-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="6c958-181">Notes for the app.</span></span> <span data-ttu-id="6c958-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6c958-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6c958-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="6c958-183">uploadState</span></span>|<span data-ttu-id="6c958-184">Int32</span><span class="sxs-lookup"><span data-stu-id="6c958-184">Int32</span></span>|<span data-ttu-id="6c958-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="6c958-185">The upload state.</span></span> <span data-ttu-id="6c958-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6c958-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6c958-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="6c958-187">publishingState</span></span>|[<span data-ttu-id="6c958-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="6c958-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="6c958-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="6c958-189">The publishing state for the app.</span></span> <span data-ttu-id="6c958-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="6c958-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="6c958-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="6c958-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="6c958-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="6c958-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="6c958-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="6c958-193">isAssigned</span></span>|<span data-ttu-id="6c958-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c958-194">Boolean</span></span>|<span data-ttu-id="6c958-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="6c958-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="6c958-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6c958-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6c958-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6c958-197">roleScopeTagIds</span></span>|<span data-ttu-id="6c958-198">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="6c958-198">String collection</span></span>|<span data-ttu-id="6c958-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="6c958-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="6c958-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6c958-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6c958-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="6c958-201">dependentAppCount</span></span>|<span data-ttu-id="6c958-202">Int32</span><span class="sxs-lookup"><span data-stu-id="6c958-202">Int32</span></span>|<span data-ttu-id="6c958-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="6c958-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="6c958-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6c958-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="6c958-205">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="6c958-205">appStoreUrl</span></span>|<span data-ttu-id="6c958-206">String</span><span class="sxs-lookup"><span data-stu-id="6c958-206">String</span></span>|<span data-ttu-id="6c958-207">Windows Phone 8.1 アプリストアの URL。</span><span class="sxs-lookup"><span data-stu-id="6c958-207">The Windows Phone 8.1 app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="6c958-208">応答</span><span class="sxs-lookup"><span data-stu-id="6c958-208">Response</span></span>
<span data-ttu-id="6c958-209">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6c958-209">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c958-210">例</span><span class="sxs-lookup"><span data-stu-id="6c958-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c958-211">要求</span><span class="sxs-lookup"><span data-stu-id="6c958-211">Request</span></span>
<span data-ttu-id="6c958-212">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6c958-212">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 775

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
  "dependentAppCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="6c958-213">応答</span><span class="sxs-lookup"><span data-stu-id="6c958-213">Response</span></span>
<span data-ttu-id="6c958-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6c958-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 947

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
  "dependentAppCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```






