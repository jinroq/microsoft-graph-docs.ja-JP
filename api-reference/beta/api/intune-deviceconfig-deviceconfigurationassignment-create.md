---
title: deviceConfigurationAssignment の作成
description: 新しい deviceConfigurationAssignment オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 035828ad5266c745e33cbd57f097d925e6ea4c5c
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31792560"
---
# <a name="create-deviceconfigurationassignment"></a><span data-ttu-id="8e9d3-103">deviceConfigurationAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="8e9d3-103">Create deviceConfigurationAssignment</span></span>

> <span data-ttu-id="8e9d3-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8e9d3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e9d3-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8e9d3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e9d3-106">新しい [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="8e9d3-106">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8e9d3-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="8e9d3-107">Prerequisites</span></span>
<span data-ttu-id="8e9d3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8e9d3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e9d3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8e9d3-110">Permission type</span></span>|<span data-ttu-id="8e9d3-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8e9d3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e9d3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8e9d3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8e9d3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e9d3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8e9d3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8e9d3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e9d3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8e9d3-115">Not supported.</span></span>|
|<span data-ttu-id="8e9d3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8e9d3-116">Application</span></span>|<span data-ttu-id="8e9d3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8e9d3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e9d3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8e9d3-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="8e9d3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8e9d3-119">Request headers</span></span>
|<span data-ttu-id="8e9d3-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8e9d3-120">Header</span></span>|<span data-ttu-id="8e9d3-121">値</span><span class="sxs-lookup"><span data-stu-id="8e9d3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e9d3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e9d3-122">Authorization</span></span>|<span data-ttu-id="8e9d3-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8e9d3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e9d3-124">承諾</span><span class="sxs-lookup"><span data-stu-id="8e9d3-124">Accept</span></span>|<span data-ttu-id="8e9d3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8e9d3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e9d3-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8e9d3-126">Request body</span></span>
<span data-ttu-id="8e9d3-127">要求本文で、deviceConfigurationAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8e9d3-127">In the request body, supply a JSON representation for the deviceConfigurationAssignment object.</span></span>

<span data-ttu-id="8e9d3-128">次の表に、deviceConfigurationAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8e9d3-128">The following table shows the properties that are required when you create the deviceConfigurationAssignment.</span></span>

|<span data-ttu-id="8e9d3-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8e9d3-129">Property</span></span>|<span data-ttu-id="8e9d3-130">型</span><span class="sxs-lookup"><span data-stu-id="8e9d3-130">Type</span></span>|<span data-ttu-id="8e9d3-131">説明</span><span class="sxs-lookup"><span data-stu-id="8e9d3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e9d3-132">id</span><span class="sxs-lookup"><span data-stu-id="8e9d3-132">id</span></span>|<span data-ttu-id="8e9d3-133">String</span><span class="sxs-lookup"><span data-stu-id="8e9d3-133">String</span></span>|<span data-ttu-id="8e9d3-134">割り当てのキー。</span><span class="sxs-lookup"><span data-stu-id="8e9d3-134">The key of the assignment.</span></span>|
|<span data-ttu-id="8e9d3-135">target</span><span class="sxs-lookup"><span data-stu-id="8e9d3-135">target</span></span>|[<span data-ttu-id="8e9d3-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="8e9d3-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="8e9d3-137">デバイス構成の割り当て先。</span><span class="sxs-lookup"><span data-stu-id="8e9d3-137">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="8e9d3-138">応答</span><span class="sxs-lookup"><span data-stu-id="8e9d3-138">Response</span></span>
<span data-ttu-id="8e9d3-139">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8e9d3-139">If successful, this method returns a `201 Created` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e9d3-140">例</span><span class="sxs-lookup"><span data-stu-id="8e9d3-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="8e9d3-141">要求</span><span class="sxs-lookup"><span data-stu-id="8e9d3-141">Request</span></span>
<span data-ttu-id="8e9d3-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8e9d3-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8e9d3-143">応答</span><span class="sxs-lookup"><span data-stu-id="8e9d3-143">Response</span></span>
<span data-ttu-id="8e9d3-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8e9d3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





