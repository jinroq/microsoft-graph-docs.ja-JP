---
title: IntuneBrandingProfile を取得します。
description: IntuneBrandingProfile オブジェクトのプロパティと関係を参照してください。
ms.openlocfilehash: 2c1c4d16cdd6166de0f7170bdef7a038a7ebd98b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073995"
---
# <a name="get-intunebrandingprofile"></a><span data-ttu-id="456a4-103">IntuneBrandingProfile を取得します。</span><span class="sxs-lookup"><span data-stu-id="456a4-103">Get intuneBrandingProfile</span></span>

> <span data-ttu-id="456a4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="456a4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="456a4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="456a4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="456a4-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="456a4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="456a4-107">[IntuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="456a4-107">Read properties and relationships of the [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="456a4-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="456a4-108">Prerequisites</span></span>
<span data-ttu-id="456a4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="456a4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="456a4-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="456a4-111">Permission type</span></span>|<span data-ttu-id="456a4-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="456a4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="456a4-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="456a4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="456a4-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="456a4-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="456a4-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="456a4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="456a4-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="456a4-116">Not supported.</span></span>|
|<span data-ttu-id="456a4-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="456a4-117">Application</span></span>|<span data-ttu-id="456a4-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="456a4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="456a4-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="456a4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="456a4-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="456a4-120">Optional query parameters</span></span>
<span data-ttu-id="456a4-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="456a4-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="456a4-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="456a4-122">Request headers</span></span>
|<span data-ttu-id="456a4-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="456a4-123">Header</span></span>|<span data-ttu-id="456a4-124">値</span><span class="sxs-lookup"><span data-stu-id="456a4-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="456a4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="456a4-125">Authorization</span></span>|<span data-ttu-id="456a4-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="456a4-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="456a4-127">Accept</span><span class="sxs-lookup"><span data-stu-id="456a4-127">Accept</span></span>|<span data-ttu-id="456a4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="456a4-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="456a4-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="456a4-129">Request body</span></span>
<span data-ttu-id="456a4-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="456a4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="456a4-131">応答</span><span class="sxs-lookup"><span data-stu-id="456a4-131">Response</span></span>
<span data-ttu-id="456a4-132">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="456a4-132">If successful, this method returns a `200 OK` response code and [intuneBrandingProfile](../resources/intune-wip-intunebrandingprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="456a4-133">例</span><span class="sxs-lookup"><span data-stu-id="456a4-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="456a4-134">要求</span><span class="sxs-lookup"><span data-stu-id="456a4-134">Request</span></span>
<span data-ttu-id="456a4-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="456a4-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}
```

### <a name="response"></a><span data-ttu-id="456a4-136">応答</span><span class="sxs-lookup"><span data-stu-id="456a4-136">Response</span></span>
<span data-ttu-id="456a4-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="456a4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1472

{
  "value": {
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
}
```





