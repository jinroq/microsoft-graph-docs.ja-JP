---
title: macOSOfficeSuiteApp の作成
description: 新しい macOSOfficeSuiteApp オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bf65f879832e4687ad3e784d0b09d7234c8920b8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840475"
---
# <a name="create-macosofficesuiteapp"></a><span data-ttu-id="72711-103">macOSOfficeSuiteApp の作成</span><span class="sxs-lookup"><span data-stu-id="72711-103">Create macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="72711-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="72711-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="72711-105">新しい [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="72711-105">Create a new [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="72711-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="72711-106">Prerequisites</span></span>
<span data-ttu-id="72711-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="72711-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72711-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="72711-109">Permission type</span></span>|<span data-ttu-id="72711-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="72711-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72711-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="72711-111">Delegated (work or school account)</span></span>|<span data-ttu-id="72711-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72711-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="72711-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="72711-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72711-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="72711-114">Not supported.</span></span>|
|<span data-ttu-id="72711-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="72711-115">Application</span></span>|<span data-ttu-id="72711-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="72711-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="72711-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="72711-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="72711-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="72711-118">Request headers</span></span>
|<span data-ttu-id="72711-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="72711-119">Header</span></span>|<span data-ttu-id="72711-120">値</span><span class="sxs-lookup"><span data-stu-id="72711-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72711-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="72711-121">Authorization</span></span>|<span data-ttu-id="72711-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="72711-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72711-123">Accept</span><span class="sxs-lookup"><span data-stu-id="72711-123">Accept</span></span>|<span data-ttu-id="72711-124">application/json</span><span class="sxs-lookup"><span data-stu-id="72711-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72711-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="72711-125">Request body</span></span>
<span data-ttu-id="72711-126">要求本文で、macOSOfficeSuiteApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="72711-126">In the request body, supply a JSON representation for the macOSOfficeSuiteApp object.</span></span>

<span data-ttu-id="72711-127">次の表に、macOSOfficeSuiteApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="72711-127">The following table shows the properties that are required when you create the macOSOfficeSuiteApp.</span></span>

|<span data-ttu-id="72711-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="72711-128">Property</span></span>|<span data-ttu-id="72711-129">種類</span><span class="sxs-lookup"><span data-stu-id="72711-129">Type</span></span>|<span data-ttu-id="72711-130">説明</span><span class="sxs-lookup"><span data-stu-id="72711-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72711-131">ID</span><span class="sxs-lookup"><span data-stu-id="72711-131">id</span></span>|<span data-ttu-id="72711-132">String</span><span class="sxs-lookup"><span data-stu-id="72711-132">String</span></span>|<span data-ttu-id="72711-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="72711-133">Key of the entity.</span></span> <span data-ttu-id="72711-134">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="72711-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="72711-135">displayName</span><span class="sxs-lookup"><span data-stu-id="72711-135">displayName</span></span>|<span data-ttu-id="72711-136">String</span><span class="sxs-lookup"><span data-stu-id="72711-136">String</span></span>|<span data-ttu-id="72711-137">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="72711-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="72711-138">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="72711-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="72711-139">説明</span><span class="sxs-lookup"><span data-stu-id="72711-139">description</span></span>|<span data-ttu-id="72711-140">String</span><span class="sxs-lookup"><span data-stu-id="72711-140">String</span></span>|<span data-ttu-id="72711-141">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="72711-141">The description of the app.</span></span> <span data-ttu-id="72711-142">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="72711-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="72711-143">publisher</span><span class="sxs-lookup"><span data-stu-id="72711-143">publisher</span></span>|<span data-ttu-id="72711-144">String</span><span class="sxs-lookup"><span data-stu-id="72711-144">String</span></span>|<span data-ttu-id="72711-145">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="72711-145">The publisher of the app.</span></span> <span data-ttu-id="72711-146">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="72711-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="72711-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="72711-147">largeIcon</span></span>|[<span data-ttu-id="72711-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="72711-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="72711-149">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="72711-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="72711-150">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="72711-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="72711-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="72711-151">createdDateTime</span></span>|<span data-ttu-id="72711-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72711-152">DateTimeOffset</span></span>|<span data-ttu-id="72711-153">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="72711-153">The date and time the app was created.</span></span> <span data-ttu-id="72711-154">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="72711-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="72711-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="72711-155">lastModifiedDateTime</span></span>|<span data-ttu-id="72711-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72711-156">DateTimeOffset</span></span>|<span data-ttu-id="72711-157">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="72711-157">The date and time the app was last modified.</span></span> <span data-ttu-id="72711-158">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="72711-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="72711-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="72711-159">isFeatured</span></span>|<span data-ttu-id="72711-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="72711-160">Boolean</span></span>|<span data-ttu-id="72711-161">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="72711-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="72711-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="72711-162">privacyInformationUrl</span></span>|<span data-ttu-id="72711-163">String</span><span class="sxs-lookup"><span data-stu-id="72711-163">String</span></span>|<span data-ttu-id="72711-164">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="72711-164">The privacy statement Url.</span></span> <span data-ttu-id="72711-165">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="72711-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="72711-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="72711-166">informationUrl</span></span>|<span data-ttu-id="72711-167">String</span><span class="sxs-lookup"><span data-stu-id="72711-167">String</span></span>|<span data-ttu-id="72711-168">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="72711-168">The more information Url.</span></span> <span data-ttu-id="72711-169">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="72711-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="72711-170">owner</span><span class="sxs-lookup"><span data-stu-id="72711-170">owner</span></span>|<span data-ttu-id="72711-171">String</span><span class="sxs-lookup"><span data-stu-id="72711-171">String</span></span>|<span data-ttu-id="72711-172">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="72711-172">The owner of the app.</span></span> <span data-ttu-id="72711-173">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="72711-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="72711-174">developer</span><span class="sxs-lookup"><span data-stu-id="72711-174">developer</span></span>|<span data-ttu-id="72711-175">String</span><span class="sxs-lookup"><span data-stu-id="72711-175">String</span></span>|<span data-ttu-id="72711-176">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="72711-176">The developer of the app.</span></span> <span data-ttu-id="72711-177">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="72711-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="72711-178">notes</span><span class="sxs-lookup"><span data-stu-id="72711-178">notes</span></span>|<span data-ttu-id="72711-179">String</span><span class="sxs-lookup"><span data-stu-id="72711-179">String</span></span>|<span data-ttu-id="72711-180">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="72711-180">Notes for the app.</span></span> <span data-ttu-id="72711-181">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="72711-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="72711-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="72711-182">publishingState</span></span>|[<span data-ttu-id="72711-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="72711-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="72711-184">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="72711-184">The publishing state for the app.</span></span> <span data-ttu-id="72711-185">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="72711-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="72711-186">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="72711-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="72711-187">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="72711-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|



## <a name="response"></a><span data-ttu-id="72711-188">応答</span><span class="sxs-lookup"><span data-stu-id="72711-188">Response</span></span>
<span data-ttu-id="72711-189">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="72711-189">If successful, this method returns a `201 Created` response code and a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72711-190">例</span><span class="sxs-lookup"><span data-stu-id="72711-190">Example</span></span>
### <a name="request"></a><span data-ttu-id="72711-191">要求</span><span class="sxs-lookup"><span data-stu-id="72711-191">Request</span></span>
<span data-ttu-id="72711-192">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="72711-192">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="72711-193">応答</span><span class="sxs-lookup"><span data-stu-id="72711-193">Response</span></span>
<span data-ttu-id="72711-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="72711-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



