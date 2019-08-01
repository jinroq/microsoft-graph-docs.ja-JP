---
title: macOSOfficeSuiteApp の更新
description: macOSOfficeSuiteApp オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 29da7eb0d4f3a54bef8b5141aeb43d383853de57
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36014173"
---
# <a name="update-macosofficesuiteapp"></a><span data-ttu-id="be07c-103">macOSOfficeSuiteApp の更新</span><span class="sxs-lookup"><span data-stu-id="be07c-103">Update macOSOfficeSuiteApp</span></span>

> <span data-ttu-id="be07c-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="be07c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be07c-105">[macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="be07c-105">Update the properties of a [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="be07c-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="be07c-106">Prerequisites</span></span>
<span data-ttu-id="be07c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="be07c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="be07c-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="be07c-109">Permission type</span></span>|<span data-ttu-id="be07c-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="be07c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="be07c-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="be07c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="be07c-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="be07c-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="be07c-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="be07c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="be07c-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be07c-114">Not supported.</span></span>|
|<span data-ttu-id="be07c-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="be07c-115">Application</span></span>|<span data-ttu-id="be07c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be07c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="be07c-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="be07c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="be07c-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="be07c-118">Request headers</span></span>
|<span data-ttu-id="be07c-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="be07c-119">Header</span></span>|<span data-ttu-id="be07c-120">値</span><span class="sxs-lookup"><span data-stu-id="be07c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="be07c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="be07c-121">Authorization</span></span>|<span data-ttu-id="be07c-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="be07c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="be07c-123">承諾</span><span class="sxs-lookup"><span data-stu-id="be07c-123">Accept</span></span>|<span data-ttu-id="be07c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="be07c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="be07c-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="be07c-125">Request body</span></span>
<span data-ttu-id="be07c-126">要求本文で、[macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="be07c-126">In the request body, supply a JSON representation for the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object.</span></span>

<span data-ttu-id="be07c-127">次の表に、[macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="be07c-127">The following table shows the properties that are required when you create the [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md).</span></span>

|<span data-ttu-id="be07c-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be07c-128">Property</span></span>|<span data-ttu-id="be07c-129">型</span><span class="sxs-lookup"><span data-stu-id="be07c-129">Type</span></span>|<span data-ttu-id="be07c-130">説明</span><span class="sxs-lookup"><span data-stu-id="be07c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be07c-131">id</span><span class="sxs-lookup"><span data-stu-id="be07c-131">id</span></span>|<span data-ttu-id="be07c-132">文字列</span><span class="sxs-lookup"><span data-stu-id="be07c-132">String</span></span>|<span data-ttu-id="be07c-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="be07c-133">Key of the entity.</span></span> <span data-ttu-id="be07c-134">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="be07c-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be07c-135">displayName</span><span class="sxs-lookup"><span data-stu-id="be07c-135">displayName</span></span>|<span data-ttu-id="be07c-136">文字列</span><span class="sxs-lookup"><span data-stu-id="be07c-136">String</span></span>|<span data-ttu-id="be07c-137">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="be07c-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="be07c-138">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="be07c-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be07c-139">description</span><span class="sxs-lookup"><span data-stu-id="be07c-139">description</span></span>|<span data-ttu-id="be07c-140">String</span><span class="sxs-lookup"><span data-stu-id="be07c-140">String</span></span>|<span data-ttu-id="be07c-141">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="be07c-141">The description of the app.</span></span> <span data-ttu-id="be07c-142">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="be07c-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be07c-143">publisher</span><span class="sxs-lookup"><span data-stu-id="be07c-143">publisher</span></span>|<span data-ttu-id="be07c-144">String</span><span class="sxs-lookup"><span data-stu-id="be07c-144">String</span></span>|<span data-ttu-id="be07c-145">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="be07c-145">The publisher of the app.</span></span> <span data-ttu-id="be07c-146">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="be07c-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be07c-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="be07c-147">largeIcon</span></span>|[<span data-ttu-id="be07c-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="be07c-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="be07c-149">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="be07c-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="be07c-150">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="be07c-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be07c-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="be07c-151">createdDateTime</span></span>|<span data-ttu-id="be07c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be07c-152">DateTimeOffset</span></span>|<span data-ttu-id="be07c-153">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="be07c-153">The date and time the app was created.</span></span> <span data-ttu-id="be07c-154">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="be07c-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be07c-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="be07c-155">lastModifiedDateTime</span></span>|<span data-ttu-id="be07c-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be07c-156">DateTimeOffset</span></span>|<span data-ttu-id="be07c-157">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="be07c-157">The date and time the app was last modified.</span></span> <span data-ttu-id="be07c-158">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="be07c-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be07c-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="be07c-159">isFeatured</span></span>|<span data-ttu-id="be07c-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="be07c-160">Boolean</span></span>|<span data-ttu-id="be07c-161">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="be07c-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be07c-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="be07c-162">privacyInformationUrl</span></span>|<span data-ttu-id="be07c-163">String</span><span class="sxs-lookup"><span data-stu-id="be07c-163">String</span></span>|<span data-ttu-id="be07c-164">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="be07c-164">The privacy statement Url.</span></span> <span data-ttu-id="be07c-165">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="be07c-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be07c-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="be07c-166">informationUrl</span></span>|<span data-ttu-id="be07c-167">String</span><span class="sxs-lookup"><span data-stu-id="be07c-167">String</span></span>|<span data-ttu-id="be07c-168">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="be07c-168">The more information Url.</span></span> <span data-ttu-id="be07c-169">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="be07c-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be07c-170">owner</span><span class="sxs-lookup"><span data-stu-id="be07c-170">owner</span></span>|<span data-ttu-id="be07c-171">String</span><span class="sxs-lookup"><span data-stu-id="be07c-171">String</span></span>|<span data-ttu-id="be07c-172">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="be07c-172">The owner of the app.</span></span> <span data-ttu-id="be07c-173">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="be07c-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be07c-174">developer</span><span class="sxs-lookup"><span data-stu-id="be07c-174">developer</span></span>|<span data-ttu-id="be07c-175">String</span><span class="sxs-lookup"><span data-stu-id="be07c-175">String</span></span>|<span data-ttu-id="be07c-176">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="be07c-176">The developer of the app.</span></span> <span data-ttu-id="be07c-177">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="be07c-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be07c-178">notes</span><span class="sxs-lookup"><span data-stu-id="be07c-178">notes</span></span>|<span data-ttu-id="be07c-179">String</span><span class="sxs-lookup"><span data-stu-id="be07c-179">String</span></span>|<span data-ttu-id="be07c-180">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="be07c-180">Notes for the app.</span></span> <span data-ttu-id="be07c-181">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="be07c-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="be07c-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="be07c-182">publishingState</span></span>|[<span data-ttu-id="be07c-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="be07c-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="be07c-184">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="be07c-184">The publishing state for the app.</span></span> <span data-ttu-id="be07c-185">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="be07c-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="be07c-186">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="be07c-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="be07c-187">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="be07c-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|



## <a name="response"></a><span data-ttu-id="be07c-188">応答</span><span class="sxs-lookup"><span data-stu-id="be07c-188">Response</span></span>
<span data-ttu-id="be07c-189">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="be07c-189">If successful, this method returns a `200 OK` response code and an updated [macOSOfficeSuiteApp](../resources/intune-apps-macosofficesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="be07c-190">例</span><span class="sxs-lookup"><span data-stu-id="be07c-190">Example</span></span>

### <a name="request"></a><span data-ttu-id="be07c-191">要求</span><span class="sxs-lookup"><span data-stu-id="be07c-191">Request</span></span>
<span data-ttu-id="be07c-192">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="be07c-192">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="be07c-193">応答</span><span class="sxs-lookup"><span data-stu-id="be07c-193">Response</span></span>
<span data-ttu-id="be07c-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="be07c-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



