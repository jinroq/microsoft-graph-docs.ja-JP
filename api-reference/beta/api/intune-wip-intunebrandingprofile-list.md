---
title: リスト intuneBrandingProfiles
description: IntuneBrandingProfile オブジェクトのプロパティと関係を一覧表示します。
ms.openlocfilehash: 0c7fa1a191de73ea5042e319489633388b1f95df
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072478"
---
# <a name="list-intunebrandingprofiles"></a><span data-ttu-id="d48f3-103">リスト intuneBrandingProfiles</span><span class="sxs-lookup"><span data-stu-id="d48f3-103">List intuneBrandingProfiles</span></span>

> <span data-ttu-id="d48f3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d48f3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d48f3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d48f3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d48f3-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d48f3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d48f3-107">[IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="d48f3-107">List properties and relationships of the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d48f3-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="d48f3-108">Prerequisites</span></span>
<span data-ttu-id="d48f3-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d48f3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d48f3-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d48f3-111">Permission type</span></span>|<span data-ttu-id="d48f3-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d48f3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d48f3-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d48f3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d48f3-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d48f3-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d48f3-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d48f3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d48f3-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d48f3-116">Not supported.</span></span>|
|<span data-ttu-id="d48f3-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d48f3-117">Application</span></span>|<span data-ttu-id="d48f3-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d48f3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d48f3-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d48f3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intuneBrandingProfiles
```

## <a name="request-headers"></a><span data-ttu-id="d48f3-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d48f3-120">Request headers</span></span>
|<span data-ttu-id="d48f3-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d48f3-121">Header</span></span>|<span data-ttu-id="d48f3-122">値</span><span class="sxs-lookup"><span data-stu-id="d48f3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d48f3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d48f3-123">Authorization</span></span>|<span data-ttu-id="d48f3-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d48f3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d48f3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d48f3-125">Accept</span></span>|<span data-ttu-id="d48f3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d48f3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d48f3-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d48f3-127">Request body</span></span>
<span data-ttu-id="d48f3-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d48f3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d48f3-129">応答</span><span class="sxs-lookup"><span data-stu-id="d48f3-129">Response</span></span>
<span data-ttu-id="d48f3-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="d48f3-130">If successful, this method returns a `200 OK` response code and a collection of [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d48f3-131">例</span><span class="sxs-lookup"><span data-stu-id="d48f3-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="d48f3-132">要求</span><span class="sxs-lookup"><span data-stu-id="d48f3-132">Request</span></span>
<span data-ttu-id="d48f3-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d48f3-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles
```

### <a name="response"></a><span data-ttu-id="d48f3-134">応答</span><span class="sxs-lookup"><span data-stu-id="d48f3-134">Response</span></span>
<span data-ttu-id="d48f3-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d48f3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1562

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
      }
    }
  ]
}
```





