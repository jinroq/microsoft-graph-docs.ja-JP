---
title: IntuneBrandingProfile を更新します。
description: IntuneBrandingProfile オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: c4321b0197e30126c4d83371a31425af1d8e73bd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309948"
---
# <a name="update-intunebrandingprofile"></a><span data-ttu-id="f95b6-103">IntuneBrandingProfile を更新します。</span><span class="sxs-lookup"><span data-stu-id="f95b6-103">Update intuneBrandingProfile</span></span>

> <span data-ttu-id="f95b6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f95b6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f95b6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f95b6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f95b6-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f95b6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f95b6-107">[IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f95b6-107">Update the properties of a [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f95b6-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="f95b6-108">Prerequisites</span></span>
<span data-ttu-id="f95b6-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f95b6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f95b6-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f95b6-111">Permission type</span></span>|<span data-ttu-id="f95b6-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f95b6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f95b6-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f95b6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f95b6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f95b6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f95b6-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f95b6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f95b6-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f95b6-116">Not supported.</span></span>|
|<span data-ttu-id="f95b6-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f95b6-117">Application</span></span>|<span data-ttu-id="f95b6-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f95b6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f95b6-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f95b6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="f95b6-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f95b6-120">Request headers</span></span>
|<span data-ttu-id="f95b6-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f95b6-121">Header</span></span>|<span data-ttu-id="f95b6-122">値</span><span class="sxs-lookup"><span data-stu-id="f95b6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f95b6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f95b6-123">Authorization</span></span>|<span data-ttu-id="f95b6-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f95b6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f95b6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f95b6-125">Accept</span></span>|<span data-ttu-id="f95b6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f95b6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f95b6-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f95b6-127">Request body</span></span>
<span data-ttu-id="f95b6-128">要求の本文に[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="f95b6-128">In the request body, supply a JSON representation for the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>

<span data-ttu-id="f95b6-129">[IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="f95b6-129">The following table shows the properties that are required when you create the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md).</span></span>

|<span data-ttu-id="f95b6-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f95b6-130">Property</span></span>|<span data-ttu-id="f95b6-131">種類</span><span class="sxs-lookup"><span data-stu-id="f95b6-131">Type</span></span>|<span data-ttu-id="f95b6-132">説明</span><span class="sxs-lookup"><span data-stu-id="f95b6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f95b6-133">ID</span><span class="sxs-lookup"><span data-stu-id="f95b6-133">id</span></span>|<span data-ttu-id="f95b6-134">String</span><span class="sxs-lookup"><span data-stu-id="f95b6-134">String</span></span>|<span data-ttu-id="f95b6-135">プロファイル キー</span><span class="sxs-lookup"><span data-stu-id="f95b6-135">Profile Key</span></span>|
|<span data-ttu-id="f95b6-136">profilename プロパティ</span><span class="sxs-lookup"><span data-stu-id="f95b6-136">profileName</span></span>|<span data-ttu-id="f95b6-137">String</span><span class="sxs-lookup"><span data-stu-id="f95b6-137">String</span></span>|<span data-ttu-id="f95b6-138">プロファイルの名前</span><span class="sxs-lookup"><span data-stu-id="f95b6-138">Name of the profile</span></span>|
|<span data-ttu-id="f95b6-139">profileDescription</span><span class="sxs-lookup"><span data-stu-id="f95b6-139">profileDescription</span></span>|<span data-ttu-id="f95b6-140">String</span><span class="sxs-lookup"><span data-stu-id="f95b6-140">String</span></span>|<span data-ttu-id="f95b6-141">プロファイルの説明</span><span class="sxs-lookup"><span data-stu-id="f95b6-141">Description of the profile</span></span>|
|<span data-ttu-id="f95b6-142">isDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="f95b6-142">isDefaultProfile</span></span>|<span data-ttu-id="f95b6-143">ブール型</span><span class="sxs-lookup"><span data-stu-id="f95b6-143">Boolean</span></span>|<span data-ttu-id="f95b6-144">既定のプロファイルが使用される場合について説明します。</span><span class="sxs-lookup"><span data-stu-id="f95b6-144">Presents if the profile is used for default.</span></span>|
|<span data-ttu-id="f95b6-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f95b6-145">createdDateTime</span></span>|<span data-ttu-id="f95b6-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f95b6-146">DateTimeOffset</span></span>|<span data-ttu-id="f95b6-147">BrandingProfile が作成された日時です。</span><span class="sxs-lookup"><span data-stu-id="f95b6-147">When the BrandingProfile was created.</span></span>|
|<span data-ttu-id="f95b6-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f95b6-148">lastModifiedDateTime</span></span>|<span data-ttu-id="f95b6-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f95b6-149">DateTimeOffset</span></span>|<span data-ttu-id="f95b6-150">BrandingProfile の最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="f95b6-150">When the BrandingProfile was last modified.</span></span>|
|<span data-ttu-id="f95b6-151">displayName</span><span class="sxs-lookup"><span data-stu-id="f95b6-151">displayName</span></span>|<span data-ttu-id="f95b6-152">String</span><span class="sxs-lookup"><span data-stu-id="f95b6-152">String</span></span>|<span data-ttu-id="f95b6-153">エンド ユーザーに表示される会社名または組織名。</span><span class="sxs-lookup"><span data-stu-id="f95b6-153">Company/organization name that is displayed to end users.</span></span>|
|<span data-ttu-id="f95b6-154">contactITName</span><span class="sxs-lookup"><span data-stu-id="f95b6-154">contactITName</span></span>|<span data-ttu-id="f95b6-155">String</span><span class="sxs-lookup"><span data-stu-id="f95b6-155">String</span></span>|<span data-ttu-id="f95b6-156">IT サポートを担当する個人名または組織名。</span><span class="sxs-lookup"><span data-stu-id="f95b6-156">Name of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="f95b6-157">contactITPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="f95b6-157">contactITPhoneNumber</span></span>|<span data-ttu-id="f95b6-158">String</span><span class="sxs-lookup"><span data-stu-id="f95b6-158">String</span></span>|<span data-ttu-id="f95b6-159">IT サポートを担当する個人または組織の電話番号。</span><span class="sxs-lookup"><span data-stu-id="f95b6-159">Phone number of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="f95b6-160">contactITEmailAddress</span><span class="sxs-lookup"><span data-stu-id="f95b6-160">contactITEmailAddress</span></span>|<span data-ttu-id="f95b6-161">String</span><span class="sxs-lookup"><span data-stu-id="f95b6-161">String</span></span>|<span data-ttu-id="f95b6-162">IT サポートを担当する個人または組織のメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="f95b6-162">Email address of the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="f95b6-163">contactITNotes</span><span class="sxs-lookup"><span data-stu-id="f95b6-163">contactITNotes</span></span>|<span data-ttu-id="f95b6-164">String</span><span class="sxs-lookup"><span data-stu-id="f95b6-164">String</span></span>|<span data-ttu-id="f95b6-165">IT サポートを担当する個人または組織に関するテキスト コメント。</span><span class="sxs-lookup"><span data-stu-id="f95b6-165">Text comments regarding the person/organization responsible for IT support.</span></span>|
|<span data-ttu-id="f95b6-166">privacyUrl</span><span class="sxs-lookup"><span data-stu-id="f95b6-166">privacyUrl</span></span>|<span data-ttu-id="f95b6-167">String</span><span class="sxs-lookup"><span data-stu-id="f95b6-167">String</span></span>|<span data-ttu-id="f95b6-168">会社または組織のプライバシー ポリシーの URL。</span><span class="sxs-lookup"><span data-stu-id="f95b6-168">URL to the company/organization’s privacy policy.</span></span>|
|<span data-ttu-id="f95b6-169">onlineSupportSiteUrl</span><span class="sxs-lookup"><span data-stu-id="f95b6-169">onlineSupportSiteUrl</span></span>|<span data-ttu-id="f95b6-170">String</span><span class="sxs-lookup"><span data-stu-id="f95b6-170">String</span></span>|<span data-ttu-id="f95b6-171">会社または組織の IT ヘルプデスク サイトの URL。</span><span class="sxs-lookup"><span data-stu-id="f95b6-171">URL to the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="f95b6-172">onlineSupportSiteName</span><span class="sxs-lookup"><span data-stu-id="f95b6-172">onlineSupportSiteName</span></span>|<span data-ttu-id="f95b6-173">String</span><span class="sxs-lookup"><span data-stu-id="f95b6-173">String</span></span>|<span data-ttu-id="f95b6-174">会社または組織の IT ヘルプデスク サイトの表示名。</span><span class="sxs-lookup"><span data-stu-id="f95b6-174">Display name of the company/organization’s IT helpdesk site.</span></span>|
|<span data-ttu-id="f95b6-175">themeColor</span><span class="sxs-lookup"><span data-stu-id="f95b6-175">themeColor</span></span>|[<span data-ttu-id="f95b6-176">rgbColor</span><span class="sxs-lookup"><span data-stu-id="f95b6-176">rgbColor</span></span>](../resources/intune-shared-rgbcolor.md)|<span data-ttu-id="f95b6-177">会社のポータル アプリケーションと Web ポータルで使用する主要なテーマの色。</span><span class="sxs-lookup"><span data-stu-id="f95b6-177">Primary theme color used in the Company Portal applications and web portal.</span></span>|
|<span data-ttu-id="f95b6-178">showLogo</span><span class="sxs-lookup"><span data-stu-id="f95b6-178">showLogo</span></span>|<span data-ttu-id="f95b6-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="f95b6-179">Boolean</span></span>|<span data-ttu-id="f95b6-180">管理者が指定したロゴ画像が表示されるかどうかを表すブール値。</span><span class="sxs-lookup"><span data-stu-id="f95b6-180">Boolean that represents whether the administrator-supplied logo images are shown or not shown.</span></span>|
|<span data-ttu-id="f95b6-181">showDisplayNameNextToLogo</span><span class="sxs-lookup"><span data-stu-id="f95b6-181">showDisplayNameNextToLogo</span></span>|<span data-ttu-id="f95b6-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="f95b6-182">Boolean</span></span>|<span data-ttu-id="f95b6-183">管理者が指定した表示名がロゴ画像のとなりに表示されるかどうかを表すブール値。</span><span class="sxs-lookup"><span data-stu-id="f95b6-183">Boolean that represents whether the administrator-supplied display name will be shown next to the logo image.</span></span>|
|<span data-ttu-id="f95b6-184">themeColorLogo</span><span class="sxs-lookup"><span data-stu-id="f95b6-184">themeColorLogo</span></span>|[<span data-ttu-id="f95b6-185">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f95b6-185">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f95b6-186">ロゴ イメージがテーマの背景色を会社のポータル アプリケーションに表示されます。</span><span class="sxs-lookup"><span data-stu-id="f95b6-186">Logo image displayed in Company Portal apps on theme color backgrounds.</span></span>|
|<span data-ttu-id="f95b6-187">lightBackgroundLogo</span><span class="sxs-lookup"><span data-stu-id="f95b6-187">lightBackgroundLogo</span></span>|[<span data-ttu-id="f95b6-188">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f95b6-188">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f95b6-189">ロゴのイメージは明るい背景に会社のポータル アプリケーションに表示されます。</span><span class="sxs-lookup"><span data-stu-id="f95b6-189">Logo image displayed in Company Portal apps on light backgrounds.</span></span>|
|<span data-ttu-id="f95b6-190">landingPageCustomizedImage</span><span class="sxs-lookup"><span data-stu-id="f95b6-190">landingPageCustomizedImage</span></span>|[<span data-ttu-id="f95b6-191">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f95b6-191">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f95b6-192">会社のポータル アプリケーションのランディング ページに表示されるカスタムのイメージ</span><span class="sxs-lookup"><span data-stu-id="f95b6-192">Customized image displayed in Company Portal apps landing page</span></span>|



## <a name="response"></a><span data-ttu-id="f95b6-193">応答</span><span class="sxs-lookup"><span data-stu-id="f95b6-193">Response</span></span>
<span data-ttu-id="f95b6-194">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="f95b6-194">If successful, this method returns a `200 OK` response code and an updated [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f95b6-195">例</span><span class="sxs-lookup"><span data-stu-id="f95b6-195">Example</span></span>
### <a name="request"></a><span data-ttu-id="f95b6-196">要求</span><span class="sxs-lookup"><span data-stu-id="f95b6-196">Request</span></span>
<span data-ttu-id="f95b6-197">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f95b6-197">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
Content-type: application/json
Content-length: 1209

{
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

### <a name="response"></a><span data-ttu-id="f95b6-198">応答</span><span class="sxs-lookup"><span data-stu-id="f95b6-198">Response</span></span>
<span data-ttu-id="f95b6-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f95b6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





