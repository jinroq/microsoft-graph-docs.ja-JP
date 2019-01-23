---
title: managedDeviceMobileAppConfigurationUserStatuses のリスト
description: managedDeviceMobileAppConfigurationUserStatus オブジェクトのプロパティとリレーションシップをリストします。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 35d9d7b2959c4e39d74bd067b90b2ff95430f763
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397079"
---
# <a name="list-manageddevicemobileappconfigurationuserstatuses"></a><span data-ttu-id="a6141-103">managedDeviceMobileAppConfigurationUserStatuses のリスト</span><span class="sxs-lookup"><span data-stu-id="a6141-103">List managedDeviceMobileAppConfigurationUserStatuses</span></span>

> <span data-ttu-id="a6141-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a6141-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a6141-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6141-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a6141-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a6141-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6141-107">[managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a6141-107">List properties and relationships of the [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6141-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="a6141-108">Prerequisites</span></span>
<span data-ttu-id="a6141-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a6141-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a6141-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a6141-111">Permission type</span></span>|<span data-ttu-id="a6141-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a6141-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6141-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a6141-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a6141-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6141-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a6141-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a6141-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6141-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6141-116">Not supported.</span></span>|
|<span data-ttu-id="a6141-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a6141-117">Application</span></span>|<span data-ttu-id="a6141-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6141-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6141-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a6141-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
GET /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="a6141-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a6141-120">Request headers</span></span>
|<span data-ttu-id="a6141-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a6141-121">Header</span></span>|<span data-ttu-id="a6141-122">値</span><span class="sxs-lookup"><span data-stu-id="a6141-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6141-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6141-123">Authorization</span></span>|<span data-ttu-id="a6141-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a6141-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6141-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a6141-125">Accept</span></span>|<span data-ttu-id="a6141-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a6141-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6141-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a6141-127">Request body</span></span>
<span data-ttu-id="a6141-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a6141-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6141-129">応答</span><span class="sxs-lookup"><span data-stu-id="a6141-129">Response</span></span>
<span data-ttu-id="a6141-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="a6141-130">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6141-131">例</span><span class="sxs-lookup"><span data-stu-id="a6141-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6141-132">要求</span><span class="sxs-lookup"><span data-stu-id="a6141-132">Request</span></span>
<span data-ttu-id="a6141-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a6141-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="a6141-134">応答</span><span class="sxs-lookup"><span data-stu-id="a6141-134">Response</span></span>
<span data-ttu-id="a6141-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a6141-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 416

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationUserStatus",
      "id": "44960944-0944-4496-4409-964444099644",
      "userDisplayName": "User Display Name value",
      "devicesCount": 12,
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```




