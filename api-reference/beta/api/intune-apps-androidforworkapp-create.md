---
title: AndroidForWorkApp を作成します。
description: 新しい androidForWorkApp オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: d88346184c1eee294c9cff2abe8274493d57ebef
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340874"
---
# <a name="create-androidforworkapp"></a><span data-ttu-id="eeeb5-103">AndroidForWorkApp を作成します。</span><span class="sxs-lookup"><span data-stu-id="eeeb5-103">Create androidForWorkApp</span></span>

> <span data-ttu-id="eeeb5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="eeeb5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eeeb5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eeeb5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eeeb5-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="eeeb5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eeeb5-107">新しい[androidForWorkApp](../resources/intune-apps-androidforworkapp.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="eeeb5-107">Create a new [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eeeb5-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="eeeb5-108">Prerequisites</span></span>
<span data-ttu-id="eeeb5-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eeeb5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eeeb5-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="eeeb5-111">Permission type</span></span>|<span data-ttu-id="eeeb5-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="eeeb5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eeeb5-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="eeeb5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eeeb5-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eeeb5-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="eeeb5-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="eeeb5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eeeb5-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eeeb5-116">Not supported.</span></span>|
|<span data-ttu-id="eeeb5-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="eeeb5-117">Application</span></span>|<span data-ttu-id="eeeb5-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eeeb5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eeeb5-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="eeeb5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="eeeb5-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eeeb5-120">Request headers</span></span>
|<span data-ttu-id="eeeb5-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eeeb5-121">Header</span></span>|<span data-ttu-id="eeeb5-122">値</span><span class="sxs-lookup"><span data-stu-id="eeeb5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eeeb5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="eeeb5-123">Authorization</span></span>|<span data-ttu-id="eeeb5-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="eeeb5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eeeb5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="eeeb5-125">Accept</span></span>|<span data-ttu-id="eeeb5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eeeb5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eeeb5-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="eeeb5-127">Request body</span></span>
<span data-ttu-id="eeeb5-128">要求の本文に androidForWorkApp オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="eeeb5-128">In the request body, supply a JSON representation for the androidForWorkApp object.</span></span>

<span data-ttu-id="eeeb5-129">次の表は、androidForWorkApp を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="eeeb5-129">The following table shows the properties that are required when you create the androidForWorkApp.</span></span>

|<span data-ttu-id="eeeb5-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eeeb5-130">Property</span></span>|<span data-ttu-id="eeeb5-131">種類</span><span class="sxs-lookup"><span data-stu-id="eeeb5-131">Type</span></span>|<span data-ttu-id="eeeb5-132">説明</span><span class="sxs-lookup"><span data-stu-id="eeeb5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eeeb5-133">ID</span><span class="sxs-lookup"><span data-stu-id="eeeb5-133">id</span></span>|<span data-ttu-id="eeeb5-134">String</span><span class="sxs-lookup"><span data-stu-id="eeeb5-134">String</span></span>|<span data-ttu-id="eeeb5-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="eeeb5-135">Key of the entity.</span></span> <span data-ttu-id="eeeb5-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eeeb5-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eeeb5-137">displayName</span><span class="sxs-lookup"><span data-stu-id="eeeb5-137">displayName</span></span>|<span data-ttu-id="eeeb5-138">String</span><span class="sxs-lookup"><span data-stu-id="eeeb5-138">String</span></span>|<span data-ttu-id="eeeb5-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="eeeb5-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="eeeb5-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eeeb5-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eeeb5-141">説明</span><span class="sxs-lookup"><span data-stu-id="eeeb5-141">description</span></span>|<span data-ttu-id="eeeb5-142">String</span><span class="sxs-lookup"><span data-stu-id="eeeb5-142">String</span></span>|<span data-ttu-id="eeeb5-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="eeeb5-143">The description of the app.</span></span> <span data-ttu-id="eeeb5-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eeeb5-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eeeb5-145">publisher</span><span class="sxs-lookup"><span data-stu-id="eeeb5-145">publisher</span></span>|<span data-ttu-id="eeeb5-146">String</span><span class="sxs-lookup"><span data-stu-id="eeeb5-146">String</span></span>|<span data-ttu-id="eeeb5-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="eeeb5-147">The publisher of the app.</span></span> <span data-ttu-id="eeeb5-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eeeb5-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eeeb5-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="eeeb5-149">largeIcon</span></span>|[<span data-ttu-id="eeeb5-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="eeeb5-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="eeeb5-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="eeeb5-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="eeeb5-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eeeb5-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eeeb5-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eeeb5-153">createdDateTime</span></span>|<span data-ttu-id="eeeb5-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eeeb5-154">DateTimeOffset</span></span>|<span data-ttu-id="eeeb5-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="eeeb5-155">The date and time the app was created.</span></span> <span data-ttu-id="eeeb5-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eeeb5-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eeeb5-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eeeb5-157">lastModifiedDateTime</span></span>|<span data-ttu-id="eeeb5-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eeeb5-158">DateTimeOffset</span></span>|<span data-ttu-id="eeeb5-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="eeeb5-159">The date and time the app was last modified.</span></span> <span data-ttu-id="eeeb5-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eeeb5-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eeeb5-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="eeeb5-161">isFeatured</span></span>|<span data-ttu-id="eeeb5-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="eeeb5-162">Boolean</span></span>|<span data-ttu-id="eeeb5-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eeeb5-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eeeb5-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="eeeb5-164">privacyInformationUrl</span></span>|<span data-ttu-id="eeeb5-165">String</span><span class="sxs-lookup"><span data-stu-id="eeeb5-165">String</span></span>|<span data-ttu-id="eeeb5-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="eeeb5-166">The privacy statement Url.</span></span> <span data-ttu-id="eeeb5-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eeeb5-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eeeb5-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="eeeb5-168">informationUrl</span></span>|<span data-ttu-id="eeeb5-169">String</span><span class="sxs-lookup"><span data-stu-id="eeeb5-169">String</span></span>|<span data-ttu-id="eeeb5-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="eeeb5-170">The more information Url.</span></span> <span data-ttu-id="eeeb5-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eeeb5-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eeeb5-172">owner</span><span class="sxs-lookup"><span data-stu-id="eeeb5-172">owner</span></span>|<span data-ttu-id="eeeb5-173">String</span><span class="sxs-lookup"><span data-stu-id="eeeb5-173">String</span></span>|<span data-ttu-id="eeeb5-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="eeeb5-174">The owner of the app.</span></span> <span data-ttu-id="eeeb5-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eeeb5-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eeeb5-176">developer</span><span class="sxs-lookup"><span data-stu-id="eeeb5-176">developer</span></span>|<span data-ttu-id="eeeb5-177">String</span><span class="sxs-lookup"><span data-stu-id="eeeb5-177">String</span></span>|<span data-ttu-id="eeeb5-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="eeeb5-178">The developer of the app.</span></span> <span data-ttu-id="eeeb5-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eeeb5-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eeeb5-180">notes</span><span class="sxs-lookup"><span data-stu-id="eeeb5-180">notes</span></span>|<span data-ttu-id="eeeb5-181">String</span><span class="sxs-lookup"><span data-stu-id="eeeb5-181">String</span></span>|<span data-ttu-id="eeeb5-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="eeeb5-182">Notes for the app.</span></span> <span data-ttu-id="eeeb5-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eeeb5-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eeeb5-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="eeeb5-184">uploadState</span></span>|<span data-ttu-id="eeeb5-185">Int32</span><span class="sxs-lookup"><span data-stu-id="eeeb5-185">Int32</span></span>|<span data-ttu-id="eeeb5-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="eeeb5-186">The upload state.</span></span> <span data-ttu-id="eeeb5-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eeeb5-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eeeb5-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="eeeb5-188">publishingState</span></span>|[<span data-ttu-id="eeeb5-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="eeeb5-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="eeeb5-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="eeeb5-190">The publishing state for the app.</span></span> <span data-ttu-id="eeeb5-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="eeeb5-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="eeeb5-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="eeeb5-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="eeeb5-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="eeeb5-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="eeeb5-194">packageId</span><span class="sxs-lookup"><span data-stu-id="eeeb5-194">packageId</span></span>|<span data-ttu-id="eeeb5-195">String</span><span class="sxs-lookup"><span data-stu-id="eeeb5-195">String</span></span>|<span data-ttu-id="eeeb5-196">パッケージの識別子。</span><span class="sxs-lookup"><span data-stu-id="eeeb5-196">The package identifier.</span></span>|
|<span data-ttu-id="eeeb5-197">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="eeeb5-197">appIdentifier</span></span>|<span data-ttu-id="eeeb5-198">String</span><span class="sxs-lookup"><span data-stu-id="eeeb5-198">String</span></span>|<span data-ttu-id="eeeb5-199">ID 名。</span><span class="sxs-lookup"><span data-stu-id="eeeb5-199">The Identity Name.</span></span>|
|<span data-ttu-id="eeeb5-200">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="eeeb5-200">usedLicenseCount</span></span>|<span data-ttu-id="eeeb5-201">Int32</span><span class="sxs-lookup"><span data-stu-id="eeeb5-201">Int32</span></span>|<span data-ttu-id="eeeb5-202">使用中の VPP ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="eeeb5-202">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="eeeb5-203">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="eeeb5-203">totalLicenseCount</span></span>|<span data-ttu-id="eeeb5-204">Int32</span><span class="sxs-lookup"><span data-stu-id="eeeb5-204">Int32</span></span>|<span data-ttu-id="eeeb5-205">VPP ライセンスの総数。</span><span class="sxs-lookup"><span data-stu-id="eeeb5-205">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="eeeb5-206">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="eeeb5-206">appStoreUrl</span></span>|<span data-ttu-id="eeeb5-207">String</span><span class="sxs-lookup"><span data-stu-id="eeeb5-207">String</span></span>|<span data-ttu-id="eeeb5-208">作業ストア アプリケーションの URL を再生します。</span><span class="sxs-lookup"><span data-stu-id="eeeb5-208">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="eeeb5-209">応答</span><span class="sxs-lookup"><span data-stu-id="eeeb5-209">Response</span></span>
<span data-ttu-id="eeeb5-210">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[androidForWorkApp](../resources/intune-apps-androidforworkapp.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="eeeb5-210">If successful, this method returns a `201 Created` response code and a [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eeeb5-211">例</span><span class="sxs-lookup"><span data-stu-id="eeeb5-211">Example</span></span>
### <a name="request"></a><span data-ttu-id="eeeb5-212">要求</span><span class="sxs-lookup"><span data-stu-id="eeeb5-212">Request</span></span>
<span data-ttu-id="eeeb5-213">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="eeeb5-213">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 855

{
  "@odata.type": "#microsoft.graph.androidForWorkApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="eeeb5-214">応答</span><span class="sxs-lookup"><span data-stu-id="eeeb5-214">Response</span></span>
<span data-ttu-id="eeeb5-p117">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="eeeb5-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 963

{
  "@odata.type": "#microsoft.graph.androidForWorkApp",
  "id": "c5010785-0785-c501-8507-01c5850701c5",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```




