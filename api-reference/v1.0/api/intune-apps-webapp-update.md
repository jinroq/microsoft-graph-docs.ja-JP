---
title: Update webApp
description: webApp オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6e8c40738aaf0e59f384c02df69664dd3a6e320b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580525"
---
# <a name="update-webapp"></a><span data-ttu-id="5c711-103">Update webApp</span><span class="sxs-lookup"><span data-stu-id="5c711-103">Update webApp</span></span>

> <span data-ttu-id="5c711-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5c711-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c711-105">[webApp](../resources/intune-apps-webapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5c711-105">Update the properties of a [webApp](../resources/intune-apps-webapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5c711-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="5c711-106">Prerequisites</span></span>
<span data-ttu-id="5c711-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5c711-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c711-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5c711-109">Permission type</span></span>|<span data-ttu-id="5c711-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5c711-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c711-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5c711-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5c711-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c711-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5c711-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5c711-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c711-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5c711-114">Not supported.</span></span>|
|<span data-ttu-id="5c711-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5c711-115">Application</span></span>|<span data-ttu-id="5c711-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5c711-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c711-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5c711-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="5c711-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5c711-118">Request headers</span></span>
|<span data-ttu-id="5c711-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5c711-119">Header</span></span>|<span data-ttu-id="5c711-120">値</span><span class="sxs-lookup"><span data-stu-id="5c711-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c711-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c711-121">Authorization</span></span>|<span data-ttu-id="5c711-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="5c711-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c711-123">承諾</span><span class="sxs-lookup"><span data-stu-id="5c711-123">Accept</span></span>|<span data-ttu-id="5c711-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5c711-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c711-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="5c711-125">Request body</span></span>
<span data-ttu-id="5c711-126">要求本文で、[webApp](../resources/intune-apps-webapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5c711-126">In the request body, supply a JSON representation for the [webApp](../resources/intune-apps-webapp.md) object.</span></span>

<span data-ttu-id="5c711-127">次の表に、[webApp](../resources/intune-apps-webapp.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="5c711-127">The following table shows the properties that are required when you create the [webApp](../resources/intune-apps-webapp.md).</span></span>

|<span data-ttu-id="5c711-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5c711-128">Property</span></span>|<span data-ttu-id="5c711-129">型</span><span class="sxs-lookup"><span data-stu-id="5c711-129">Type</span></span>|<span data-ttu-id="5c711-130">説明</span><span class="sxs-lookup"><span data-stu-id="5c711-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c711-131">id</span><span class="sxs-lookup"><span data-stu-id="5c711-131">id</span></span>|<span data-ttu-id="5c711-132">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="5c711-132">String</span></span>|<span data-ttu-id="5c711-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="5c711-133">Key of the entity.</span></span> <span data-ttu-id="5c711-134">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c711-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c711-135">displayName</span><span class="sxs-lookup"><span data-stu-id="5c711-135">displayName</span></span>|<span data-ttu-id="5c711-136">String</span><span class="sxs-lookup"><span data-stu-id="5c711-136">String</span></span>|<span data-ttu-id="5c711-137">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="5c711-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="5c711-138">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c711-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c711-139">説明</span><span class="sxs-lookup"><span data-stu-id="5c711-139">description</span></span>|<span data-ttu-id="5c711-140">String</span><span class="sxs-lookup"><span data-stu-id="5c711-140">String</span></span>|<span data-ttu-id="5c711-141">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="5c711-141">The description of the app.</span></span> <span data-ttu-id="5c711-142">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c711-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c711-143">publisher</span><span class="sxs-lookup"><span data-stu-id="5c711-143">publisher</span></span>|<span data-ttu-id="5c711-144">String</span><span class="sxs-lookup"><span data-stu-id="5c711-144">String</span></span>|<span data-ttu-id="5c711-145">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="5c711-145">The publisher of the app.</span></span> <span data-ttu-id="5c711-146">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c711-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c711-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="5c711-147">largeIcon</span></span>|[<span data-ttu-id="5c711-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5c711-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5c711-149">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="5c711-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="5c711-150">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c711-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c711-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5c711-151">createdDateTime</span></span>|<span data-ttu-id="5c711-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c711-152">DateTimeOffset</span></span>|<span data-ttu-id="5c711-153">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="5c711-153">The date and time the app was created.</span></span> <span data-ttu-id="5c711-154">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c711-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c711-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5c711-155">lastModifiedDateTime</span></span>|<span data-ttu-id="5c711-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c711-156">DateTimeOffset</span></span>|<span data-ttu-id="5c711-157">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="5c711-157">The date and time the app was last modified.</span></span> <span data-ttu-id="5c711-158">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c711-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c711-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="5c711-159">isFeatured</span></span>|<span data-ttu-id="5c711-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c711-160">Boolean</span></span>|<span data-ttu-id="5c711-161">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c711-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c711-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="5c711-162">privacyInformationUrl</span></span>|<span data-ttu-id="5c711-163">String</span><span class="sxs-lookup"><span data-stu-id="5c711-163">String</span></span>|<span data-ttu-id="5c711-164">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="5c711-164">The privacy statement Url.</span></span> <span data-ttu-id="5c711-165">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c711-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c711-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="5c711-166">informationUrl</span></span>|<span data-ttu-id="5c711-167">String</span><span class="sxs-lookup"><span data-stu-id="5c711-167">String</span></span>|<span data-ttu-id="5c711-168">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="5c711-168">The more information Url.</span></span> <span data-ttu-id="5c711-169">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c711-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c711-170">owner</span><span class="sxs-lookup"><span data-stu-id="5c711-170">owner</span></span>|<span data-ttu-id="5c711-171">String</span><span class="sxs-lookup"><span data-stu-id="5c711-171">String</span></span>|<span data-ttu-id="5c711-172">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="5c711-172">The owner of the app.</span></span> <span data-ttu-id="5c711-173">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c711-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c711-174">developer</span><span class="sxs-lookup"><span data-stu-id="5c711-174">developer</span></span>|<span data-ttu-id="5c711-175">String</span><span class="sxs-lookup"><span data-stu-id="5c711-175">String</span></span>|<span data-ttu-id="5c711-176">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="5c711-176">The developer of the app.</span></span> <span data-ttu-id="5c711-177">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c711-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c711-178">notes</span><span class="sxs-lookup"><span data-stu-id="5c711-178">notes</span></span>|<span data-ttu-id="5c711-179">String</span><span class="sxs-lookup"><span data-stu-id="5c711-179">String</span></span>|<span data-ttu-id="5c711-180">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="5c711-180">Notes for the app.</span></span> <span data-ttu-id="5c711-181">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5c711-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5c711-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="5c711-182">publishingState</span></span>|[<span data-ttu-id="5c711-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="5c711-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="5c711-184">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="5c711-184">The publishing state for the app.</span></span> <span data-ttu-id="5c711-185">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="5c711-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="5c711-186">[mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="5c711-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="5c711-187">可能な値は `notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="5c711-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="5c711-188">appUrl</span><span class="sxs-lookup"><span data-stu-id="5c711-188">appUrl</span></span>|<span data-ttu-id="5c711-189">String</span><span class="sxs-lookup"><span data-stu-id="5c711-189">String</span></span>|<span data-ttu-id="5c711-190">Web アプリの URL。</span><span class="sxs-lookup"><span data-stu-id="5c711-190">The web app URL.</span></span>|
|<span data-ttu-id="5c711-191">useManagedBrowser</span><span class="sxs-lookup"><span data-stu-id="5c711-191">useManagedBrowser</span></span>|<span data-ttu-id="5c711-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c711-192">Boolean</span></span>|<span data-ttu-id="5c711-193">管理対象のブラウザーを使用するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="5c711-193">Whether or not to use managed browser.</span></span> <span data-ttu-id="5c711-194">このプロパティは、Android と iOS にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="5c711-194">This property is only applicable for Android and IOS.</span></span>|



## <a name="response"></a><span data-ttu-id="5c711-195">応答</span><span class="sxs-lookup"><span data-stu-id="5c711-195">Response</span></span>
<span data-ttu-id="5c711-196">このメソッドが成功した場合、このメソッドは `200 OK` 応答コードと、更新された [webApp](../resources/intune-apps-webapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="5c711-196">If successful, this method returns a `200 OK` response code and an updated [webApp](../resources/intune-apps-webapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c711-197">例</span><span class="sxs-lookup"><span data-stu-id="5c711-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="5c711-198">要求</span><span class="sxs-lookup"><span data-stu-id="5c711-198">Request</span></span>
<span data-ttu-id="5c711-199">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5c711-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 645

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
  "publishingState": "processing",
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```

### <a name="response"></a><span data-ttu-id="5c711-200">応答</span><span class="sxs-lookup"><span data-stu-id="5c711-200">Response</span></span>
<span data-ttu-id="5c711-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5c711-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 817

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
  "publishingState": "processing",
  "appUrl": "https://example.com/appUrl/",
  "useManagedBrowser": true
}
```



