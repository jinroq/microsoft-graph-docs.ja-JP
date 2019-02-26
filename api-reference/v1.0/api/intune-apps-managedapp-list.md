---
title: managedApps のリスト
description: managedApp オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1ff2631cfed6b94bdcca8f68ba8cee07af56064a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263855"
---
# <a name="list-managedapps"></a><span data-ttu-id="1a7c1-103">managedApps のリスト</span><span class="sxs-lookup"><span data-stu-id="1a7c1-103">List managedApps</span></span>

> <span data-ttu-id="1a7c1-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1a7c1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a7c1-105">[managedApp](../resources/intune-apps-managedapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="1a7c1-105">List properties and relationships of the [managedApp](../resources/intune-apps-managedapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a7c1-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="1a7c1-106">Prerequisites</span></span>
<span data-ttu-id="1a7c1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1a7c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1a7c1-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1a7c1-109">Permission type</span></span>|<span data-ttu-id="1a7c1-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1a7c1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a7c1-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1a7c1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1a7c1-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a7c1-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1a7c1-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1a7c1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a7c1-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a7c1-114">Not supported.</span></span>|
|<span data-ttu-id="1a7c1-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1a7c1-115">Application</span></span>|<span data-ttu-id="1a7c1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a7c1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a7c1-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1a7c1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="1a7c1-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1a7c1-118">Request headers</span></span>
|<span data-ttu-id="1a7c1-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1a7c1-119">Header</span></span>|<span data-ttu-id="1a7c1-120">値</span><span class="sxs-lookup"><span data-stu-id="1a7c1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a7c1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a7c1-121">Authorization</span></span>|<span data-ttu-id="1a7c1-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="1a7c1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a7c1-123">承諾</span><span class="sxs-lookup"><span data-stu-id="1a7c1-123">Accept</span></span>|<span data-ttu-id="1a7c1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1a7c1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a7c1-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="1a7c1-125">Request body</span></span>
<span data-ttu-id="1a7c1-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1a7c1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a7c1-127">応答</span><span class="sxs-lookup"><span data-stu-id="1a7c1-127">Response</span></span>
<span data-ttu-id="1a7c1-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [managedApp](../resources/intune-apps-managedapp.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="1a7c1-128">If successful, this method returns a `200 OK` response code and a collection of [managedApp](../resources/intune-apps-managedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a7c1-129">例</span><span class="sxs-lookup"><span data-stu-id="1a7c1-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a7c1-130">要求</span><span class="sxs-lookup"><span data-stu-id="1a7c1-130">Request</span></span>
<span data-ttu-id="1a7c1-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1a7c1-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="1a7c1-132">応答</span><span class="sxs-lookup"><span data-stu-id="1a7c1-132">Response</span></span>
<span data-ttu-id="1a7c1-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1a7c1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 935

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedApp",
      "id": "f687dd85-dd85-f687-85dd-87f685dd87f6",
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
      "publishingState": "processing",
      "appAvailability": "lineOfBusiness",
      "version": "Version value"
    }
  ]
}
```



