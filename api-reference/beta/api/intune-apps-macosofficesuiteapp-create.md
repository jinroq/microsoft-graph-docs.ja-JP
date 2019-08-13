---
title: macOSOfficeSuiteApp の作成
description: 新しい macOSOfficeSuiteApp オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9112d278b1cf560f813a3838b1b796ea4c8bc71c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36330203"
---
# <a name="create-macosofficesuiteapp"></a><span data-ttu-id="61dd4-103">macOSOfficeSuiteApp の作成</span><span class="sxs-lookup"><span data-stu-id="61dd4-103">Create macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="61dd4-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="61dd4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61dd4-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="61dd4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61dd4-106">新しい [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="61dd4-106">Create a new [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="61dd4-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="61dd4-107">Prerequisites</span></span>
<span data-ttu-id="61dd4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="61dd4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61dd4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="61dd4-110">Permission type</span></span>|<span data-ttu-id="61dd4-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="61dd4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61dd4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="61dd4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="61dd4-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61dd4-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="61dd4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="61dd4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61dd4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="61dd4-115">Not supported.</span></span>|
|<span data-ttu-id="61dd4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="61dd4-116">Application</span></span>|<span data-ttu-id="61dd4-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61dd4-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="61dd4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="61dd4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="61dd4-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="61dd4-119">Request headers</span></span>
|<span data-ttu-id="61dd4-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="61dd4-120">Header</span></span>|<span data-ttu-id="61dd4-121">値</span><span class="sxs-lookup"><span data-stu-id="61dd4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61dd4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="61dd4-122">Authorization</span></span>|<span data-ttu-id="61dd4-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="61dd4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61dd4-124">承諾</span><span class="sxs-lookup"><span data-stu-id="61dd4-124">Accept</span></span>|<span data-ttu-id="61dd4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="61dd4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61dd4-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="61dd4-126">Request body</span></span>
<span data-ttu-id="61dd4-127">要求本文で、macOSOfficeSuiteApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="61dd4-127">In the request body, supply a JSON representation for the macOSOfficeSuiteApp object.</span></span>

<span data-ttu-id="61dd4-128">次の表に、macOSOfficeSuiteApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="61dd4-128">The following table shows the properties that are required when you create the macOSOfficeSuiteApp.</span></span>

