---
title: WindowsStoreApp を作成します。
description: 新しい windowsStoreApp オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 524c02ac23655f9313c75dffad2bea0c77176431
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394230"
---
# <a name="create-windowsstoreapp"></a><span data-ttu-id="c1bec-103">WindowsStoreApp を作成します。</span><span class="sxs-lookup"><span data-stu-id="c1bec-103">Create windowsStoreApp</span></span>

> <span data-ttu-id="c1bec-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c1bec-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c1bec-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c1bec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c1bec-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c1bec-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1bec-107">新しい[windowsStoreApp](../resources/intune-apps-windowsstoreapp.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c1bec-107">Create a new [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c1bec-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="c1bec-108">Prerequisites</span></span>
<span data-ttu-id="c1bec-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c1bec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c1bec-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c1bec-111">Permission type</span></span>|<span data-ttu-id="c1bec-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c1bec-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c1bec-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c1bec-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c1bec-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c1bec-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c1bec-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c1bec-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1bec-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c1bec-116">Not supported.</span></span>|
|<span data-ttu-id="c1bec-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c1bec-117">Application</span></span>|<span data-ttu-id="c1bec-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c1bec-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1bec-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c1bec-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="c1bec-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c1bec-120">Request headers</span></span>
|<span data-ttu-id="c1bec-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c1bec-121">Header</span></span>|<span data-ttu-id="c1bec-122">値</span><span class="sxs-lookup"><span data-stu-id="c1bec-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c1bec-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1bec-123">Authorization</span></span>|<span data-ttu-id="c1bec-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c1bec-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c1bec-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c1bec-125">Accept</span></span>|<span data-ttu-id="c1bec-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c1bec-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1bec-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c1bec-127">Request body</span></span>
<span data-ttu-id="c1bec-128">要求の本文に windowsStoreApp オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="c1bec-128">In the request body, supply a JSON representation for the windowsStoreApp object.</span></span>

<span data-ttu-id="c1bec-129">次の表は、windowsStoreApp を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c1bec-129">The following table shows the properties that are required when you create the windowsStoreApp.</span></span>

|<span data-ttu-id="c1bec-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1bec-130">Property</span></span>|<span data-ttu-id="c1bec-131">型</span><span class="sxs-lookup"><span data-stu-id="c1bec-131">Type</span></span>|<span data-ttu-id="c1bec-132">説明</span><span class="sxs-lookup"><span data-stu-id="c1bec-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1bec-133">id</span><span class="sxs-lookup"><span data-stu-id="c1bec-133">id</span></span>|<span data-ttu-id="c1bec-134">String</span><span class="sxs-lookup"><span data-stu-id="c1bec-134">String</span></span>|<span data-ttu-id="c1bec-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c1bec-135">Key of the entity.</span></span> <span data-ttu-id="c1bec-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1bec-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1bec-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c1bec-137">displayName</span></span>|<span data-ttu-id="c1bec-138">String</span><span class="sxs-lookup"><span data-stu-id="c1bec-138">String</span></span>|<span data-ttu-id="c1bec-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="c1bec-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="c1bec-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1bec-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1bec-141">説明</span><span class="sxs-lookup"><span data-stu-id="c1bec-141">description</span></span>|<span data-ttu-id="c1bec-142">String</span><span class="sxs-lookup"><span data-stu-id="c1bec-142">String</span></span>|<span data-ttu-id="c1bec-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="c1bec-143">The description of the app.</span></span> <span data-ttu-id="c1bec-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1bec-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1bec-145">publisher</span><span class="sxs-lookup"><span data-stu-id="c1bec-145">publisher</span></span>|<span data-ttu-id="c1bec-146">String</span><span class="sxs-lookup"><span data-stu-id="c1bec-146">String</span></span>|<span data-ttu-id="c1bec-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="c1bec-147">The publisher of the app.</span></span> <span data-ttu-id="c1bec-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1bec-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1bec-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="c1bec-149">largeIcon</span></span>|[<span data-ttu-id="c1bec-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="c1bec-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="c1bec-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="c1bec-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="c1bec-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1bec-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1bec-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c1bec-153">createdDateTime</span></span>|<span data-ttu-id="c1bec-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1bec-154">DateTimeOffset</span></span>|<span data-ttu-id="c1bec-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="c1bec-155">The date and time the app was created.</span></span> <span data-ttu-id="c1bec-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1bec-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1bec-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c1bec-157">lastModifiedDateTime</span></span>|<span data-ttu-id="c1bec-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1bec-158">DateTimeOffset</span></span>|<span data-ttu-id="c1bec-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="c1bec-159">The date and time the app was last modified.</span></span> <span data-ttu-id="c1bec-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1bec-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1bec-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="c1bec-161">isFeatured</span></span>|<span data-ttu-id="c1bec-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1bec-162">Boolean</span></span>|<span data-ttu-id="c1bec-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1bec-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1bec-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="c1bec-164">privacyInformationUrl</span></span>|<span data-ttu-id="c1bec-165">String</span><span class="sxs-lookup"><span data-stu-id="c1bec-165">String</span></span>|<span data-ttu-id="c1bec-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="c1bec-166">The privacy statement Url.</span></span> <span data-ttu-id="c1bec-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1bec-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1bec-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="c1bec-168">informationUrl</span></span>|<span data-ttu-id="c1bec-169">String</span><span class="sxs-lookup"><span data-stu-id="c1bec-169">String</span></span>|<span data-ttu-id="c1bec-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="c1bec-170">The more information Url.</span></span> <span data-ttu-id="c1bec-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1bec-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1bec-172">owner</span><span class="sxs-lookup"><span data-stu-id="c1bec-172">owner</span></span>|<span data-ttu-id="c1bec-173">String</span><span class="sxs-lookup"><span data-stu-id="c1bec-173">String</span></span>|<span data-ttu-id="c1bec-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="c1bec-174">The owner of the app.</span></span> <span data-ttu-id="c1bec-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1bec-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1bec-176">developer</span><span class="sxs-lookup"><span data-stu-id="c1bec-176">developer</span></span>|<span data-ttu-id="c1bec-177">String</span><span class="sxs-lookup"><span data-stu-id="c1bec-177">String</span></span>|<span data-ttu-id="c1bec-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="c1bec-178">The developer of the app.</span></span> <span data-ttu-id="c1bec-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1bec-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1bec-180">notes</span><span class="sxs-lookup"><span data-stu-id="c1bec-180">notes</span></span>|<span data-ttu-id="c1bec-181">String</span><span class="sxs-lookup"><span data-stu-id="c1bec-181">String</span></span>|<span data-ttu-id="c1bec-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="c1bec-182">Notes for the app.</span></span> <span data-ttu-id="c1bec-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1bec-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1bec-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="c1bec-184">uploadState</span></span>|<span data-ttu-id="c1bec-185">Int32</span><span class="sxs-lookup"><span data-stu-id="c1bec-185">Int32</span></span>|<span data-ttu-id="c1bec-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="c1bec-186">The upload state.</span></span> <span data-ttu-id="c1bec-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1bec-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1bec-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="c1bec-188">publishingState</span></span>|[<span data-ttu-id="c1bec-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="c1bec-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="c1bec-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="c1bec-190">The publishing state for the app.</span></span> <span data-ttu-id="c1bec-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="c1bec-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="c1bec-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="c1bec-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="c1bec-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="c1bec-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="c1bec-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="c1bec-194">isAssigned</span></span>|<span data-ttu-id="c1bec-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1bec-195">Boolean</span></span>|<span data-ttu-id="c1bec-196">アプリケーションが少なくとも 1 つのグループに割り当てられているかどうかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="c1bec-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="c1bec-197">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1bec-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1bec-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c1bec-198">roleScopeTagIds</span></span>|<span data-ttu-id="c1bec-199">String コレクション</span><span class="sxs-lookup"><span data-stu-id="c1bec-199">String collection</span></span>|<span data-ttu-id="c1bec-200">このモバイル アプリケーションのスコープのタグ id の一覧です。</span><span class="sxs-lookup"><span data-stu-id="c1bec-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="c1bec-201">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c1bec-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="c1bec-202">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="c1bec-202">appStoreUrl</span></span>|<span data-ttu-id="c1bec-203">String</span><span class="sxs-lookup"><span data-stu-id="c1bec-203">String</span></span>|<span data-ttu-id="c1bec-204">Windows アプリケーション ストアの URL です。</span><span class="sxs-lookup"><span data-stu-id="c1bec-204">The Windows app store URL.</span></span>|



## <a name="response"></a><span data-ttu-id="c1bec-205">応答</span><span class="sxs-lookup"><span data-stu-id="c1bec-205">Response</span></span>
<span data-ttu-id="c1bec-206">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[windowsStoreApp](../resources/intune-apps-windowsstoreapp.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="c1bec-206">If successful, this method returns a `201 Created` response code and a [windowsStoreApp](../resources/intune-apps-windowsstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c1bec-207">例</span><span class="sxs-lookup"><span data-stu-id="c1bec-207">Example</span></span>

### <a name="request"></a><span data-ttu-id="c1bec-208">要求</span><span class="sxs-lookup"><span data-stu-id="c1bec-208">Request</span></span>
<span data-ttu-id="c1bec-209">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c1bec-209">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 741

{
  "@odata.type": "#microsoft.graph.windowsStoreApp",
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

### <a name="response"></a><span data-ttu-id="c1bec-210">応答</span><span class="sxs-lookup"><span data-stu-id="c1bec-210">Response</span></span>
<span data-ttu-id="c1bec-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c1bec-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 913

{
  "@odata.type": "#microsoft.graph.windowsStoreApp",
  "id": "fd4a5f8a-5f8a-fd4a-8a5f-4afd8a5f4afd",
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




