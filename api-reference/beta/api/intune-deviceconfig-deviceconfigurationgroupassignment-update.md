---
title: DeviceConfigurationGroupAssignment の更新
description: DeviceConfigurationGroupAssignment オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 49f9255ae8423895bcfce67a1107c4f3c98f90cb
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34967672"
---
# <a name="update-deviceconfigurationgroupassignment"></a><span data-ttu-id="7998c-103">DeviceConfigurationGroupAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="7998c-103">Update deviceConfigurationGroupAssignment</span></span>

> <span data-ttu-id="7998c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7998c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7998c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7998c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7998c-106">[DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7998c-106">Update the properties of a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7998c-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="7998c-107">Prerequisites</span></span>
<span data-ttu-id="7998c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7998c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7998c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7998c-110">Permission type</span></span>|<span data-ttu-id="7998c-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7998c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7998c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7998c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7998c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7998c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7998c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7998c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7998c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7998c-115">Not supported.</span></span>|
|<span data-ttu-id="7998c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7998c-116">Application</span></span>|<span data-ttu-id="7998c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7998c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7998c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7998c-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="7998c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7998c-119">Request headers</span></span>
|<span data-ttu-id="7998c-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7998c-120">Header</span></span>|<span data-ttu-id="7998c-121">値</span><span class="sxs-lookup"><span data-stu-id="7998c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7998c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7998c-122">Authorization</span></span>|<span data-ttu-id="7998c-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7998c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7998c-124">承諾</span><span class="sxs-lookup"><span data-stu-id="7998c-124">Accept</span></span>|<span data-ttu-id="7998c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7998c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7998c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7998c-126">Request body</span></span>
<span data-ttu-id="7998c-127">要求本文で、 [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7998c-127">In the request body, supply a JSON representation for the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

<span data-ttu-id="7998c-128">次の表に、 [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7998c-128">The following table shows the properties that are required when you create the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span></span>

|<span data-ttu-id="7998c-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7998c-129">Property</span></span>|<span data-ttu-id="7998c-130">型</span><span class="sxs-lookup"><span data-stu-id="7998c-130">Type</span></span>|<span data-ttu-id="7998c-131">説明</span><span class="sxs-lookup"><span data-stu-id="7998c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7998c-132">id</span><span class="sxs-lookup"><span data-stu-id="7998c-132">id</span></span>|<span data-ttu-id="7998c-133">String</span><span class="sxs-lookup"><span data-stu-id="7998c-133">String</span></span>|<span data-ttu-id="7998c-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7998c-134">Key of the entity.</span></span>|
|<span data-ttu-id="7998c-135">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="7998c-135">targetGroupId</span></span>|<span data-ttu-id="7998c-136">String</span><span class="sxs-lookup"><span data-stu-id="7998c-136">String</span></span>|<span data-ttu-id="7998c-137">デバイス構成を対象としている AAD グループの Id。</span><span class="sxs-lookup"><span data-stu-id="7998c-137">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="7998c-138">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="7998c-138">excludeGroup</span></span>|<span data-ttu-id="7998c-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="7998c-139">Boolean</span></span>|<span data-ttu-id="7998c-140">このグループを除外する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7998c-140">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="7998c-141">グループが含まれる既定値</span><span class="sxs-lookup"><span data-stu-id="7998c-141">Defaults that the group should be included</span></span>|



## <a name="response"></a><span data-ttu-id="7998c-142">応答</span><span class="sxs-lookup"><span data-stu-id="7998c-142">Response</span></span>
<span data-ttu-id="7998c-143">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7998c-143">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7998c-144">例</span><span class="sxs-lookup"><span data-stu-id="7998c-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="7998c-145">要求</span><span class="sxs-lookup"><span data-stu-id="7998c-145">Request</span></span>
<span data-ttu-id="7998c-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7998c-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7998c-147">応答</span><span class="sxs-lookup"><span data-stu-id="7998c-147">Response</span></span>
<span data-ttu-id="7998c-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7998c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





