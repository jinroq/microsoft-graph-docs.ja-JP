---
title: macOSOfficeSuiteApp の作成
description: 新しい macOSOfficeSuiteApp オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cc6d25d96e3fefddb81783b3eb2e28c96773d64a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414348"
---
# <a name="create-macosofficesuiteapp"></a><span data-ttu-id="f20c8-103">macOSOfficeSuiteApp の作成</span><span class="sxs-lookup"><span data-stu-id="f20c8-103">Create macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="f20c8-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f20c8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f20c8-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f20c8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f20c8-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f20c8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f20c8-107">新しい [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f20c8-107">Create a new [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f20c8-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="f20c8-108">Prerequisites</span></span>
<span data-ttu-id="f20c8-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f20c8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f20c8-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f20c8-111">Permission type</span></span>|<span data-ttu-id="f20c8-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f20c8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f20c8-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f20c8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f20c8-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f20c8-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f20c8-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f20c8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f20c8-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f20c8-116">Not supported.</span></span>|
|<span data-ttu-id="f20c8-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f20c8-117">Application</span></span>|<span data-ttu-id="f20c8-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f20c8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f20c8-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f20c8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="f20c8-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f20c8-120">Request headers</span></span>
|<span data-ttu-id="f20c8-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f20c8-121">Header</span></span>|<span data-ttu-id="f20c8-122">値</span><span class="sxs-lookup"><span data-stu-id="f20c8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f20c8-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f20c8-123">Authorization</span></span>|<span data-ttu-id="f20c8-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f20c8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f20c8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f20c8-125">Accept</span></span>|<span data-ttu-id="f20c8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f20c8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f20c8-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f20c8-127">Request body</span></span>
<span data-ttu-id="f20c8-128">要求本文で、macOSOfficeSuiteApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f20c8-128">In the request body, supply a JSON representation for the macOSOfficeSuiteApp object.</span></span>

<span data-ttu-id="f20c8-129">次の表に、macOSOfficeSuiteApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f20c8-129">The following table shows the properties that are required when you create the macOSOfficeSuiteApp.</span></span>

