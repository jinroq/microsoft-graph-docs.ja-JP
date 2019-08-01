---
title: macOSOfficeSuiteApp の作成
description: 新しい macOSOfficeSuiteApp オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 07a2d810d55fe0734bb9c227405cd546e5e36ff4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36014215"
---
# <a name="create-macosofficesuiteapp"></a><span data-ttu-id="e07f2-103">macOSOfficeSuiteApp の作成</span><span class="sxs-lookup"><span data-stu-id="e07f2-103">Create macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="e07f2-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e07f2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e07f2-105">新しい [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e07f2-105">Create a new [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e07f2-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="e07f2-106">Prerequisites</span></span>
<span data-ttu-id="e07f2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e07f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e07f2-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e07f2-109">Permission type</span></span>|<span data-ttu-id="e07f2-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e07f2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e07f2-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e07f2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e07f2-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e07f2-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e07f2-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e07f2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e07f2-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e07f2-114">Not supported.</span></span>|
|<span data-ttu-id="e07f2-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e07f2-115">Application</span></span>|<span data-ttu-id="e07f2-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e07f2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e07f2-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e07f2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="e07f2-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e07f2-118">Request headers</span></span>
|<span data-ttu-id="e07f2-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e07f2-119">Header</span></span>|<span data-ttu-id="e07f2-120">値</span><span class="sxs-lookup"><span data-stu-id="e07f2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e07f2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e07f2-121">Authorization</span></span>|<span data-ttu-id="e07f2-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e07f2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e07f2-123">承諾</span><span class="sxs-lookup"><span data-stu-id="e07f2-123">Accept</span></span>|<span data-ttu-id="e07f2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e07f2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e07f2-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="e07f2-125">Request body</span></span>
<span data-ttu-id="e07f2-126">要求本文で、macOSOfficeSuiteApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e07f2-126">In the request body, supply a JSON representation for the macOSOfficeSuiteApp object.</span></span>

<span data-ttu-id="e07f2-127">次の表に、macOSOfficeSuiteApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e07f2-127">The following table shows the properties that are required when you create the macOSOfficeSuiteApp.</span></span>

