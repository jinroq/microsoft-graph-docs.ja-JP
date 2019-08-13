---
title: リスト intuneBrandingProfiles
description: IntuneBrandingProfile オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dab09c4f126b09bce7ab1e882f87bd9a1ecbcd83
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347256"
---
# <a name="list-intunebrandingprofiles"></a><span data-ttu-id="54aed-103">リスト intuneBrandingProfiles</span><span class="sxs-lookup"><span data-stu-id="54aed-103">List intuneBrandingProfiles</span></span>

> <span data-ttu-id="54aed-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="54aed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="54aed-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="54aed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54aed-106">[IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="54aed-106">List properties and relationships of the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54aed-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="54aed-107">Prerequisites</span></span>
<span data-ttu-id="54aed-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="54aed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54aed-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="54aed-110">Permission type</span></span>|<span data-ttu-id="54aed-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="54aed-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54aed-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="54aed-112">Delegated (work or school account)</span></span>|<span data-ttu-id="54aed-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="54aed-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="54aed-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="54aed-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54aed-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="54aed-115">Not supported.</span></span>|
|<span data-ttu-id="54aed-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="54aed-116">Application</span></span>|<span data-ttu-id="54aed-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="54aed-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="54aed-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="54aed-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a><span data-ttu-id="54aed-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="54aed-119">Request headers</span></span>
|<span data-ttu-id="54aed-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="54aed-120">Header</span></span>|<span data-ttu-id="54aed-121">値</span><span class="sxs-lookup"><span data-stu-id="54aed-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54aed-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="54aed-122">Authorization</span></span>|<span data-ttu-id="54aed-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="54aed-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54aed-124">承諾</span><span class="sxs-lookup"><span data-stu-id="54aed-124">Accept</span></span>|<span data-ttu-id="54aed-125">application/json</span><span class="sxs-lookup"><span data-stu-id="54aed-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54aed-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="54aed-126">Request body</span></span>
<span data-ttu-id="54aed-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="54aed-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54aed-128">応答</span><span class="sxs-lookup"><span data-stu-id="54aed-128">Response</span></span>
<span data-ttu-id="54aed-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="54aed-129">If successful, this method returns a `200 OK` response code and a collection of [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54aed-130">例</span><span class="sxs-lookup"><span data-stu-id="54aed-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="54aed-131">要求</span><span class="sxs-lookup"><span data-stu-id="54aed-131">Request</span></span>
<span data-ttu-id="54aed-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="54aed-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
```

### <a name="response"></a><span data-ttu-id="54aed-133">応答</span><span class="sxs-lookup"><span data-stu-id="54aed-133">Response</span></span>
<span data-ttu-id="54aed-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="54aed-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1703

{
  "value": [
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
      },
      "customPrivacyMessage": "Custom Privacy Message value",
      "isRemoveDeviceDisabled": true,
      "isFactoryResetDisabled": true
    }
  ]
}
```






