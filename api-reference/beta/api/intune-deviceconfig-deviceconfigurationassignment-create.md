---
title: deviceConfigurationAssignment の作成
description: 新しい deviceConfigurationAssignment オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c9e655e28ce61830122aad3194ace5ca83f20259
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156008"
---
# <a name="create-deviceconfigurationassignment"></a><span data-ttu-id="daaf8-103">deviceConfigurationAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="daaf8-103">Create deviceConfigurationAssignment</span></span>

> <span data-ttu-id="daaf8-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="daaf8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="daaf8-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="daaf8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="daaf8-106">新しい [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="daaf8-106">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="daaf8-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="daaf8-107">Prerequisites</span></span>
<span data-ttu-id="daaf8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="daaf8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="daaf8-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="daaf8-110">Permission type</span></span>|<span data-ttu-id="daaf8-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="daaf8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="daaf8-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="daaf8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="daaf8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="daaf8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="daaf8-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="daaf8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="daaf8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="daaf8-115">Not supported.</span></span>|
|<span data-ttu-id="daaf8-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="daaf8-116">Application</span></span>|<span data-ttu-id="daaf8-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="daaf8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="daaf8-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="daaf8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="daaf8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="daaf8-119">Request headers</span></span>
|<span data-ttu-id="daaf8-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="daaf8-120">Header</span></span>|<span data-ttu-id="daaf8-121">値</span><span class="sxs-lookup"><span data-stu-id="daaf8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="daaf8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="daaf8-122">Authorization</span></span>|<span data-ttu-id="daaf8-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="daaf8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="daaf8-124">承諾</span><span class="sxs-lookup"><span data-stu-id="daaf8-124">Accept</span></span>|<span data-ttu-id="daaf8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="daaf8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="daaf8-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="daaf8-126">Request body</span></span>
<span data-ttu-id="daaf8-127">要求本文で、deviceConfigurationAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="daaf8-127">In the request body, supply a JSON representation for the deviceConfigurationAssignment object.</span></span>

<span data-ttu-id="daaf8-128">次の表に、deviceConfigurationAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="daaf8-128">The following table shows the properties that are required when you create the deviceConfigurationAssignment.</span></span>

|<span data-ttu-id="daaf8-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="daaf8-129">Property</span></span>|<span data-ttu-id="daaf8-130">型</span><span class="sxs-lookup"><span data-stu-id="daaf8-130">Type</span></span>|<span data-ttu-id="daaf8-131">説明</span><span class="sxs-lookup"><span data-stu-id="daaf8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="daaf8-132">id</span><span class="sxs-lookup"><span data-stu-id="daaf8-132">id</span></span>|<span data-ttu-id="daaf8-133">String</span><span class="sxs-lookup"><span data-stu-id="daaf8-133">String</span></span>|<span data-ttu-id="daaf8-134">割り当てのキー。</span><span class="sxs-lookup"><span data-stu-id="daaf8-134">The key of the assignment.</span></span>|
|<span data-ttu-id="daaf8-135">target</span><span class="sxs-lookup"><span data-stu-id="daaf8-135">target</span></span>|[<span data-ttu-id="daaf8-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="daaf8-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="daaf8-137">デバイス構成の割り当て先。</span><span class="sxs-lookup"><span data-stu-id="daaf8-137">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="daaf8-138">応答</span><span class="sxs-lookup"><span data-stu-id="daaf8-138">Response</span></span>
<span data-ttu-id="daaf8-139">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="daaf8-139">If successful, this method returns a `201 Created` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="daaf8-140">例</span><span class="sxs-lookup"><span data-stu-id="daaf8-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="daaf8-141">要求</span><span class="sxs-lookup"><span data-stu-id="daaf8-141">Request</span></span>
<span data-ttu-id="daaf8-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="daaf8-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
Content-type: application/json
Content-length: 169

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="daaf8-143">応答</span><span class="sxs-lookup"><span data-stu-id="daaf8-143">Response</span></span>
<span data-ttu-id="daaf8-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="daaf8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 218

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```




