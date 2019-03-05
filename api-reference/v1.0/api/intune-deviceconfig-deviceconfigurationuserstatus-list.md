---
title: deviceConfigurationUserStatuses のリスト
description: deviceConfigurationUserStatus オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cc3f0c3c453a225bfc839af25218403803889910
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255480"
---
# <a name="list-deviceconfigurationuserstatuses"></a><span data-ttu-id="a4fcd-103">deviceConfigurationUserStatuses のリスト</span><span class="sxs-lookup"><span data-stu-id="a4fcd-103">List deviceConfigurationUserStatuses</span></span>

> <span data-ttu-id="a4fcd-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a4fcd-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a4fcd-105">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a4fcd-105">List properties and relationships of the [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a4fcd-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="a4fcd-106">Prerequisites</span></span>
<span data-ttu-id="a4fcd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a4fcd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a4fcd-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a4fcd-109">Permission type</span></span>|<span data-ttu-id="a4fcd-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a4fcd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a4fcd-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a4fcd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a4fcd-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a4fcd-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a4fcd-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a4fcd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a4fcd-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4fcd-114">Not supported.</span></span>|
|<span data-ttu-id="a4fcd-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a4fcd-115">Application</span></span>|<span data-ttu-id="a4fcd-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a4fcd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a4fcd-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a4fcd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="a4fcd-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a4fcd-118">Request headers</span></span>
|<span data-ttu-id="a4fcd-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a4fcd-119">Header</span></span>|<span data-ttu-id="a4fcd-120">値</span><span class="sxs-lookup"><span data-stu-id="a4fcd-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a4fcd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4fcd-121">Authorization</span></span>|<span data-ttu-id="a4fcd-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a4fcd-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a4fcd-123">承諾</span><span class="sxs-lookup"><span data-stu-id="a4fcd-123">Accept</span></span>|<span data-ttu-id="a4fcd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a4fcd-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a4fcd-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a4fcd-125">Request body</span></span>
<span data-ttu-id="a4fcd-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a4fcd-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a4fcd-127">応答</span><span class="sxs-lookup"><span data-stu-id="a4fcd-127">Response</span></span>
<span data-ttu-id="a4fcd-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="a4fcd-128">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4fcd-129">例</span><span class="sxs-lookup"><span data-stu-id="a4fcd-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="a4fcd-130">要求</span><span class="sxs-lookup"><span data-stu-id="a4fcd-130">Request</span></span>
<span data-ttu-id="a4fcd-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a4fcd-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="a4fcd-132">応答</span><span class="sxs-lookup"><span data-stu-id="a4fcd-132">Response</span></span>
<span data-ttu-id="a4fcd-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a4fcd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 400

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
      "id": "7e323db2-3db2-7e32-b23d-327eb23d327e",
      "userDisplayName": "User Display Name value",
      "devicesCount": 12,
      "status": "notApplicable",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```



