---
title: deviceConfigurationAssignment の作成
description: 新しい deviceConfigurationAssignment オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f6dcac355c72e9326909091293af8759d0e8584c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400383"
---
# <a name="create-deviceconfigurationassignment"></a><span data-ttu-id="dcab2-103">deviceConfigurationAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="dcab2-103">Create deviceConfigurationAssignment</span></span>

> <span data-ttu-id="dcab2-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dcab2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="dcab2-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dcab2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dcab2-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dcab2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dcab2-107">新しい [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="dcab2-107">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dcab2-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="dcab2-108">Prerequisites</span></span>
<span data-ttu-id="dcab2-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dcab2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="dcab2-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dcab2-111">Permission type</span></span>|<span data-ttu-id="dcab2-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="dcab2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dcab2-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dcab2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dcab2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dcab2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dcab2-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dcab2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dcab2-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dcab2-116">Not supported.</span></span>|
|<span data-ttu-id="dcab2-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dcab2-117">Application</span></span>|<span data-ttu-id="dcab2-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dcab2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dcab2-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dcab2-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="dcab2-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dcab2-120">Request headers</span></span>
|<span data-ttu-id="dcab2-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dcab2-121">Header</span></span>|<span data-ttu-id="dcab2-122">値</span><span class="sxs-lookup"><span data-stu-id="dcab2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dcab2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dcab2-123">Authorization</span></span>|<span data-ttu-id="dcab2-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="dcab2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dcab2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="dcab2-125">Accept</span></span>|<span data-ttu-id="dcab2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dcab2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dcab2-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="dcab2-127">Request body</span></span>
<span data-ttu-id="dcab2-128">要求本文で、deviceConfigurationAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="dcab2-128">In the request body, supply a JSON representation for the deviceConfigurationAssignment object.</span></span>

<span data-ttu-id="dcab2-129">次の表に、deviceConfigurationAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="dcab2-129">The following table shows the properties that are required when you create the deviceConfigurationAssignment.</span></span>

|<span data-ttu-id="dcab2-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dcab2-130">Property</span></span>|<span data-ttu-id="dcab2-131">型</span><span class="sxs-lookup"><span data-stu-id="dcab2-131">Type</span></span>|<span data-ttu-id="dcab2-132">説明</span><span class="sxs-lookup"><span data-stu-id="dcab2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dcab2-133">id</span><span class="sxs-lookup"><span data-stu-id="dcab2-133">id</span></span>|<span data-ttu-id="dcab2-134">String</span><span class="sxs-lookup"><span data-stu-id="dcab2-134">String</span></span>|<span data-ttu-id="dcab2-135">割り当てのキー。</span><span class="sxs-lookup"><span data-stu-id="dcab2-135">The key of the assignment.</span></span>|
|<span data-ttu-id="dcab2-136">target</span><span class="sxs-lookup"><span data-stu-id="dcab2-136">target</span></span>|[<span data-ttu-id="dcab2-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="dcab2-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="dcab2-138">デバイス構成の割り当て先。</span><span class="sxs-lookup"><span data-stu-id="dcab2-138">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="dcab2-139">応答</span><span class="sxs-lookup"><span data-stu-id="dcab2-139">Response</span></span>
<span data-ttu-id="dcab2-140">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="dcab2-140">If successful, this method returns a `201 Created` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dcab2-141">例</span><span class="sxs-lookup"><span data-stu-id="dcab2-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="dcab2-142">要求</span><span class="sxs-lookup"><span data-stu-id="dcab2-142">Request</span></span>
<span data-ttu-id="dcab2-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dcab2-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="dcab2-144">応答</span><span class="sxs-lookup"><span data-stu-id="dcab2-144">Response</span></span>
<span data-ttu-id="dcab2-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dcab2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




