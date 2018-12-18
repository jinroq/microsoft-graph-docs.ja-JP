---
title: macOSOfficeSuiteApp の作成
description: 新しい macOSOfficeSuiteApp オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 7d0f71c501e3645f0f8b4f89610094fa9b13dd2a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358871"
---
# <a name="create-macosofficesuiteapp"></a><span data-ttu-id="7e1e1-103">macOSOfficeSuiteApp の作成</span><span class="sxs-lookup"><span data-stu-id="7e1e1-103">Create macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="7e1e1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7e1e1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7e1e1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e1e1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7e1e1-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7e1e1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7e1e1-107">新しい [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7e1e1-107">Create a new [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7e1e1-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="7e1e1-108">Prerequisites</span></span>
<span data-ttu-id="7e1e1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7e1e1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e1e1-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7e1e1-111">Permission type</span></span>|<span data-ttu-id="7e1e1-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7e1e1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e1e1-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7e1e1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7e1e1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e1e1-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7e1e1-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7e1e1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e1e1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e1e1-116">Not supported.</span></span>|
|<span data-ttu-id="7e1e1-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7e1e1-117">Application</span></span>|<span data-ttu-id="7e1e1-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e1e1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e1e1-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7e1e1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="7e1e1-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7e1e1-120">Request headers</span></span>
|<span data-ttu-id="7e1e1-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7e1e1-121">Header</span></span>|<span data-ttu-id="7e1e1-122">値</span><span class="sxs-lookup"><span data-stu-id="7e1e1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e1e1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e1e1-123">Authorization</span></span>|<span data-ttu-id="7e1e1-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7e1e1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e1e1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7e1e1-125">Accept</span></span>|<span data-ttu-id="7e1e1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7e1e1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e1e1-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7e1e1-127">Request body</span></span>
<span data-ttu-id="7e1e1-128">要求本文で、macOSOfficeSuiteApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7e1e1-128">In the request body, supply a JSON representation for the macOSOfficeSuiteApp object.</span></span>

<span data-ttu-id="7e1e1-129">次の表に、macOSOfficeSuiteApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7e1e1-129">The following table shows the properties that are required when you create the macOSOfficeSuiteApp.</span></span>