|<span data-ttu-id="e07f2-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e07f2-128">Property</span></span>|<span data-ttu-id="e07f2-129">型</span><span class="sxs-lookup"><span data-stu-id="e07f2-129">Type</span></span>|<span data-ttu-id="e07f2-130">説明</span><span class="sxs-lookup"><span data-stu-id="e07f2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e07f2-131">id</span><span class="sxs-lookup"><span data-stu-id="e07f2-131">id</span></span>|<span data-ttu-id="e07f2-132">文字列</span><span class="sxs-lookup"><span data-stu-id="e07f2-132">String</span></span>|<span data-ttu-id="e07f2-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e07f2-133">Key of the entity.</span></span> <span data-ttu-id="e07f2-134">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e07f2-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e07f2-135">displayName</span><span class="sxs-lookup"><span data-stu-id="e07f2-135">displayName</span></span>|<span data-ttu-id="e07f2-136">文字列</span><span class="sxs-lookup"><span data-stu-id="e07f2-136">String</span></span>|<span data-ttu-id="e07f2-137">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="e07f2-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e07f2-138">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e07f2-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e07f2-139">description</span><span class="sxs-lookup"><span data-stu-id="e07f2-139">description</span></span>|<span data-ttu-id="e07f2-140">String</span><span class="sxs-lookup"><span data-stu-id="e07f2-140">String</span></span>|<span data-ttu-id="e07f2-141">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="e07f2-141">The description of the app.</span></span> <span data-ttu-id="e07f2-142">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e07f2-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e07f2-143">publisher</span><span class="sxs-lookup"><span data-stu-id="e07f2-143">publisher</span></span>|<span data-ttu-id="e07f2-144">String</span><span class="sxs-lookup"><span data-stu-id="e07f2-144">String</span></span>|<span data-ttu-id="e07f2-145">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="e07f2-145">The publisher of the app.</span></span> <span data-ttu-id="e07f2-146">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e07f2-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e07f2-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e07f2-147">largeIcon</span></span>|[<span data-ttu-id="e07f2-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e07f2-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e07f2-149">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="e07f2-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e07f2-150">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e07f2-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e07f2-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e07f2-151">createdDateTime</span></span>|<span data-ttu-id="e07f2-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e07f2-152">DateTimeOffset</span></span>|<span data-ttu-id="e07f2-153">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="e07f2-153">The date and time the app was created.</span></span> <span data-ttu-id="e07f2-154">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e07f2-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e07f2-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e07f2-155">lastModifiedDateTime</span></span>|<span data-ttu-id="e07f2-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e07f2-156">DateTimeOffset</span></span>|<span data-ttu-id="e07f2-157">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="e07f2-157">The date and time the app was last modified.</span></span> <span data-ttu-id="e07f2-158">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e07f2-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e07f2-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e07f2-159">isFeatured</span></span>|<span data-ttu-id="e07f2-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="e07f2-160">Boolean</span></span>|<span data-ttu-id="e07f2-161">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e07f2-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e07f2-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e07f2-162">privacyInformationUrl</span></span>|<span data-ttu-id="e07f2-163">String</span><span class="sxs-lookup"><span data-stu-id="e07f2-163">String</span></span>|<span data-ttu-id="e07f2-164">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="e07f2-164">The privacy statement Url.</span></span> <span data-ttu-id="e07f2-165">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e07f2-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e07f2-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e07f2-166">informationUrl</span></span>|<span data-ttu-id="e07f2-167">String</span><span class="sxs-lookup"><span data-stu-id="e07f2-167">String</span></span>|<span data-ttu-id="e07f2-168">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="e07f2-168">The more information Url.</span></span> <span data-ttu-id="e07f2-169">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e07f2-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e07f2-170">owner</span><span class="sxs-lookup"><span data-stu-id="e07f2-170">owner</span></span>|<span data-ttu-id="e07f2-171">String</span><span class="sxs-lookup"><span data-stu-id="e07f2-171">String</span></span>|<span data-ttu-id="e07f2-172">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="e07f2-172">The owner of the app.</span></span> <span data-ttu-id="e07f2-173">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e07f2-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e07f2-174">developer</span><span class="sxs-lookup"><span data-stu-id="e07f2-174">developer</span></span>|<span data-ttu-id="e07f2-175">String</span><span class="sxs-lookup"><span data-stu-id="e07f2-175">String</span></span>|<span data-ttu-id="e07f2-176">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="e07f2-176">The developer of the app.</span></span> <span data-ttu-id="e07f2-177">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e07f2-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e07f2-178">notes</span><span class="sxs-lookup"><span data-stu-id="e07f2-178">notes</span></span>|<span data-ttu-id="e07f2-179">String</span><span class="sxs-lookup"><span data-stu-id="e07f2-179">String</span></span>|<span data-ttu-id="e07f2-180">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="e07f2-180">Notes for the app.</span></span> <span data-ttu-id="e07f2-181">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e07f2-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e07f2-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="e07f2-182">publishingState</span></span>|[<span data-ttu-id="e07f2-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e07f2-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e07f2-184">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="e07f2-184">The publishing state for the app.</span></span> <span data-ttu-id="e07f2-185">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="e07f2-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e07f2-186">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="e07f2-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e07f2-187">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="e07f2-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|



## <a name="response"></a><span data-ttu-id="e07f2-188">応答</span><span class="sxs-lookup"><span data-stu-id="e07f2-188">Response</span></span>
<span data-ttu-id="e07f2-189">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e07f2-189">If successful, this method returns a `201 Created` response code and a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e07f2-190">例</span><span class="sxs-lookup"><span data-stu-id="e07f2-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="e07f2-191">要求</span><span class="sxs-lookup"><span data-stu-id="e07f2-191">Request</span></span>
<span data-ttu-id="e07f2-192">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e07f2-192">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e07f2-193">応答</span><span class="sxs-lookup"><span data-stu-id="e07f2-193">Response</span></span>
<span data-ttu-id="e07f2-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e07f2-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



