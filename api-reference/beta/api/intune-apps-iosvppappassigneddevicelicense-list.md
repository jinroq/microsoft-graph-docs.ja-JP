---
title: リスト iosVppAppAssignedDeviceLicenses
description: iosVppAppAssignedDeviceLicense オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 61ae06fdfb35b804f33b9d5bb6143ab785924bc4
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30975288"
---
# <a name="list-iosvppappassigneddevicelicenses"></a><span data-ttu-id="270cd-103">リスト iosVppAppAssignedDeviceLicenses</span><span class="sxs-lookup"><span data-stu-id="270cd-103">List iosVppAppAssignedDeviceLicenses</span></span>

> <span data-ttu-id="270cd-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="270cd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="270cd-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="270cd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="270cd-106">[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="270cd-106">List properties and relationships of the [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="270cd-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="270cd-107">Prerequisites</span></span>
<span data-ttu-id="270cd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="270cd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="270cd-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="270cd-110">Permission type</span></span>|<span data-ttu-id="270cd-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="270cd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="270cd-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="270cd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="270cd-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="270cd-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="270cd-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="270cd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="270cd-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="270cd-115">Not supported.</span></span>|
|<span data-ttu-id="270cd-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="270cd-116">Application</span></span>|<span data-ttu-id="270cd-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="270cd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="270cd-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="270cd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="270cd-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="270cd-119">Request headers</span></span>
|<span data-ttu-id="270cd-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="270cd-120">Header</span></span>|<span data-ttu-id="270cd-121">値</span><span class="sxs-lookup"><span data-stu-id="270cd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="270cd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="270cd-122">Authorization</span></span>|<span data-ttu-id="270cd-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="270cd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="270cd-124">承諾</span><span class="sxs-lookup"><span data-stu-id="270cd-124">Accept</span></span>|<span data-ttu-id="270cd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="270cd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="270cd-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="270cd-126">Request body</span></span>
<span data-ttu-id="270cd-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="270cd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="270cd-128">応答</span><span class="sxs-lookup"><span data-stu-id="270cd-128">Response</span></span>
<span data-ttu-id="270cd-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="270cd-129">If successful, this method returns a `200 OK` response code and a collection of [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="270cd-130">例</span><span class="sxs-lookup"><span data-stu-id="270cd-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="270cd-131">要求</span><span class="sxs-lookup"><span data-stu-id="270cd-131">Request</span></span>
<span data-ttu-id="270cd-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="270cd-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

### <a name="response"></a><span data-ttu-id="270cd-133">応答</span><span class="sxs-lookup"><span data-stu-id="270cd-133">Response</span></span>
<span data-ttu-id="270cd-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="270cd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 441

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosVppAppAssignedDeviceLicense",
      "id": "bed943d0-43d0-bed9-d043-d9bed043d9be",
      "userEmailAddress": "User Email Address value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value",
      "managedDeviceId": "Managed Device Id value",
      "deviceName": "Device Name value"
    }
  ]
}
```