|<span data-ttu-id="f20c8-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f20c8-130">Property</span></span>|<span data-ttu-id="f20c8-131">型</span><span class="sxs-lookup"><span data-stu-id="f20c8-131">Type</span></span>|<span data-ttu-id="f20c8-132">説明</span><span class="sxs-lookup"><span data-stu-id="f20c8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f20c8-133">id</span><span class="sxs-lookup"><span data-stu-id="f20c8-133">id</span></span>|<span data-ttu-id="f20c8-134">String</span><span class="sxs-lookup"><span data-stu-id="f20c8-134">String</span></span>|<span data-ttu-id="f20c8-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f20c8-135">Key of the entity.</span></span> <span data-ttu-id="f20c8-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f20c8-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f20c8-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f20c8-137">displayName</span></span>|<span data-ttu-id="f20c8-138">String</span><span class="sxs-lookup"><span data-stu-id="f20c8-138">String</span></span>|<span data-ttu-id="f20c8-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="f20c8-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f20c8-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f20c8-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f20c8-141">説明</span><span class="sxs-lookup"><span data-stu-id="f20c8-141">description</span></span>|<span data-ttu-id="f20c8-142">String</span><span class="sxs-lookup"><span data-stu-id="f20c8-142">String</span></span>|<span data-ttu-id="f20c8-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="f20c8-143">The description of the app.</span></span> <span data-ttu-id="f20c8-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f20c8-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f20c8-145">publisher</span><span class="sxs-lookup"><span data-stu-id="f20c8-145">publisher</span></span>|<span data-ttu-id="f20c8-146">String</span><span class="sxs-lookup"><span data-stu-id="f20c8-146">String</span></span>|<span data-ttu-id="f20c8-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="f20c8-147">The publisher of the app.</span></span> <span data-ttu-id="f20c8-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f20c8-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f20c8-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f20c8-149">largeIcon</span></span>|[<span data-ttu-id="f20c8-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f20c8-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f20c8-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="f20c8-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f20c8-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f20c8-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f20c8-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f20c8-153">createdDateTime</span></span>|<span data-ttu-id="f20c8-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f20c8-154">DateTimeOffset</span></span>|<span data-ttu-id="f20c8-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="f20c8-155">The date and time the app was created.</span></span> <span data-ttu-id="f20c8-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f20c8-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f20c8-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f20c8-157">lastModifiedDateTime</span></span>|<span data-ttu-id="f20c8-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f20c8-158">DateTimeOffset</span></span>|<span data-ttu-id="f20c8-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="f20c8-159">The date and time the app was last modified.</span></span> <span data-ttu-id="f20c8-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f20c8-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f20c8-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f20c8-161">isFeatured</span></span>|<span data-ttu-id="f20c8-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="f20c8-162">Boolean</span></span>|<span data-ttu-id="f20c8-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f20c8-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f20c8-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f20c8-164">privacyInformationUrl</span></span>|<span data-ttu-id="f20c8-165">String</span><span class="sxs-lookup"><span data-stu-id="f20c8-165">String</span></span>|<span data-ttu-id="f20c8-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="f20c8-166">The privacy statement Url.</span></span> <span data-ttu-id="f20c8-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f20c8-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f20c8-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f20c8-168">informationUrl</span></span>|<span data-ttu-id="f20c8-169">String</span><span class="sxs-lookup"><span data-stu-id="f20c8-169">String</span></span>|<span data-ttu-id="f20c8-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="f20c8-170">The more information Url.</span></span> <span data-ttu-id="f20c8-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f20c8-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f20c8-172">owner</span><span class="sxs-lookup"><span data-stu-id="f20c8-172">owner</span></span>|<span data-ttu-id="f20c8-173">String</span><span class="sxs-lookup"><span data-stu-id="f20c8-173">String</span></span>|<span data-ttu-id="f20c8-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="f20c8-174">The owner of the app.</span></span> <span data-ttu-id="f20c8-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f20c8-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f20c8-176">developer</span><span class="sxs-lookup"><span data-stu-id="f20c8-176">developer</span></span>|<span data-ttu-id="f20c8-177">String</span><span class="sxs-lookup"><span data-stu-id="f20c8-177">String</span></span>|<span data-ttu-id="f20c8-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="f20c8-178">The developer of the app.</span></span> <span data-ttu-id="f20c8-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f20c8-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f20c8-180">notes</span><span class="sxs-lookup"><span data-stu-id="f20c8-180">notes</span></span>|<span data-ttu-id="f20c8-181">String</span><span class="sxs-lookup"><span data-stu-id="f20c8-181">String</span></span>|<span data-ttu-id="f20c8-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="f20c8-182">Notes for the app.</span></span> <span data-ttu-id="f20c8-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f20c8-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f20c8-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="f20c8-184">uploadState</span></span>|<span data-ttu-id="f20c8-185">Int32</span><span class="sxs-lookup"><span data-stu-id="f20c8-185">Int32</span></span>|<span data-ttu-id="f20c8-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="f20c8-186">The upload state.</span></span> <span data-ttu-id="f20c8-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f20c8-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f20c8-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="f20c8-188">publishingState</span></span>|[<span data-ttu-id="f20c8-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f20c8-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f20c8-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="f20c8-190">The publishing state for the app.</span></span> <span data-ttu-id="f20c8-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="f20c8-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f20c8-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="f20c8-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="f20c8-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="f20c8-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f20c8-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="f20c8-194">isAssigned</span></span>|<span data-ttu-id="f20c8-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="f20c8-195">Boolean</span></span>|<span data-ttu-id="f20c8-196">アプリケーションが少なくとも 1 つのグループに割り当てられているかどうかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="f20c8-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="f20c8-197">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f20c8-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f20c8-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f20c8-198">roleScopeTagIds</span></span>|<span data-ttu-id="f20c8-199">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f20c8-199">String collection</span></span>|<span data-ttu-id="f20c8-200">このモバイル アプリケーションのスコープのタグ id の一覧です。</span><span class="sxs-lookup"><span data-stu-id="f20c8-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="f20c8-201">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f20c8-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|



## <a name="response"></a><span data-ttu-id="f20c8-202">応答</span><span class="sxs-lookup"><span data-stu-id="f20c8-202">Response</span></span>
<span data-ttu-id="f20c8-203">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f20c8-203">If successful, this method returns a `201 Created` response code and a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f20c8-204">例</span><span class="sxs-lookup"><span data-stu-id="f20c8-204">Example</span></span>

### <a name="request"></a><span data-ttu-id="f20c8-205">要求</span><span class="sxs-lookup"><span data-stu-id="f20c8-205">Request</span></span>
<span data-ttu-id="f20c8-206">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f20c8-206">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 691

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
  ]
}
```

### <a name="response"></a><span data-ttu-id="f20c8-207">応答</span><span class="sxs-lookup"><span data-stu-id="f20c8-207">Response</span></span>
<span data-ttu-id="f20c8-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f20c8-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 863

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
  ]
}
```




