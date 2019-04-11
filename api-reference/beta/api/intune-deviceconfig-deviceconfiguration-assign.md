---
title: assign アクション
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: abf34960a3f992138094e55a1e6aa3282e7b3d69
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776732"
---
# <a name="assign-action"></a><span data-ttu-id="ee13b-103">アクションの割り当て</span><span class="sxs-lookup"><span data-stu-id="ee13b-103">assign action</span></span>

> <span data-ttu-id="ee13b-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee13b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee13b-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ee13b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee13b-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ee13b-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ee13b-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ee13b-107">Prerequisites</span></span>
<span data-ttu-id="ee13b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ee13b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ee13b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ee13b-110">Permission type</span></span>|<span data-ttu-id="ee13b-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ee13b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee13b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ee13b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ee13b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee13b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ee13b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ee13b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee13b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee13b-115">Not supported.</span></span>|
|<span data-ttu-id="ee13b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ee13b-116">Application</span></span>|<span data-ttu-id="ee13b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee13b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee13b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ee13b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/assign
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="ee13b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ee13b-119">Request headers</span></span>
|<span data-ttu-id="ee13b-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ee13b-120">Header</span></span>|<span data-ttu-id="ee13b-121">値</span><span class="sxs-lookup"><span data-stu-id="ee13b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee13b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee13b-122">Authorization</span></span>|<span data-ttu-id="ee13b-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ee13b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee13b-124">承諾</span><span class="sxs-lookup"><span data-stu-id="ee13b-124">Accept</span></span>|<span data-ttu-id="ee13b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ee13b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee13b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ee13b-126">Request body</span></span>
<span data-ttu-id="ee13b-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ee13b-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ee13b-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="ee13b-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ee13b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ee13b-129">Property</span></span>|<span data-ttu-id="ee13b-130">型</span><span class="sxs-lookup"><span data-stu-id="ee13b-130">Type</span></span>|<span data-ttu-id="ee13b-131">説明</span><span class="sxs-lookup"><span data-stu-id="ee13b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee13b-132">deviceConfigurationGroupAssignments</span><span class="sxs-lookup"><span data-stu-id="ee13b-132">deviceConfigurationGroupAssignments</span></span>|<span data-ttu-id="ee13b-133">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ee13b-133">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="ee13b-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ee13b-134">Not yet documented</span></span>|
|<span data-ttu-id="ee13b-135">assignments</span><span class="sxs-lookup"><span data-stu-id="ee13b-135">assignments</span></span>|<span data-ttu-id="ee13b-136">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ee13b-136">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="ee13b-137">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ee13b-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ee13b-138">応答</span><span class="sxs-lookup"><span data-stu-id="ee13b-138">Response</span></span>
<span data-ttu-id="ee13b-139">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="ee13b-139">If successful, this action returns a `200 OK` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee13b-140">例</span><span class="sxs-lookup"><span data-stu-id="ee13b-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="ee13b-141">要求</span><span class="sxs-lookup"><span data-stu-id="ee13b-141">Request</span></span>
<span data-ttu-id="ee13b-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ee13b-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assign

Content-type: application/json
Content-length: 548

{
  "deviceConfigurationGroupAssignments": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
      "id": "561d26c5-26c5-561d-c526-1d56c5261d56",
      "targetGroupId": "Target Group Id value",
      "excludeGroup": true
    }
  ],
  "assignments": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="ee13b-143">応答</span><span class="sxs-lookup"><span data-stu-id="ee13b-143">Response</span></span>
<span data-ttu-id="ee13b-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ee13b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 271

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





