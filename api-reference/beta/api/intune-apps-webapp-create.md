---
title: webApp の作成
description: 新しい webApp オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9ad9c3a9dd89910d0d1f2d8df44a5b7bdcdaeb87
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413865"
---
# <a name="create-webapp"></a><span data-ttu-id="4db57-103">webApp の作成</span><span class="sxs-lookup"><span data-stu-id="4db57-103">Create webApp</span></span>

> <span data-ttu-id="4db57-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4db57-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4db57-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4db57-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4db57-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4db57-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4db57-107">新しい [webApp](../resources/intune-apps-webapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4db57-107">Create a new [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4db57-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="4db57-108">Prerequisites</span></span>
<span data-ttu-id="4db57-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4db57-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4db57-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4db57-111">Permission type</span></span>|<span data-ttu-id="4db57-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4db57-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4db57-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4db57-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4db57-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4db57-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4db57-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4db57-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4db57-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4db57-116">Not supported.</span></span>|
|<span data-ttu-id="4db57-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4db57-117">Application</span></span>|<span data-ttu-id="4db57-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4db57-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4db57-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4db57-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="4db57-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4db57-120">Request headers</span></span>
|<span data-ttu-id="4db57-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4db57-121">Header</span></span>|<span data-ttu-id="4db57-122">値</span><span class="sxs-lookup"><span data-stu-id="4db57-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4db57-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4db57-123">Authorization</span></span>|<span data-ttu-id="4db57-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="4db57-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4db57-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4db57-125">Accept</span></span>|<span data-ttu-id="4db57-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4db57-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4db57-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="4db57-127">Request body</span></span>
<span data-ttu-id="4db57-128">要求本文で、webApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4db57-128">In the request body, supply a JSON representation for the webApp object.</span></span>

<span data-ttu-id="4db57-129">次の表に、webApp 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4db57-129">The following table shows the properties that are required when you create the webApp.</span></span>

|<span data-ttu-id="4db57-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4db57-130">Property</span></span>|<span data-ttu-id="4db57-131">型</span><span class="sxs-lookup"><span data-stu-id="4db57-131">Type</span></span>|<span data-ttu-id="4db57-132">説明</span><span class="sxs-lookup"><span data-stu-id="4db57-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4db57-133">id</span><span class="sxs-lookup"><span data-stu-id="4db57-133">id</span></span>|<span data-ttu-id="4db57-134">String</span><span class="sxs-lookup"><span data-stu-id="4db57-134">String</span></span>|<span data-ttu-id="4db57-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4db57-135">Key of the entity.</span></span> <span data-ttu-id="4db57-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4db57-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4db57-137">displayName</span><span class="sxs-lookup"><span data-stu-id="4db57-137">displayName</span></span>|<span data-ttu-id="4db57-138">String</span><span class="sxs-lookup"><span data-stu-id="4db57-138">String</span></span>|<span data-ttu-id="4db57-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="4db57-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4db57-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4db57-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4db57-141">説明</span><span class="sxs-lookup"><span data-stu-id="4db57-141">description</span></span>|<span data-ttu-id="4db57-142">String</span><span class="sxs-lookup"><span data-stu-id="4db57-142">String</span></span>|<span data-ttu-id="4db57-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="4db57-143">The description of the app.</span></span> <span data-ttu-id="4db57-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4db57-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4db57-145">publisher</span><span class="sxs-lookup"><span data-stu-id="4db57-145">publisher</span></span>|<span data-ttu-id="4db57-146">String</span><span class="sxs-lookup"><span data-stu-id="4db57-146">String</span></span>|<span data-ttu-id="4db57-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="4db57-147">The publisher of the app.</span></span> <span data-ttu-id="4db57-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4db57-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4db57-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4db57-149">largeIcon</span></span>|[<span data-ttu-id="4db57-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4db57-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4db57-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="4db57-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4db57-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4db57-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4db57-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4db57-153">createdDateTime</span></span>|<span data-ttu-id="4db57-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4db57-154">DateTimeOffset</span></span>|<span data-ttu-id="4db57-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="4db57-155">The date and time the app was created.</span></span> <span data-ttu-id="4db57-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4db57-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4db57-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4db57-157">lastModifiedDateTime</span></span>|<span data-ttu-id="4db57-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4db57-158">DateTimeOffset</span></span>|<span data-ttu-id="4db57-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="4db57-159">The date and time the app was last modified.</span></span> <span data-ttu-id="4db57-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4db57-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4db57-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4db57-161">isFeatured</span></span>|<span data-ttu-id="4db57-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db57-162">Boolean</span></span>|<span data-ttu-id="4db57-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4db57-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4db57-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4db57-164">privacyInformationUrl</span></span>|<span data-ttu-id="4db57-165">String</span><span class="sxs-lookup"><span data-stu-id="4db57-165">String</span></span>|<span data-ttu-id="4db57-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="4db57-166">The privacy statement Url.</span></span> <span data-ttu-id="4db57-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4db57-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4db57-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4db57-168">informationUrl</span></span>|<span data-ttu-id="4db57-169">String</span><span class="sxs-lookup"><span data-stu-id="4db57-169">String</span></span>|<span data-ttu-id="4db57-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="4db57-170">The more information Url.</span></span> <span data-ttu-id="4db57-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4db57-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4db57-172">owner</span><span class="sxs-lookup"><span data-stu-id="4db57-172">owner</span></span>|<span data-ttu-id="4db57-173">String</span><span class="sxs-lookup"><span data-stu-id="4db57-173">String</span></span>|<span data-ttu-id="4db57-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="4db57-174">The owner of the app.</span></span> <span data-ttu-id="4db57-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4db57-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4db57-176">developer</span><span class="sxs-lookup"><span data-stu-id="4db57-176">developer</span></span>|<span data-ttu-id="4db57-177">String</span><span class="sxs-lookup"><span data-stu-id="4db57-177">String</span></span>|<span data-ttu-id="4db57-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="4db57-178">The developer of the app.</span></span> <span data-ttu-id="4db57-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4db57-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4db57-180">notes</span><span class="sxs-lookup"><span data-stu-id="4db57-180">notes</span></span>|<span data-ttu-id="4db57-181">String</span><span class="sxs-lookup"><span data-stu-id="4db57-181">String</span></span>|<span data-ttu-id="4db57-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="4db57-182">Notes for the app.</span></span> <span data-ttu-id="4db57-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4db57-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4db57-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="4db57-184">uploadState</span></span>|<span data-ttu-id="4db57-185">Int32</span><span class="sxs-lookup"><span data-stu-id="4db57-185">Int32</span></span>|<span data-ttu-id="4db57-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="4db57-186">The upload state.</span></span> <span data-ttu-id="4db57-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4db57-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4db57-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="4db57-188">publishingState</span></span>|[<span data-ttu-id="4db57-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="4db57-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4db57-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="4db57-190">The publishing state for the app.</span></span> <span data-ttu-id="4db57-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="4db57-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4db57-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="4db57-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="4db57-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="4db57-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4db57-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="4db57-194">isAssigned</span></span>|<span data-ttu-id="4db57-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db57-195">Boolean</span></span>|<span data-ttu-id="4db57-196">アプリケーションが少なくとも 1 つのグループに割り当てられているかどうかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="4db57-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="4db57-197">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4db57-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4db57-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4db57-198">roleScopeTagIds</span></span>|<span data-ttu-id="4db57-199">String コレクション</span><span class="sxs-lookup"><span data-stu-id="4db57-199">String collection</span></span>|<span data-ttu-id="4db57-200">このモバイル アプリケーションのスコープのタグ id の一覧です。</span><span class="sxs-lookup"><span data-stu-id="4db57-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="4db57-201">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4db57-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4db57-202">appUrl</span><span class="sxs-lookup"><span data-stu-id="4db57-202">appUrl</span></span>|<span data-ttu-id="4db57-203">String</span><span class="sxs-lookup"><span data-stu-id="4db57-203">String</span></span>|<span data-ttu-id="4db57-204">Web アプリの URL。</span><span class="sxs-lookup"><span data-stu-id="4db57-204">The web app URL.</span></span>|
|<span data-ttu-id="4db57-205">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="4db57-205">useManagedBrowser</span></span>|<span data-ttu-id="4db57-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="4db57-206">Boolean</span></span>|<span data-ttu-id="4db57-207">管理対象のブラウザーを使用するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="4db57-207">Whether or not to use managed browser.</span></span> <span data-ttu-id="4db57-208">このプロパティは、Android と iOS にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="4db57-208">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="4db57-209">応答</span><span class="sxs-lookup"><span data-stu-id="4db57-209">Response</span></span>
<span data-ttu-id="4db57-210">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [webApp](../resources/intune-apps-webapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4db57-210">If successful, this method returns a `201 Created` response code and a [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4db57-211">例</span><span class="sxs-lookup"><span data-stu-id="4db57-211">Example</span></span>

### <a name="request"></a><span data-ttu-id="4db57-212">要求</span><span class="sxs-lookup"><span data-stu-id="4db57-212">Request</span></span>
<span data-ttu-id="4db57-213">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4db57-213">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 752

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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```

### <a name="response"></a><span data-ttu-id="4db57-214">応答</span><span class="sxs-lookup"><span data-stu-id="4db57-214">Response</span></span>
<span data-ttu-id="4db57-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4db57-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 924

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
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```




