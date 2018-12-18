---
title: DeviceConfigurationGroupAssignment を更新します。
description: DeviceConfigurationGroupAssignment オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 7ea879c7d267337a247455235f069206b7b3b2a0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313882"
---
# <a name="update-deviceconfigurationgroupassignment"></a><span data-ttu-id="8d2ae-103">DeviceConfigurationGroupAssignment を更新します。</span><span class="sxs-lookup"><span data-stu-id="8d2ae-103">Update deviceConfigurationGroupAssignment</span></span>

> <span data-ttu-id="8d2ae-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8d2ae-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d2ae-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d2ae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8d2ae-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8d2ae-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8d2ae-107">[DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8d2ae-107">Update the properties of a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8d2ae-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="8d2ae-108">Prerequisites</span></span>
<span data-ttu-id="8d2ae-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8d2ae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d2ae-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8d2ae-111">Permission type</span></span>|<span data-ttu-id="8d2ae-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8d2ae-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d2ae-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8d2ae-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8d2ae-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d2ae-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8d2ae-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8d2ae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d2ae-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d2ae-116">Not supported.</span></span>|
|<span data-ttu-id="8d2ae-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8d2ae-117">Application</span></span>|<span data-ttu-id="8d2ae-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d2ae-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d2ae-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8d2ae-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="8d2ae-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8d2ae-120">Request headers</span></span>
|<span data-ttu-id="8d2ae-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8d2ae-121">Header</span></span>|<span data-ttu-id="8d2ae-122">値</span><span class="sxs-lookup"><span data-stu-id="8d2ae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d2ae-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d2ae-123">Authorization</span></span>|<span data-ttu-id="8d2ae-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="8d2ae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d2ae-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8d2ae-125">Accept</span></span>|<span data-ttu-id="8d2ae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8d2ae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d2ae-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="8d2ae-127">Request body</span></span>
<span data-ttu-id="8d2ae-128">要求の本文に[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="8d2ae-128">In the request body, supply a JSON representation for the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

<span data-ttu-id="8d2ae-129">[DeviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="8d2ae-129">The following table shows the properties that are required when you create the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span></span>

|<span data-ttu-id="8d2ae-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8d2ae-130">Property</span></span>|<span data-ttu-id="8d2ae-131">種類</span><span class="sxs-lookup"><span data-stu-id="8d2ae-131">Type</span></span>|<span data-ttu-id="8d2ae-132">説明</span><span class="sxs-lookup"><span data-stu-id="8d2ae-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d2ae-133">ID</span><span class="sxs-lookup"><span data-stu-id="8d2ae-133">id</span></span>|<span data-ttu-id="8d2ae-134">String</span><span class="sxs-lookup"><span data-stu-id="8d2ae-134">String</span></span>|<span data-ttu-id="8d2ae-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8d2ae-135">Key of the entity.</span></span>|
|<span data-ttu-id="8d2ae-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="8d2ae-136">targetGroupId</span></span>|<span data-ttu-id="8d2ae-137">String</span><span class="sxs-lookup"><span data-stu-id="8d2ae-137">String</span></span>|<span data-ttu-id="8d2ae-138">AAD グループの Id は、対象としてデバイスを構成します。</span><span class="sxs-lookup"><span data-stu-id="8d2ae-138">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="8d2ae-139">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="8d2ae-139">excludeGroup</span></span>|<span data-ttu-id="8d2ae-140">ブール型</span><span class="sxs-lookup"><span data-stu-id="8d2ae-140">Boolean</span></span>|<span data-ttu-id="8d2ae-141">かどうかをこのグループを除外するようにします。</span><span class="sxs-lookup"><span data-stu-id="8d2ae-141">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="8d2ae-142">既定のグループが含まれている必要があること</span><span class="sxs-lookup"><span data-stu-id="8d2ae-142">Defaults that the group should be included</span></span>|



## <a name="response"></a><span data-ttu-id="8d2ae-143">応答</span><span class="sxs-lookup"><span data-stu-id="8d2ae-143">Response</span></span>
<span data-ttu-id="8d2ae-144">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="8d2ae-144">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d2ae-145">例</span><span class="sxs-lookup"><span data-stu-id="8d2ae-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="8d2ae-146">要求</span><span class="sxs-lookup"><span data-stu-id="8d2ae-146">Request</span></span>
<span data-ttu-id="8d2ae-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8d2ae-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
Content-type: application/json
Content-length: 73

{
  "targetGroupId": "Target Group Id value",
  "excludeGroup": true
}
```

### <a name="response"></a><span data-ttu-id="8d2ae-148">応答</span><span class="sxs-lookup"><span data-stu-id="8d2ae-148">Response</span></span>
<span data-ttu-id="8d2ae-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8d2ae-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





