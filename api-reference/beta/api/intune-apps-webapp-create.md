---
title: webApp の作成
description: 新しい webApp オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d454ad69737ed870dbd8658f2c0fd6e1be2edc3e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36328873"
---
# <a name="create-webapp"></a><span data-ttu-id="77acc-103">webApp の作成</span><span class="sxs-lookup"><span data-stu-id="77acc-103">Create webApp</span></span>

> <span data-ttu-id="77acc-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77acc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77acc-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="77acc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77acc-106">新しい [webApp](../resources/intune-apps-webapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="77acc-106">Create a new [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77acc-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="77acc-107">Prerequisites</span></span>
<span data-ttu-id="77acc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="77acc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77acc-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="77acc-110">Permission type</span></span>|<span data-ttu-id="77acc-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="77acc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77acc-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="77acc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="77acc-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77acc-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="77acc-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="77acc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77acc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77acc-115">Not supported.</span></span>|
|<span data-ttu-id="77acc-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="77acc-116">Application</span></span>|<span data-ttu-id="77acc-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77acc-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="77acc-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="77acc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="77acc-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="77acc-119">Request headers</span></span>
|<span data-ttu-id="77acc-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="77acc-120">Header</span></span>|<span data-ttu-id="77acc-121">値</span><span class="sxs-lookup"><span data-stu-id="77acc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77acc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="77acc-122">Authorization</span></span>|<span data-ttu-id="77acc-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="77acc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77acc-124">承諾</span><span class="sxs-lookup"><span data-stu-id="77acc-124">Accept</span></span>|<span data-ttu-id="77acc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="77acc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77acc-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="77acc-126">Request body</span></span>
<span data-ttu-id="77acc-127">要求本文で、webApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="77acc-127">In the request body, supply a JSON representation for the webApp object.</span></span>

<span data-ttu-id="77acc-128">次の表に、webApp 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="77acc-128">The following table shows the properties that are required when you create the webApp.</span></span>