|<span data-ttu-id="7e1e1-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7e1e1-130">Property</span></span>|<span data-ttu-id="7e1e1-131">種類</span><span class="sxs-lookup"><span data-stu-id="7e1e1-131">Type</span></span>|<span data-ttu-id="7e1e1-132">説明</span><span class="sxs-lookup"><span data-stu-id="7e1e1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e1e1-133">ID</span><span class="sxs-lookup"><span data-stu-id="7e1e1-133">id</span></span>|<span data-ttu-id="7e1e1-134">String</span><span class="sxs-lookup"><span data-stu-id="7e1e1-134">String</span></span>|<span data-ttu-id="7e1e1-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7e1e1-135">Key of the entity.</span></span> <span data-ttu-id="7e1e1-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e1e1-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e1e1-137">displayName</span><span class="sxs-lookup"><span data-stu-id="7e1e1-137">displayName</span></span>|<span data-ttu-id="7e1e1-138">String</span><span class="sxs-lookup"><span data-stu-id="7e1e1-138">String</span></span>|<span data-ttu-id="7e1e1-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="7e1e1-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="7e1e1-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e1e1-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e1e1-141">説明</span><span class="sxs-lookup"><span data-stu-id="7e1e1-141">description</span></span>|<span data-ttu-id="7e1e1-142">String</span><span class="sxs-lookup"><span data-stu-id="7e1e1-142">String</span></span>|<span data-ttu-id="7e1e1-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="7e1e1-143">The description of the app.</span></span> <span data-ttu-id="7e1e1-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e1e1-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e1e1-145">publisher</span><span class="sxs-lookup"><span data-stu-id="7e1e1-145">publisher</span></span>|<span data-ttu-id="7e1e1-146">String</span><span class="sxs-lookup"><span data-stu-id="7e1e1-146">String</span></span>|<span data-ttu-id="7e1e1-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="7e1e1-147">The publisher of the app.</span></span> <span data-ttu-id="7e1e1-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e1e1-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e1e1-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="7e1e1-149">largeIcon</span></span>|[<span data-ttu-id="7e1e1-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7e1e1-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="7e1e1-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="7e1e1-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="7e1e1-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e1e1-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e1e1-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7e1e1-153">createdDateTime</span></span>|<span data-ttu-id="7e1e1-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e1e1-154">DateTimeOffset</span></span>|<span data-ttu-id="7e1e1-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="7e1e1-155">The date and time the app was created.</span></span> <span data-ttu-id="7e1e1-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e1e1-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e1e1-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7e1e1-157">lastModifiedDateTime</span></span>|<span data-ttu-id="7e1e1-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e1e1-158">DateTimeOffset</span></span>|<span data-ttu-id="7e1e1-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="7e1e1-159">The date and time the app was last modified.</span></span> <span data-ttu-id="7e1e1-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e1e1-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e1e1-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="7e1e1-161">isFeatured</span></span>|<span data-ttu-id="7e1e1-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="7e1e1-162">Boolean</span></span>|<span data-ttu-id="7e1e1-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e1e1-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e1e1-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7e1e1-164">privacyInformationUrl</span></span>|<span data-ttu-id="7e1e1-165">String</span><span class="sxs-lookup"><span data-stu-id="7e1e1-165">String</span></span>|<span data-ttu-id="7e1e1-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="7e1e1-166">The privacy statement Url.</span></span> <span data-ttu-id="7e1e1-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e1e1-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e1e1-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7e1e1-168">informationUrl</span></span>|<span data-ttu-id="7e1e1-169">String</span><span class="sxs-lookup"><span data-stu-id="7e1e1-169">String</span></span>|<span data-ttu-id="7e1e1-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="7e1e1-170">The more information Url.</span></span> <span data-ttu-id="7e1e1-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e1e1-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e1e1-172">owner</span><span class="sxs-lookup"><span data-stu-id="7e1e1-172">owner</span></span>|<span data-ttu-id="7e1e1-173">String</span><span class="sxs-lookup"><span data-stu-id="7e1e1-173">String</span></span>|<span data-ttu-id="7e1e1-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="7e1e1-174">The owner of the app.</span></span> <span data-ttu-id="7e1e1-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e1e1-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e1e1-176">developer</span><span class="sxs-lookup"><span data-stu-id="7e1e1-176">developer</span></span>|<span data-ttu-id="7e1e1-177">String</span><span class="sxs-lookup"><span data-stu-id="7e1e1-177">String</span></span>|<span data-ttu-id="7e1e1-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="7e1e1-178">The developer of the app.</span></span> <span data-ttu-id="7e1e1-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e1e1-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e1e1-180">notes</span><span class="sxs-lookup"><span data-stu-id="7e1e1-180">notes</span></span>|<span data-ttu-id="7e1e1-181">String</span><span class="sxs-lookup"><span data-stu-id="7e1e1-181">String</span></span>|<span data-ttu-id="7e1e1-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="7e1e1-182">Notes for the app.</span></span> <span data-ttu-id="7e1e1-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e1e1-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e1e1-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="7e1e1-184">uploadState</span></span>|<span data-ttu-id="7e1e1-185">Int32</span><span class="sxs-lookup"><span data-stu-id="7e1e1-185">Int32</span></span>|<span data-ttu-id="7e1e1-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="7e1e1-186">The upload state.</span></span> <span data-ttu-id="7e1e1-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7e1e1-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7e1e1-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="7e1e1-188">publishingState</span></span>|[<span data-ttu-id="7e1e1-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="7e1e1-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="7e1e1-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="7e1e1-190">The publishing state for the app.</span></span> <span data-ttu-id="7e1e1-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="7e1e1-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="7e1e1-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="7e1e1-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="7e1e1-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="7e1e1-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|



## <a name="response"></a><span data-ttu-id="7e1e1-194">応答</span><span class="sxs-lookup"><span data-stu-id="7e1e1-194">Response</span></span>
<span data-ttu-id="7e1e1-195">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7e1e1-195">If successful, this method returns a `201 Created` response code and a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e1e1-196">例</span><span class="sxs-lookup"><span data-stu-id="7e1e1-196">Example</span></span>
### <a name="request"></a><span data-ttu-id="7e1e1-197">要求</span><span class="sxs-lookup"><span data-stu-id="7e1e1-197">Request</span></span>
<span data-ttu-id="7e1e1-198">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7e1e1-198">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 670

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
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing"
}
```

### <a name="response"></a><span data-ttu-id="7e1e1-199">応答</span><span class="sxs-lookup"><span data-stu-id="7e1e1-199">Response</span></span>
<span data-ttu-id="7e1e1-p117">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7e1e1-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 778

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
  "publishingState": "processing"
}
```





