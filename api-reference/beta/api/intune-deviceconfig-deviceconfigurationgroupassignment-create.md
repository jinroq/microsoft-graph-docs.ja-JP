---
title: DeviceConfigurationGroupAssignment を作成します。
description: 新しい deviceConfigurationGroupAssignment オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: c07356d3cf63699fda95e2be6fe361841e0b0d95
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355105"
---
# <a name="create-deviceconfigurationgroupassignment"></a><span data-ttu-id="cf8db-103">DeviceConfigurationGroupAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="cf8db-103">Create deviceConfigurationGroupAssignment</span></span>

> <span data-ttu-id="cf8db-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cf8db-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cf8db-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf8db-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cf8db-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cf8db-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cf8db-107">新しい[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="cf8db-107">Create a new [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cf8db-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="cf8db-108">Prerequisites</span></span>
<span data-ttu-id="cf8db-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cf8db-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf8db-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cf8db-111">Permission type</span></span>|<span data-ttu-id="cf8db-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cf8db-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf8db-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cf8db-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cf8db-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf8db-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cf8db-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cf8db-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf8db-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf8db-116">Not supported.</span></span>|
|<span data-ttu-id="cf8db-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cf8db-117">Application</span></span>|<span data-ttu-id="cf8db-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf8db-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf8db-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cf8db-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="cf8db-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cf8db-120">Request headers</span></span>
|<span data-ttu-id="cf8db-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cf8db-121">Header</span></span>|<span data-ttu-id="cf8db-122">値</span><span class="sxs-lookup"><span data-stu-id="cf8db-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf8db-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf8db-123">Authorization</span></span>|<span data-ttu-id="cf8db-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="cf8db-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf8db-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cf8db-125">Accept</span></span>|<span data-ttu-id="cf8db-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cf8db-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf8db-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="cf8db-127">Request body</span></span>
<span data-ttu-id="cf8db-128">要求の本文に deviceConfigurationGroupAssignment オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="cf8db-128">In the request body, supply a JSON representation for the deviceConfigurationGroupAssignment object.</span></span>

<span data-ttu-id="cf8db-129">次の表は、deviceConfigurationGroupAssignment を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="cf8db-129">The following table shows the properties that are required when you create the deviceConfigurationGroupAssignment.</span></span>

|<span data-ttu-id="cf8db-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cf8db-130">Property</span></span>|<span data-ttu-id="cf8db-131">種類</span><span class="sxs-lookup"><span data-stu-id="cf8db-131">Type</span></span>|<span data-ttu-id="cf8db-132">説明</span><span class="sxs-lookup"><span data-stu-id="cf8db-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf8db-133">ID</span><span class="sxs-lookup"><span data-stu-id="cf8db-133">id</span></span>|<span data-ttu-id="cf8db-134">String</span><span class="sxs-lookup"><span data-stu-id="cf8db-134">String</span></span>|<span data-ttu-id="cf8db-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="cf8db-135">Key of the entity.</span></span>|
|<span data-ttu-id="cf8db-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="cf8db-136">targetGroupId</span></span>|<span data-ttu-id="cf8db-137">String</span><span class="sxs-lookup"><span data-stu-id="cf8db-137">String</span></span>|<span data-ttu-id="cf8db-138">AAD グループの Id は、対象としてデバイスを構成します。</span><span class="sxs-lookup"><span data-stu-id="cf8db-138">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="cf8db-139">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="cf8db-139">excludeGroup</span></span>|<span data-ttu-id="cf8db-140">ブール型</span><span class="sxs-lookup"><span data-stu-id="cf8db-140">Boolean</span></span>|<span data-ttu-id="cf8db-141">かどうかをこのグループを除外するようにします。</span><span class="sxs-lookup"><span data-stu-id="cf8db-141">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="cf8db-142">既定のグループが含まれている必要があること</span><span class="sxs-lookup"><span data-stu-id="cf8db-142">Defaults that the group should be included</span></span>|



## <a name="response"></a><span data-ttu-id="cf8db-143">応答</span><span class="sxs-lookup"><span data-stu-id="cf8db-143">Response</span></span>
<span data-ttu-id="cf8db-144">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="cf8db-144">If successful, this method returns a `201 Created` response code and a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf8db-145">例</span><span class="sxs-lookup"><span data-stu-id="cf8db-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="cf8db-146">要求</span><span class="sxs-lookup"><span data-stu-id="cf8db-146">Request</span></span>
<span data-ttu-id="cf8db-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cf8db-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments
Content-type: application/json
Content-length: 146

{
  "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
  "targetGroupId": "Target Group Id value",
  "excludeGroup": true
}
```

### <a name="response"></a><span data-ttu-id="cf8db-148">応答</span><span class="sxs-lookup"><span data-stu-id="cf8db-148">Response</span></span>
<span data-ttu-id="cf8db-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cf8db-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 195

{
  "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
  "id": "561d26c5-26c5-561d-c526-1d56c5261d56",
  "targetGroupId": "Target Group Id value",
  "excludeGroup": true
}
```




