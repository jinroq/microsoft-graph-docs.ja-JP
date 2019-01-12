---
title: IntuneBrandingProfile を作成します。
description: 新しい intuneBrandingProfile オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 755de596da82aa2ef7a8d5bc142f43e6bf2ca4c8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964544"
---
# <a name="create-intunebrandingprofile"></a><span data-ttu-id="e3c34-103">IntuneBrandingProfile を作成します。</span><span class="sxs-lookup"><span data-stu-id="e3c34-103">Create intuneBrandingProfile</span></span>

> <span data-ttu-id="e3c34-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e3c34-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e3c34-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3c34-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e3c34-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e3c34-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e3c34-107">新しい[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e3c34-107">Create a new [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e3c34-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="e3c34-108">Prerequisites</span></span>
<span data-ttu-id="e3c34-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3c34-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3c34-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e3c34-111">Permission type</span></span>|<span data-ttu-id="e3c34-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e3c34-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3c34-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e3c34-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e3c34-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3c34-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e3c34-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e3c34-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3c34-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3c34-116">Not supported.</span></span>|
|<span data-ttu-id="e3c34-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e3c34-117">Application</span></span>|<span data-ttu-id="e3c34-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3c34-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3c34-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e3c34-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a><span data-ttu-id="e3c34-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3c34-120">Request headers</span></span>
|<span data-ttu-id="e3c34-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3c34-121">Header</span></span>|<span data-ttu-id="e3c34-122">値</span><span class="sxs-lookup"><span data-stu-id="e3c34-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3c34-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3c34-123">Authorization</span></span>|<span data-ttu-id="e3c34-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e3c34-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3c34-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e3c34-125">Accept</span></span>|<span data-ttu-id="e3c34-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e3c34-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3c34-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e3c34-127">Request body</span></span>
<span data-ttu-id="e3c34-128">要求の本文に intuneBrandingProfile オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="e3c34-128">In the request body, supply a JSON representation for the intuneBrandingProfile object.</span></span>

<span data-ttu-id="e3c34-129">次の表は、intuneBrandingProfile を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e3c34-129">The following table shows the properties that are required when you create the intuneBrandingProfile.</span></span>

|<span data-ttu-id="e3c34-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e3c34-130">Property</span></span>|<span data-ttu-id="e3c34-131">型</span><span class="sxs-lookup"><span data-stu-id="e3c34-131">Type</span></span>|<span data-ttu-id="e3c34-132">説明</span><span class="sxs-lookup"><span data-stu-id="e3c34-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3c34-133">ID</span><span class="sxs-lookup"><span data-stu-id="e3c34-133">id</span></span>|<span data-ttu-id="e3c34-134">String</span><span class="sxs-lookup"><span data-stu-id="e3c34-134">String</span></span>|<span data-ttu-id="e3c34-135">プロファイル キー</span><span class="sxs-lookup"><span data-stu-id="e3c34-135">Profile Key</span></span>|
|<span data-ttu-id="e3c34-136">profilename プロパティ</span><span class="sxs-lookup"><span data-stu-id="e3c34-136">profileName</span></span>|<span data-ttu-id="e3c34-137">String</span><span class="sxs-lookup"><span data-stu-id="e3c34-137">String</span></span>|<span data-ttu-id="e3c34-138">プロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="e3c34-138">Name of the profile</span></span>|
|<span data-ttu-id="e3c34-139">profileDescription</span><span class="sxs-lookup"><span data-stu-id="e3c34-139">profileDescription</span></span>|<span data-ttu-id="e3c34-140">String</span><span class="sxs-lookup"><span data-stu-id="e3c34-140">String</span></span>|<span data-ttu-id="e3c34-141">プロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="e3c34-141">Description of the profile</span></span>|
|<span data-ttu-id="e3c34-142">isDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="e3c34-142">isDefaultProfile</span></span>|<span data-ttu-id="e3c34-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3c34-143">Boolean</span></span>|<span data-ttu-id="e3c34-144">既定のプロファイルが使用される場合について説明します。</span><span class="sxs-lookup"><span data-stu-id="e3c34-144">Presents if the profile is used for default.</span></span>|
|<span data-ttu-id="e3c34-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e3c34-145">createdDateTime</span></span>|<span data-ttu-id="e3c34-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3c34-146">DateTimeOffset</span></span>|<span data-ttu-id="e3c34-147">BrandingProfile が作成された日時です。</span><span class="sxs-lookup"><span data-stu-id="e3c34-147">When the BrandingProfile was created.</span></span>|
|<span data-ttu-id="e3c34-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e3c34-148">lastModifiedDateTime</span></span>|<span data-ttu-id="e3c34-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3c34-149">DateTimeOffset</span></span>|<span data-ttu-id="e3c34-150">BrandingProfile の最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="e3c34-150">When the BrandingProfile was last modified.</span></span>|
|<span data-ttu-id="e3c34-151">displayName</span><span class="sxs-lookup"><span data-stu-id="e3c34-151">displayName</span></span>|<span data-ttu-id="e3c34-152">String</span><span class="sxs-lookup"><span data-stu-id="e3c34-152">String</span></span>|<span data-ttu-id="e3c34-153">エンド ユーザーに表示される会社名または組織名。</span><span class="sxs-lookup"><span data-stu-id="e3c34-153">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="e3c34-154">contactITName</span><span class="sxs-lookup"><span data-stu-id="e3c34-154">contactITName</span></span>|<span data-ttu-id="e3c34-155">String</span><span class="sxs-lookup"><span data-stu-id="e3c34-155">String</span></span>|<span data-ttu-id="e3c34-156">IT サポートを担当する個人名または組織名。</span><span class="sxs-lookup"><span data-stu-id="e3c34-156">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="e3c34-157">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="e3c34-157">contactITPhoneNumber</span></span>|<span data-ttu-id="e3c34-158">String</span><span class="sxs-lookup"><span data-stu-id="e3c34-158">String</span></span>|<span data-ttu-id="e3c34-159">IT サポートを担当する個人または組織の電話番号。</span><span class="sxs-lookup"><span data-stu-id="e3c34-159">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="e3c34-160">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="e3c34-160">contactITEmailAddress</span></span>|<span data-ttu-id="e3c34-161">String</span><span class="sxs-lookup"><span data-stu-id="e3c34-161">String</span></span>|<span data-ttu-id="e3c34-162">IT サポートを担当する個人または組織のメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="e3c34-162">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="e3c34-163">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="e3c34-163">contactITNotes</span></span>|<span data-ttu-id="e3c34-164">String</span><span class="sxs-lookup"><span data-stu-id="e3c34-164">String</span></span>|<span data-ttu-id="e3c34-165">IT サポートを担当する個人または組織に関するテキスト コメント。</span><span class="sxs-lookup"><span data-stu-id="e3c34-165">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="e3c34-166">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="e3c34-166">privacyUrl</span></span>|<span data-ttu-id="e3c34-167">String</span><span class="sxs-lookup"><span data-stu-id="e3c34-167">String</span></span>|<span data-ttu-id="e3c34-168">会社または組織のプライバシー ポリシーの URL。</span><span class="sxs-lookup"><span data-stu-id="e3c34-168">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="e3c34-169">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="e3c34-169">onlineSupportSiteUrl</span></span>|<span data-ttu-id="e3c34-170">String</span><span class="sxs-lookup"><span data-stu-id="e3c34-170">String</span></span>|<span data-ttu-id="e3c34-171">会社または組織の IT ヘルプデスク サイトの URL。</span><span class="sxs-lookup"><span data-stu-id="e3c34-171">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="e3c34-172">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="e3c34-172">onlineSupportSiteName</span></span>|<span data-ttu-id="e3c34-173">String</span><span class="sxs-lookup"><span data-stu-id="e3c34-173">String</span></span>|<span data-ttu-id="e3c34-174">会社または組織の IT ヘルプデスク サイトの表示名。</span><span class="sxs-lookup"><span data-stu-id="e3c34-174">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="e3c34-175">themeColor</span><span class="sxs-lookup"><span data-stu-id="e3c34-175">themeColor</span></span>|[<span data-ttu-id="e3c34-176">rgbColor</span><span class="sxs-lookup"><span data-stu-id="e3c34-176">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="e3c34-177">会社のポータル アプリケーションと Web ポータルで使用する主要なテーマの色。</span><span class="sxs-lookup"><span data-stu-id="e3c34-177">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="e3c34-178">showLogo</span><span class="sxs-lookup"><span data-stu-id="e3c34-178">showLogo</span></span>|<span data-ttu-id="e3c34-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3c34-179">Boolean</span></span>|<span data-ttu-id="e3c34-180">管理者が指定したロゴ画像が表示されるかどうかを表すブール値。</span><span class="sxs-lookup"><span data-stu-id="e3c34-180">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="e3c34-181">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="e3c34-181">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="e3c34-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3c34-182">Boolean</span></span>|<span data-ttu-id="e3c34-183">管理者が指定した表示名がロゴ画像のとなりに表示されるかどうかを表すブール値。</span><span class="sxs-lookup"><span data-stu-id="e3c34-183">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="e3c34-184">themeColorLogo</span><span class="sxs-lookup"><span data-stu-id="e3c34-184">themeColorLogo</span></span>|[<span data-ttu-id="e3c34-185">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e3c34-185">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e3c34-186">ロゴ イメージがテーマの背景色を会社のポータル アプリケーションに表示されます。</span><span class="sxs-lookup"><span data-stu-id="e3c34-186">Logo image displayed in Company Portal apps on theme color backgrounds.</span></span>|
|<span data-ttu-id="e3c34-187">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="e3c34-187">lightBackgroundLogo</span></span>|[<span data-ttu-id="e3c34-188">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e3c34-188">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e3c34-189">ロゴのイメージは明るい背景に会社のポータル アプリケーションに表示されます。</span><span class="sxs-lookup"><span data-stu-id="e3c34-189">Logo image displayed in Company Portal apps on light backgrounds.</span></span>|
|<span data-ttu-id="e3c34-190">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="e3c34-190">landingPageCustomizedImage</span></span>|[<span data-ttu-id="e3c34-191">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e3c34-191">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e3c34-192">会社のポータル アプリケーションのランディング ページに表示されるカスタムのイメージ</span><span class="sxs-lookup"><span data-stu-id="e3c34-192">Customized image displayed in Company Portal apps landing page</span></span>|



## <a name="response"></a><span data-ttu-id="e3c34-193">応答</span><span class="sxs-lookup"><span data-stu-id="e3c34-193">Response</span></span>
<span data-ttu-id="e3c34-194">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="e3c34-194">If successful, this method returns a `201 Created` response code and a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3c34-195">例</span><span class="sxs-lookup"><span data-stu-id="e3c34-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="e3c34-196">要求</span><span class="sxs-lookup"><span data-stu-id="e3c34-196">Request</span></span>
<span data-ttu-id="e3c34-197">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e3c34-197">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
Content-type: application/json
Content-length: 1269

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "contactITName": "Contact ITName value",
  "contactITPhoneNumber": "Contact ITPhone Number value",
  "contactITEmailAddress": "Contact ITEmail Address value",
  "contactITNotes": "Contact ITNotes value",
  "privacyUrl": "https://example.com/privacyUrl/",
  "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
  "onlineSupportSiteName": "Online Support Site Name value",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1,
    "g": 1,
    "b": 1
  },
  "showLogo": true,
  "showDisplayNameNextToLogo": true,
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```

### <a name="response"></a><span data-ttu-id="e3c34-198">応答</span><span class="sxs-lookup"><span data-stu-id="e3c34-198">Response</span></span>
<span data-ttu-id="e3c34-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e3c34-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1377

{
  "@odata.type": "#microsoft.graph.intuneBrandingProfile",
  "id": "fcd6136c-136c-fcd6-6c13-d6fc6c13d6fc",
  "profileName": "Profile Name value",
  "profileDescription": "Profile Description value",
  "isDefaultProfile": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "contactITName": "Contact ITName value",
  "contactITPhoneNumber": "Contact ITPhone Number value",
  "contactITEmailAddress": "Contact ITEmail Address value",
  "contactITNotes": "Contact ITNotes value",
  "privacyUrl": "https://example.com/privacyUrl/",
  "onlineSupportSiteUrl": "https://example.com/onlineSupportSiteUrl/",
  "onlineSupportSiteName": "Online Support Site Name value",
  "themeColor": {
    "@odata.type": "microsoft.graph.rgbColor",
    "r": 1,
    "g": 1,
    "b": 1
  },
  "showLogo": true,
  "showDisplayNameNextToLogo": true,
  "themeColorLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lightBackgroundLogo": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "landingPageCustomizedImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```





