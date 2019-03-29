---
title: managedDeviceMobileAppConfigurationAssignments のリスト
description: managedDeviceMobileAppConfigurationAssignment オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7cc477f0193f80bb6df1fdc6f42eabe8e7fce220
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30957228"
---
# <a name="list-manageddevicemobileappconfigurationassignments"></a><span data-ttu-id="665cc-103">managedDeviceMobileAppConfigurationAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="665cc-103">List managedDeviceMobileAppConfigurationAssignments</span></span>

> <span data-ttu-id="665cc-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="665cc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="665cc-105">[managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="665cc-105">List properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="665cc-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="665cc-106">Prerequisites</span></span>
<span data-ttu-id="665cc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="665cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="665cc-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="665cc-109">Permission type</span></span>|<span data-ttu-id="665cc-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="665cc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="665cc-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="665cc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="665cc-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="665cc-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="665cc-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="665cc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="665cc-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="665cc-114">Not supported.</span></span>|
|<span data-ttu-id="665cc-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="665cc-115">Application</span></span>|<span data-ttu-id="665cc-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="665cc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="665cc-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="665cc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="665cc-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="665cc-118">Request headers</span></span>
|<span data-ttu-id="665cc-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="665cc-119">Header</span></span>|<span data-ttu-id="665cc-120">値</span><span class="sxs-lookup"><span data-stu-id="665cc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="665cc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="665cc-121">Authorization</span></span>|<span data-ttu-id="665cc-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="665cc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="665cc-123">承諾</span><span class="sxs-lookup"><span data-stu-id="665cc-123">Accept</span></span>|<span data-ttu-id="665cc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="665cc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="665cc-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="665cc-125">Request body</span></span>
<span data-ttu-id="665cc-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="665cc-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="665cc-127">応答</span><span class="sxs-lookup"><span data-stu-id="665cc-127">Response</span></span>
<span data-ttu-id="665cc-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="665cc-128">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="665cc-129">例</span><span class="sxs-lookup"><span data-stu-id="665cc-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="665cc-130">要求</span><span class="sxs-lookup"><span data-stu-id="665cc-130">Request</span></span>
<span data-ttu-id="665cc-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="665cc-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="665cc-132">応答</span><span class="sxs-lookup"><span data-stu-id="665cc-132">Response</span></span>
<span data-ttu-id="665cc-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="665cc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 287

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
      "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```



