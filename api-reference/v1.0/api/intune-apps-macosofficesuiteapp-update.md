---
title: macOSOfficeSuiteApp の更新
description: macOSOfficeSuiteApp オブジェクトのプロパティを更新します。
ms.openlocfilehash: a7747c4b4bd4325a2a39477de9d2593bb436024b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022900"
---
# <a name="update-macosofficesuiteapp"></a><span data-ttu-id="ce25f-103">macOSOfficeSuiteApp の更新</span><span class="sxs-lookup"><span data-stu-id="ce25f-103">Update macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="ce25f-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ce25f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ce25f-105">[macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ce25f-105">Update the properties of a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ce25f-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="ce25f-106">Prerequisites</span></span>
<span data-ttu-id="ce25f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ce25f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce25f-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ce25f-109">Permission type</span></span>|<span data-ttu-id="ce25f-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ce25f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce25f-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ce25f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ce25f-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce25f-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ce25f-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ce25f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce25f-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce25f-114">Not supported.</span></span>|
|<span data-ttu-id="ce25f-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ce25f-115">Application</span></span>|<span data-ttu-id="ce25f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce25f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce25f-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ce25f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="ce25f-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ce25f-118">Request headers</span></span>
|<span data-ttu-id="ce25f-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ce25f-119">Header</span></span>|<span data-ttu-id="ce25f-120">値</span><span class="sxs-lookup"><span data-stu-id="ce25f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce25f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce25f-121">Authorization</span></span>|<span data-ttu-id="ce25f-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ce25f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce25f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ce25f-123">Accept</span></span>|<span data-ttu-id="ce25f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ce25f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce25f-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="ce25f-125">Request body</span></span>
<span data-ttu-id="ce25f-126">要求本文で、[macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ce25f-126">In the request body, supply a JSON representation for the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

<span data-ttu-id="ce25f-127">次の表に、[macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ce25f-127">The following table shows the properties that are required when you create the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span></span>

|<span data-ttu-id="ce25f-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce25f-128">Property</span></span>|<span data-ttu-id="ce25f-129">型</span><span class="sxs-lookup"><span data-stu-id="ce25f-129">Type</span></span>|<span data-ttu-id="ce25f-130">説明</span><span class="sxs-lookup"><span data-stu-id="ce25f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce25f-131">id</span><span class="sxs-lookup"><span data-stu-id="ce25f-131">id</span></span>|<span data-ttu-id="ce25f-132">String</span><span class="sxs-lookup"><span data-stu-id="ce25f-132">String</span></span>|<span data-ttu-id="ce25f-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ce25f-133">Key of the entity.</span></span> <span data-ttu-id="ce25f-134">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce25f-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce25f-135">displayName</span><span class="sxs-lookup"><span data-stu-id="ce25f-135">displayName</span></span>|<span data-ttu-id="ce25f-136">String</span><span class="sxs-lookup"><span data-stu-id="ce25f-136">String</span></span>|<span data-ttu-id="ce25f-137">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="ce25f-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ce25f-138">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce25f-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce25f-139">説明</span><span class="sxs-lookup"><span data-stu-id="ce25f-139">description</span></span>|<span data-ttu-id="ce25f-140">String</span><span class="sxs-lookup"><span data-stu-id="ce25f-140">String</span></span>|<span data-ttu-id="ce25f-141">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="ce25f-141">The description of the app.</span></span> <span data-ttu-id="ce25f-142">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce25f-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce25f-143">publisher</span><span class="sxs-lookup"><span data-stu-id="ce25f-143">publisher</span></span>|<span data-ttu-id="ce25f-144">String</span><span class="sxs-lookup"><span data-stu-id="ce25f-144">String</span></span>|<span data-ttu-id="ce25f-145">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="ce25f-145">The publisher of the app.</span></span> <span data-ttu-id="ce25f-146">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce25f-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce25f-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ce25f-147">largeIcon</span></span>|[<span data-ttu-id="ce25f-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ce25f-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ce25f-149">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="ce25f-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ce25f-150">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce25f-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce25f-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ce25f-151">createdDateTime</span></span>|<span data-ttu-id="ce25f-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce25f-152">DateTimeOffset</span></span>|<span data-ttu-id="ce25f-153">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="ce25f-153">The date and time the app was created.</span></span> <span data-ttu-id="ce25f-154">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce25f-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce25f-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce25f-155">lastModifiedDateTime</span></span>|<span data-ttu-id="ce25f-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce25f-156">DateTimeOffset</span></span>|<span data-ttu-id="ce25f-157">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="ce25f-157">The date and time the app was last modified.</span></span> <span data-ttu-id="ce25f-158">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce25f-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce25f-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ce25f-159">isFeatured</span></span>|<span data-ttu-id="ce25f-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce25f-160">Boolean</span></span>|<span data-ttu-id="ce25f-161">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce25f-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce25f-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ce25f-162">privacyInformationUrl</span></span>|<span data-ttu-id="ce25f-163">String</span><span class="sxs-lookup"><span data-stu-id="ce25f-163">String</span></span>|<span data-ttu-id="ce25f-164">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="ce25f-164">The privacy statement Url.</span></span> <span data-ttu-id="ce25f-165">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce25f-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce25f-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ce25f-166">informationUrl</span></span>|<span data-ttu-id="ce25f-167">String</span><span class="sxs-lookup"><span data-stu-id="ce25f-167">String</span></span>|<span data-ttu-id="ce25f-168">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="ce25f-168">The more information Url.</span></span> <span data-ttu-id="ce25f-169">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce25f-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce25f-170">owner</span><span class="sxs-lookup"><span data-stu-id="ce25f-170">owner</span></span>|<span data-ttu-id="ce25f-171">String</span><span class="sxs-lookup"><span data-stu-id="ce25f-171">String</span></span>|<span data-ttu-id="ce25f-172">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="ce25f-172">The owner of the app.</span></span> <span data-ttu-id="ce25f-173">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce25f-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce25f-174">developer</span><span class="sxs-lookup"><span data-stu-id="ce25f-174">developer</span></span>|<span data-ttu-id="ce25f-175">String</span><span class="sxs-lookup"><span data-stu-id="ce25f-175">String</span></span>|<span data-ttu-id="ce25f-176">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="ce25f-176">The developer of the app.</span></span> <span data-ttu-id="ce25f-177">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce25f-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce25f-178">notes</span><span class="sxs-lookup"><span data-stu-id="ce25f-178">notes</span></span>|<span data-ttu-id="ce25f-179">String</span><span class="sxs-lookup"><span data-stu-id="ce25f-179">String</span></span>|<span data-ttu-id="ce25f-180">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="ce25f-180">Notes for the app.</span></span> <span data-ttu-id="ce25f-181">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce25f-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ce25f-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="ce25f-182">publishingState</span></span>|[<span data-ttu-id="ce25f-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ce25f-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ce25f-184">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="ce25f-184">The publishing state for the app.</span></span> <span data-ttu-id="ce25f-185">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="ce25f-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ce25f-186">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="ce25f-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="ce25f-187">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="ce25f-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|



## <a name="response"></a><span data-ttu-id="ce25f-188">応答</span><span class="sxs-lookup"><span data-stu-id="ce25f-188">Response</span></span>
<span data-ttu-id="ce25f-189">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ce25f-189">If successful, this method returns a `200 OK` response code and an updated [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce25f-190">例</span><span class="sxs-lookup"><span data-stu-id="ce25f-190">Example</span></span>
### <a name="request"></a><span data-ttu-id="ce25f-191">要求</span><span class="sxs-lookup"><span data-stu-id="ce25f-191">Request</span></span>
<span data-ttu-id="ce25f-192">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ce25f-192">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 584

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
  "publishingState": "processing"
}
```

### <a name="response"></a><span data-ttu-id="ce25f-193">応答</span><span class="sxs-lookup"><span data-stu-id="ce25f-193">Response</span></span>
<span data-ttu-id="ce25f-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ce25f-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 756

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
  "publishingState": "processing"
}
```



