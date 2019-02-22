---
title: deviceConfigurationGroupAssignment の更新
description: deviceConfigurationGroupAssignment オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 04371d8797ff25c5bb403c67d5aa4bc4024cee89
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162770"
---
# <a name="update-deviceconfigurationgroupassignment"></a><span data-ttu-id="d8d33-103">deviceConfigurationGroupAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="d8d33-103">Update deviceConfigurationGroupAssignment</span></span>

> <span data-ttu-id="d8d33-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d8d33-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8d33-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d8d33-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8d33-106">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d8d33-106">Update the properties of a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8d33-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d8d33-107">Prerequisites</span></span>
<span data-ttu-id="d8d33-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d8d33-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d8d33-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d8d33-110">Permission type</span></span>|<span data-ttu-id="d8d33-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d8d33-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8d33-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d8d33-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d8d33-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8d33-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d8d33-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d8d33-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8d33-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d8d33-115">Not supported.</span></span>|
|<span data-ttu-id="d8d33-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d8d33-116">Application</span></span>|<span data-ttu-id="d8d33-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d8d33-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8d33-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d8d33-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="d8d33-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d8d33-119">Request headers</span></span>
|<span data-ttu-id="d8d33-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d8d33-120">Header</span></span>|<span data-ttu-id="d8d33-121">値</span><span class="sxs-lookup"><span data-stu-id="d8d33-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8d33-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8d33-122">Authorization</span></span>|<span data-ttu-id="d8d33-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d8d33-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8d33-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d8d33-124">Accept</span></span>|<span data-ttu-id="d8d33-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d8d33-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8d33-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d8d33-126">Request body</span></span>
<span data-ttu-id="d8d33-127">要求本文で、 [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d8d33-127">In the request body, supply a JSON representation for the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

<span data-ttu-id="d8d33-128">次の表に、 [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d8d33-128">The following table shows the properties that are required when you create the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span></span>

|<span data-ttu-id="d8d33-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d8d33-129">Property</span></span>|<span data-ttu-id="d8d33-130">型</span><span class="sxs-lookup"><span data-stu-id="d8d33-130">Type</span></span>|<span data-ttu-id="d8d33-131">説明</span><span class="sxs-lookup"><span data-stu-id="d8d33-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8d33-132">id</span><span class="sxs-lookup"><span data-stu-id="d8d33-132">id</span></span>|<span data-ttu-id="d8d33-133">String</span><span class="sxs-lookup"><span data-stu-id="d8d33-133">String</span></span>|<span data-ttu-id="d8d33-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d8d33-134">Key of the entity.</span></span>|
|<span data-ttu-id="d8d33-135">targetgroupid</span><span class="sxs-lookup"><span data-stu-id="d8d33-135">targetGroupId</span></span>|<span data-ttu-id="d8d33-136">String</span><span class="sxs-lookup"><span data-stu-id="d8d33-136">String</span></span>|<span data-ttu-id="d8d33-137">デバイス構成を対象としている AAD グループの Id。</span><span class="sxs-lookup"><span data-stu-id="d8d33-137">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="d8d33-138">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="d8d33-138">excludeGroup</span></span>|<span data-ttu-id="d8d33-139">ブール値</span><span class="sxs-lookup"><span data-stu-id="d8d33-139">Boolean</span></span>|<span data-ttu-id="d8d33-140">このグループを除外する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d8d33-140">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="d8d33-141">グループが含まれる既定値</span><span class="sxs-lookup"><span data-stu-id="d8d33-141">Defaults that the group should be included</span></span>|



## <a name="response"></a><span data-ttu-id="d8d33-142">応答</span><span class="sxs-lookup"><span data-stu-id="d8d33-142">Response</span></span>
<span data-ttu-id="d8d33-143">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d8d33-143">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8d33-144">例</span><span class="sxs-lookup"><span data-stu-id="d8d33-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8d33-145">要求</span><span class="sxs-lookup"><span data-stu-id="d8d33-145">Request</span></span>
<span data-ttu-id="d8d33-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d8d33-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
Content-type: application/json
Content-length: 146

{
  "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
  "targetGroupId": "Target Group Id value",
  "excludeGroup": true
}
```

### <a name="response"></a><span data-ttu-id="d8d33-147">応答</span><span class="sxs-lookup"><span data-stu-id="d8d33-147">Response</span></span>
<span data-ttu-id="d8d33-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d8d33-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 195

{
  "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
  "id": "561d26c5-26c5-561d-c526-1d56c5261d56",
  "targetGroupId": "Target Group Id value",
  "excludeGroup": true
}
```