|<span data-ttu-id="77acc-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="77acc-129">Property</span></span>|<span data-ttu-id="77acc-130">型</span><span class="sxs-lookup"><span data-stu-id="77acc-130">Type</span></span>|<span data-ttu-id="77acc-131">説明</span><span class="sxs-lookup"><span data-stu-id="77acc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77acc-132">id</span><span class="sxs-lookup"><span data-stu-id="77acc-132">id</span></span>|<span data-ttu-id="77acc-133">文字列</span><span class="sxs-lookup"><span data-stu-id="77acc-133">String</span></span>|<span data-ttu-id="77acc-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="77acc-134">Key of the entity.</span></span> <span data-ttu-id="77acc-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="77acc-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77acc-136">displayName</span><span class="sxs-lookup"><span data-stu-id="77acc-136">displayName</span></span>|<span data-ttu-id="77acc-137">文字列</span><span class="sxs-lookup"><span data-stu-id="77acc-137">String</span></span>|<span data-ttu-id="77acc-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="77acc-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="77acc-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="77acc-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77acc-140">description</span><span class="sxs-lookup"><span data-stu-id="77acc-140">description</span></span>|<span data-ttu-id="77acc-141">String</span><span class="sxs-lookup"><span data-stu-id="77acc-141">String</span></span>|<span data-ttu-id="77acc-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="77acc-142">The description of the app.</span></span> <span data-ttu-id="77acc-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="77acc-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77acc-144">publisher</span><span class="sxs-lookup"><span data-stu-id="77acc-144">publisher</span></span>|<span data-ttu-id="77acc-145">String</span><span class="sxs-lookup"><span data-stu-id="77acc-145">String</span></span>|<span data-ttu-id="77acc-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="77acc-146">The publisher of the app.</span></span> <span data-ttu-id="77acc-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="77acc-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77acc-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="77acc-148">largeIcon</span></span>|[<span data-ttu-id="77acc-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="77acc-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="77acc-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="77acc-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="77acc-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="77acc-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77acc-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="77acc-152">createdDateTime</span></span>|<span data-ttu-id="77acc-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77acc-153">DateTimeOffset</span></span>|<span data-ttu-id="77acc-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="77acc-154">The date and time the app was created.</span></span> <span data-ttu-id="77acc-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="77acc-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77acc-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="77acc-156">lastModifiedDateTime</span></span>|<span data-ttu-id="77acc-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77acc-157">DateTimeOffset</span></span>|<span data-ttu-id="77acc-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="77acc-158">The date and time the app was last modified.</span></span> <span data-ttu-id="77acc-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="77acc-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77acc-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="77acc-160">isFeatured</span></span>|<span data-ttu-id="77acc-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="77acc-161">Boolean</span></span>|<span data-ttu-id="77acc-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="77acc-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77acc-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="77acc-163">privacyInformationUrl</span></span>|<span data-ttu-id="77acc-164">String</span><span class="sxs-lookup"><span data-stu-id="77acc-164">String</span></span>|<span data-ttu-id="77acc-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="77acc-165">The privacy statement Url.</span></span> <span data-ttu-id="77acc-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="77acc-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77acc-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="77acc-167">informationUrl</span></span>|<span data-ttu-id="77acc-168">String</span><span class="sxs-lookup"><span data-stu-id="77acc-168">String</span></span>|<span data-ttu-id="77acc-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="77acc-169">The more information Url.</span></span> <span data-ttu-id="77acc-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="77acc-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77acc-171">owner</span><span class="sxs-lookup"><span data-stu-id="77acc-171">owner</span></span>|<span data-ttu-id="77acc-172">String</span><span class="sxs-lookup"><span data-stu-id="77acc-172">String</span></span>|<span data-ttu-id="77acc-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="77acc-173">The owner of the app.</span></span> <span data-ttu-id="77acc-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="77acc-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77acc-175">developer</span><span class="sxs-lookup"><span data-stu-id="77acc-175">developer</span></span>|<span data-ttu-id="77acc-176">String</span><span class="sxs-lookup"><span data-stu-id="77acc-176">String</span></span>|<span data-ttu-id="77acc-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="77acc-177">The developer of the app.</span></span> <span data-ttu-id="77acc-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="77acc-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77acc-179">notes</span><span class="sxs-lookup"><span data-stu-id="77acc-179">notes</span></span>|<span data-ttu-id="77acc-180">String</span><span class="sxs-lookup"><span data-stu-id="77acc-180">String</span></span>|<span data-ttu-id="77acc-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="77acc-181">Notes for the app.</span></span> <span data-ttu-id="77acc-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="77acc-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77acc-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="77acc-183">uploadState</span></span>|<span data-ttu-id="77acc-184">Int32</span><span class="sxs-lookup"><span data-stu-id="77acc-184">Int32</span></span>|<span data-ttu-id="77acc-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="77acc-185">The upload state.</span></span> <span data-ttu-id="77acc-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="77acc-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77acc-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="77acc-187">publishingState</span></span>|[<span data-ttu-id="77acc-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="77acc-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="77acc-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="77acc-189">The publishing state for the app.</span></span> <span data-ttu-id="77acc-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="77acc-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="77acc-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="77acc-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="77acc-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="77acc-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="77acc-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="77acc-193">isAssigned</span></span>|<span data-ttu-id="77acc-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="77acc-194">Boolean</span></span>|<span data-ttu-id="77acc-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="77acc-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="77acc-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="77acc-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77acc-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="77acc-197">roleScopeTagIds</span></span>|<span data-ttu-id="77acc-198">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="77acc-198">String collection</span></span>|<span data-ttu-id="77acc-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="77acc-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="77acc-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="77acc-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77acc-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="77acc-201">dependentAppCount</span></span>|<span data-ttu-id="77acc-202">Int32</span><span class="sxs-lookup"><span data-stu-id="77acc-202">Int32</span></span>|<span data-ttu-id="77acc-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="77acc-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="77acc-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="77acc-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="77acc-205">appUrl</span><span class="sxs-lookup"><span data-stu-id="77acc-205">appUrl</span></span>|<span data-ttu-id="77acc-206">String</span><span class="sxs-lookup"><span data-stu-id="77acc-206">String</span></span>|<span data-ttu-id="77acc-207">Web アプリの URL。</span><span class="sxs-lookup"><span data-stu-id="77acc-207">The web app URL.</span></span>|
|<span data-ttu-id="77acc-208">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="77acc-208">useManagedBrowser</span></span>|<span data-ttu-id="77acc-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="77acc-209">Boolean</span></span>|<span data-ttu-id="77acc-210">管理対象のブラウザーを使用するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="77acc-210">Whether or not to use managed browser.</span></span> <span data-ttu-id="77acc-211">このプロパティは、Android と iOS にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="77acc-211">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="77acc-212">応答</span><span class="sxs-lookup"><span data-stu-id="77acc-212">Response</span></span>
<span data-ttu-id="77acc-213">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [webApp](../resources/intune-apps-webapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="77acc-213">If successful, this method returns a `201 Created` response code and a [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77acc-214">例</span><span class="sxs-lookup"><span data-stu-id="77acc-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="77acc-215">要求</span><span class="sxs-lookup"><span data-stu-id="77acc-215">Request</span></span>
<span data-ttu-id="77acc-216">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="77acc-216">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 779

{
  "@odata.type": "#microsoft.graph.webApp",
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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```

### <a name="response"></a><span data-ttu-id="77acc-217">応答</span><span class="sxs-lookup"><span data-stu-id="77acc-217">Response</span></span>
<span data-ttu-id="77acc-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="77acc-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 951

{
  "@odata.type": "#microsoft.graph.webApp",
  "id": "4bdc5d30-5d30-4bdc-305d-dc4b305ddc4b",
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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```






