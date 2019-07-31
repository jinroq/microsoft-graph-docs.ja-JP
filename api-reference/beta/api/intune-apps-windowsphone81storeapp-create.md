---
title: WindowsPhone81StoreApp を作成する
description: 新しい windowsPhone81StoreApp オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 955720103f6ba3843f8363cd16a835421e1e6e69
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35959916"
---
# <a name="create-windowsphone81storeapp"></a><span data-ttu-id="df3c6-103">WindowsPhone81StoreApp を作成する</span><span class="sxs-lookup"><span data-stu-id="df3c6-103">Create windowsPhone81StoreApp</span></span>

> <span data-ttu-id="df3c6-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="df3c6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df3c6-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="df3c6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df3c6-106">新しい[windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="df3c6-106">Create a new [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df3c6-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="df3c6-107">Prerequisites</span></span>
<span data-ttu-id="df3c6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="df3c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df3c6-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="df3c6-110">Permission type</span></span>|<span data-ttu-id="df3c6-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="df3c6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df3c6-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="df3c6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="df3c6-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df3c6-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="df3c6-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="df3c6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df3c6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="df3c6-115">Not supported.</span></span>|
|<span data-ttu-id="df3c6-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="df3c6-116">Application</span></span>|<span data-ttu-id="df3c6-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="df3c6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df3c6-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="df3c6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="df3c6-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="df3c6-119">Request headers</span></span>
|<span data-ttu-id="df3c6-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="df3c6-120">Header</span></span>|<span data-ttu-id="df3c6-121">値</span><span class="sxs-lookup"><span data-stu-id="df3c6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df3c6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="df3c6-122">Authorization</span></span>|<span data-ttu-id="df3c6-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="df3c6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df3c6-124">承諾</span><span class="sxs-lookup"><span data-stu-id="df3c6-124">Accept</span></span>|<span data-ttu-id="df3c6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="df3c6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df3c6-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="df3c6-126">Request body</span></span>
<span data-ttu-id="df3c6-127">要求本文で、windowsPhone81StoreApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="df3c6-127">In the request body, supply a JSON representation for the windowsPhone81StoreApp object.</span></span>

<span data-ttu-id="df3c6-128">次の表に、windowsPhone81StoreApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="df3c6-128">The following table shows the properties that are required when you create the windowsPhone81StoreApp.</span></span>

|<span data-ttu-id="df3c6-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="df3c6-129">Property</span></span>|<span data-ttu-id="df3c6-130">型</span><span class="sxs-lookup"><span data-stu-id="df3c6-130">Type</span></span>|<span data-ttu-id="df3c6-131">説明</span><span class="sxs-lookup"><span data-stu-id="df3c6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df3c6-132">id</span><span class="sxs-lookup"><span data-stu-id="df3c6-132">id</span></span>|<span data-ttu-id="df3c6-133">文字列</span><span class="sxs-lookup"><span data-stu-id="df3c6-133">String</span></span>|<span data-ttu-id="df3c6-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="df3c6-134">Key of the entity.</span></span> <span data-ttu-id="df3c6-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df3c6-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="df3c6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="df3c6-136">displayName</span></span>|<span data-ttu-id="df3c6-137">文字列</span><span class="sxs-lookup"><span data-stu-id="df3c6-137">String</span></span>|<span data-ttu-id="df3c6-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="df3c6-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="df3c6-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df3c6-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="df3c6-140">description</span><span class="sxs-lookup"><span data-stu-id="df3c6-140">description</span></span>|<span data-ttu-id="df3c6-141">String</span><span class="sxs-lookup"><span data-stu-id="df3c6-141">String</span></span>|<span data-ttu-id="df3c6-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="df3c6-142">The description of the app.</span></span> <span data-ttu-id="df3c6-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df3c6-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="df3c6-144">publisher</span><span class="sxs-lookup"><span data-stu-id="df3c6-144">publisher</span></span>|<span data-ttu-id="df3c6-145">String</span><span class="sxs-lookup"><span data-stu-id="df3c6-145">String</span></span>|<span data-ttu-id="df3c6-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="df3c6-146">The publisher of the app.</span></span> <span data-ttu-id="df3c6-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df3c6-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="df3c6-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="df3c6-148">largeIcon</span></span>|[<span data-ttu-id="df3c6-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="df3c6-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="df3c6-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="df3c6-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="df3c6-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df3c6-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="df3c6-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="df3c6-152">createdDateTime</span></span>|<span data-ttu-id="df3c6-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df3c6-153">DateTimeOffset</span></span>|<span data-ttu-id="df3c6-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="df3c6-154">The date and time the app was created.</span></span> <span data-ttu-id="df3c6-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df3c6-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="df3c6-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="df3c6-156">lastModifiedDateTime</span></span>|<span data-ttu-id="df3c6-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df3c6-157">DateTimeOffset</span></span>|<span data-ttu-id="df3c6-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="df3c6-158">The date and time the app was last modified.</span></span> <span data-ttu-id="df3c6-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df3c6-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="df3c6-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="df3c6-160">isFeatured</span></span>|<span data-ttu-id="df3c6-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="df3c6-161">Boolean</span></span>|<span data-ttu-id="df3c6-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df3c6-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="df3c6-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="df3c6-163">privacyInformationUrl</span></span>|<span data-ttu-id="df3c6-164">String</span><span class="sxs-lookup"><span data-stu-id="df3c6-164">String</span></span>|<span data-ttu-id="df3c6-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="df3c6-165">The privacy statement Url.</span></span> <span data-ttu-id="df3c6-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df3c6-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="df3c6-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="df3c6-167">informationUrl</span></span>|<span data-ttu-id="df3c6-168">String</span><span class="sxs-lookup"><span data-stu-id="df3c6-168">String</span></span>|<span data-ttu-id="df3c6-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="df3c6-169">The more information Url.</span></span> <span data-ttu-id="df3c6-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df3c6-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="df3c6-171">owner</span><span class="sxs-lookup"><span data-stu-id="df3c6-171">owner</span></span>|<span data-ttu-id="df3c6-172">String</span><span class="sxs-lookup"><span data-stu-id="df3c6-172">String</span></span>|<span data-ttu-id="df3c6-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="df3c6-173">The owner of the app.</span></span> <span data-ttu-id="df3c6-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df3c6-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="df3c6-175">developer</span><span class="sxs-lookup"><span data-stu-id="df3c6-175">developer</span></span>|<span data-ttu-id="df3c6-176">String</span><span class="sxs-lookup"><span data-stu-id="df3c6-176">String</span></span>|<span data-ttu-id="df3c6-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="df3c6-177">The developer of the app.</span></span> <span data-ttu-id="df3c6-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df3c6-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="df3c6-179">notes</span><span class="sxs-lookup"><span data-stu-id="df3c6-179">notes</span></span>|<span data-ttu-id="df3c6-180">String</span><span class="sxs-lookup"><span data-stu-id="df3c6-180">String</span></span>|<span data-ttu-id="df3c6-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="df3c6-181">Notes for the app.</span></span> <span data-ttu-id="df3c6-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df3c6-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="df3c6-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="df3c6-183">uploadState</span></span>|<span data-ttu-id="df3c6-184">Int32</span><span class="sxs-lookup"><span data-stu-id="df3c6-184">Int32</span></span>|<span data-ttu-id="df3c6-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="df3c6-185">The upload state.</span></span> <span data-ttu-id="df3c6-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df3c6-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="df3c6-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="df3c6-187">publishingState</span></span>|[<span data-ttu-id="df3c6-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="df3c6-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="df3c6-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="df3c6-189">The publishing state for the app.</span></span> <span data-ttu-id="df3c6-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="df3c6-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="df3c6-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="df3c6-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="df3c6-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="df3c6-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="df3c6-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="df3c6-193">isAssigned</span></span>|<span data-ttu-id="df3c6-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="df3c6-194">Boolean</span></span>|<span data-ttu-id="df3c6-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="df3c6-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="df3c6-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df3c6-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="df3c6-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="df3c6-197">roleScopeTagIds</span></span>|<span data-ttu-id="df3c6-198">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="df3c6-198">String collection</span></span>|<span data-ttu-id="df3c6-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="df3c6-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="df3c6-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df3c6-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="df3c6-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="df3c6-201">dependentAppCount</span></span>|<span data-ttu-id="df3c6-202">Int32</span><span class="sxs-lookup"><span data-stu-id="df3c6-202">Int32</span></span>|<span data-ttu-id="df3c6-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="df3c6-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="df3c6-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="df3c6-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="df3c6-205">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="df3c6-205">appStoreUrl</span></span>|<span data-ttu-id="df3c6-206">String</span><span class="sxs-lookup"><span data-stu-id="df3c6-206">String</span></span>|<span data-ttu-id="df3c6-207">Windows Phone 8.1 アプリストアの URL。</span><span class="sxs-lookup"><span data-stu-id="df3c6-207">The Windows Phone 8.1 app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="df3c6-208">応答</span><span class="sxs-lookup"><span data-stu-id="df3c6-208">Response</span></span>
<span data-ttu-id="df3c6-209">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="df3c6-209">If successful, this method returns a `201 Created` response code and a [windowsPhone81StoreApp](../resources/intune-apps-windowsphone81storeapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df3c6-210">例</span><span class="sxs-lookup"><span data-stu-id="df3c6-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="df3c6-211">要求</span><span class="sxs-lookup"><span data-stu-id="df3c6-211">Request</span></span>
<span data-ttu-id="df3c6-212">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="df3c6-212">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="df3c6-213">応答</span><span class="sxs-lookup"><span data-stu-id="df3c6-213">Response</span></span>
<span data-ttu-id="df3c6-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="df3c6-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





