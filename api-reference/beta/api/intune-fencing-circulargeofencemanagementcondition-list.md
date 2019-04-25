---
title: リスト circularGeofenceManagementConditions
description: circularGeofenceManagementCondition オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7c3d0652a9bc4bad843313f21e837c1d5b2cdba4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32532402"
---
# <a name="list-circulargeofencemanagementconditions"></a><span data-ttu-id="03734-103">リスト circularGeofenceManagementConditions</span><span class="sxs-lookup"><span data-stu-id="03734-103">List circularGeofenceManagementConditions</span></span>

> <span data-ttu-id="03734-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="03734-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03734-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="03734-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03734-106">[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="03734-106">List properties and relationships of the [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03734-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="03734-107">Prerequisites</span></span>
<span data-ttu-id="03734-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="03734-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03734-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="03734-110">Permission type</span></span>|<span data-ttu-id="03734-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="03734-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03734-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="03734-112">Delegated (work or school account)</span></span>|<span data-ttu-id="03734-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="03734-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="03734-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="03734-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03734-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="03734-115">Not supported.</span></span>|
|<span data-ttu-id="03734-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="03734-116">Application</span></span>|<span data-ttu-id="03734-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="03734-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="03734-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="03734-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="03734-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="03734-119">Request headers</span></span>
|<span data-ttu-id="03734-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="03734-120">Header</span></span>|<span data-ttu-id="03734-121">値</span><span class="sxs-lookup"><span data-stu-id="03734-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03734-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="03734-122">Authorization</span></span>|<span data-ttu-id="03734-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="03734-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03734-124">承諾</span><span class="sxs-lookup"><span data-stu-id="03734-124">Accept</span></span>|<span data-ttu-id="03734-125">application/json</span><span class="sxs-lookup"><span data-stu-id="03734-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03734-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="03734-126">Request body</span></span>
<span data-ttu-id="03734-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="03734-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="03734-128">応答</span><span class="sxs-lookup"><span data-stu-id="03734-128">Response</span></span>
<span data-ttu-id="03734-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="03734-129">If successful, this method returns a `200 OK` response code and a collection of [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03734-130">例</span><span class="sxs-lookup"><span data-stu-id="03734-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="03734-131">要求</span><span class="sxs-lookup"><span data-stu-id="03734-131">Request</span></span>
<span data-ttu-id="03734-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="03734-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions
```

### <a name="response"></a><span data-ttu-id="03734-133">応答</span><span class="sxs-lookup"><span data-stu-id="03734-133">Response</span></span>
<span data-ttu-id="03734-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="03734-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 701

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.circularGeofenceManagementCondition",
      "id": "30ee27b6-27b6-30ee-b627-ee30b627ee30",
      "uniqueName": "Unique Name value",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
      "eTag": "ETag value",
      "applicablePlatforms": [
        "androidForWork"
      ],
      "latitude": "<Unknown Primitive Type Edm.Double>",
      "longitude": "<Unknown Primitive Type Edm.Double>",
      "radiusInMeters": "<Unknown Primitive Type Edm.Single>"
    }
  ]
}
```