|<span data-ttu-id="61dd4-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="61dd4-129">Property</span></span>|<span data-ttu-id="61dd4-130">型</span><span class="sxs-lookup"><span data-stu-id="61dd4-130">Type</span></span>|<span data-ttu-id="61dd4-131">説明</span><span class="sxs-lookup"><span data-stu-id="61dd4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61dd4-132">id</span><span class="sxs-lookup"><span data-stu-id="61dd4-132">id</span></span>|<span data-ttu-id="61dd4-133">文字列</span><span class="sxs-lookup"><span data-stu-id="61dd4-133">String</span></span>|<span data-ttu-id="61dd4-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="61dd4-134">Key of the entity.</span></span> <span data-ttu-id="61dd4-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="61dd4-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="61dd4-136">displayName</span><span class="sxs-lookup"><span data-stu-id="61dd4-136">displayName</span></span>|<span data-ttu-id="61dd4-137">文字列</span><span class="sxs-lookup"><span data-stu-id="61dd4-137">String</span></span>|<span data-ttu-id="61dd4-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="61dd4-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="61dd4-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="61dd4-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="61dd4-140">description</span><span class="sxs-lookup"><span data-stu-id="61dd4-140">description</span></span>|<span data-ttu-id="61dd4-141">String</span><span class="sxs-lookup"><span data-stu-id="61dd4-141">String</span></span>|<span data-ttu-id="61dd4-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="61dd4-142">The description of the app.</span></span> <span data-ttu-id="61dd4-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="61dd4-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="61dd4-144">publisher</span><span class="sxs-lookup"><span data-stu-id="61dd4-144">publisher</span></span>|<span data-ttu-id="61dd4-145">String</span><span class="sxs-lookup"><span data-stu-id="61dd4-145">String</span></span>|<span data-ttu-id="61dd4-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="61dd4-146">The publisher of the app.</span></span> <span data-ttu-id="61dd4-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="61dd4-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="61dd4-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="61dd4-148">largeIcon</span></span>|[<span data-ttu-id="61dd4-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="61dd4-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="61dd4-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="61dd4-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="61dd4-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="61dd4-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="61dd4-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="61dd4-152">createdDateTime</span></span>|<span data-ttu-id="61dd4-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61dd4-153">DateTimeOffset</span></span>|<span data-ttu-id="61dd4-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="61dd4-154">The date and time the app was created.</span></span> <span data-ttu-id="61dd4-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="61dd4-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="61dd4-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="61dd4-156">lastModifiedDateTime</span></span>|<span data-ttu-id="61dd4-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="61dd4-157">DateTimeOffset</span></span>|<span data-ttu-id="61dd4-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="61dd4-158">The date and time the app was last modified.</span></span> <span data-ttu-id="61dd4-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="61dd4-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="61dd4-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="61dd4-160">isFeatured</span></span>|<span data-ttu-id="61dd4-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="61dd4-161">Boolean</span></span>|<span data-ttu-id="61dd4-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="61dd4-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="61dd4-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="61dd4-163">privacyInformationUrl</span></span>|<span data-ttu-id="61dd4-164">String</span><span class="sxs-lookup"><span data-stu-id="61dd4-164">String</span></span>|<span data-ttu-id="61dd4-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="61dd4-165">The privacy statement Url.</span></span> <span data-ttu-id="61dd4-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="61dd4-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="61dd4-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="61dd4-167">informationUrl</span></span>|<span data-ttu-id="61dd4-168">String</span><span class="sxs-lookup"><span data-stu-id="61dd4-168">String</span></span>|<span data-ttu-id="61dd4-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="61dd4-169">The more information Url.</span></span> <span data-ttu-id="61dd4-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="61dd4-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="61dd4-171">owner</span><span class="sxs-lookup"><span data-stu-id="61dd4-171">owner</span></span>|<span data-ttu-id="61dd4-172">String</span><span class="sxs-lookup"><span data-stu-id="61dd4-172">String</span></span>|<span data-ttu-id="61dd4-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="61dd4-173">The owner of the app.</span></span> <span data-ttu-id="61dd4-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="61dd4-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="61dd4-175">developer</span><span class="sxs-lookup"><span data-stu-id="61dd4-175">developer</span></span>|<span data-ttu-id="61dd4-176">String</span><span class="sxs-lookup"><span data-stu-id="61dd4-176">String</span></span>|<span data-ttu-id="61dd4-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="61dd4-177">The developer of the app.</span></span> <span data-ttu-id="61dd4-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="61dd4-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="61dd4-179">notes</span><span class="sxs-lookup"><span data-stu-id="61dd4-179">notes</span></span>|<span data-ttu-id="61dd4-180">String</span><span class="sxs-lookup"><span data-stu-id="61dd4-180">String</span></span>|<span data-ttu-id="61dd4-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="61dd4-181">Notes for the app.</span></span> <span data-ttu-id="61dd4-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="61dd4-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="61dd4-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="61dd4-183">uploadState</span></span>|<span data-ttu-id="61dd4-184">Int32</span><span class="sxs-lookup"><span data-stu-id="61dd4-184">Int32</span></span>|<span data-ttu-id="61dd4-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="61dd4-185">The upload state.</span></span> <span data-ttu-id="61dd4-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="61dd4-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="61dd4-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="61dd4-187">publishingState</span></span>|[<span data-ttu-id="61dd4-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="61dd4-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="61dd4-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="61dd4-189">The publishing state for the app.</span></span> <span data-ttu-id="61dd4-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="61dd4-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="61dd4-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="61dd4-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="61dd4-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="61dd4-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="61dd4-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="61dd4-193">isAssigned</span></span>|<span data-ttu-id="61dd4-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="61dd4-194">Boolean</span></span>|<span data-ttu-id="61dd4-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="61dd4-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="61dd4-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="61dd4-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="61dd4-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="61dd4-197">roleScopeTagIds</span></span>|<span data-ttu-id="61dd4-198">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="61dd4-198">String collection</span></span>|<span data-ttu-id="61dd4-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="61dd4-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="61dd4-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="61dd4-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="61dd4-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="61dd4-201">dependentAppCount</span></span>|<span data-ttu-id="61dd4-202">Int32</span><span class="sxs-lookup"><span data-stu-id="61dd4-202">Int32</span></span>|<span data-ttu-id="61dd4-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="61dd4-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="61dd4-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="61dd4-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="61dd4-205">応答</span><span class="sxs-lookup"><span data-stu-id="61dd4-205">Response</span></span>
<span data-ttu-id="61dd4-206">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="61dd4-206">If successful, this method returns a `201 Created` response code and a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61dd4-207">例</span><span class="sxs-lookup"><span data-stu-id="61dd4-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="61dd4-208">要求</span><span class="sxs-lookup"><span data-stu-id="61dd4-208">Request</span></span>
<span data-ttu-id="61dd4-209">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="61dd4-209">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="61dd4-210">応答</span><span class="sxs-lookup"><span data-stu-id="61dd4-210">Response</span></span>
<span data-ttu-id="61dd4-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="61dd4-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






