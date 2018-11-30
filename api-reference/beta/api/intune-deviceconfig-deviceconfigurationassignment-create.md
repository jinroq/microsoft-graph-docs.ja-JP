---
title: deviceConfigurationAssignment の作成
description: 新しい deviceConfigurationAssignment オブジェクトを作成します。
ms.openlocfilehash: 366c4b68b6518999e696adf0363f93c7d29faec8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070970"
---
# <a name="create-deviceconfigurationassignment"></a><span data-ttu-id="c3bb6-103">deviceConfigurationAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="c3bb6-103">Create deviceConfigurationAssignment</span></span>

> <span data-ttu-id="c3bb6-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c3bb6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c3bb6-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3bb6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c3bb6-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c3bb6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c3bb6-107">新しい [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c3bb6-107">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c3bb6-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="c3bb6-108">Prerequisites</span></span>
<span data-ttu-id="c3bb6-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c3bb6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3bb6-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c3bb6-111">Permission type</span></span>|<span data-ttu-id="c3bb6-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c3bb6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3bb6-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c3bb6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c3bb6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3bb6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c3bb6-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c3bb6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3bb6-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3bb6-116">Not supported.</span></span>|
|<span data-ttu-id="c3bb6-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c3bb6-117">Application</span></span>|<span data-ttu-id="c3bb6-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c3bb6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3bb6-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c3bb6-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="c3bb6-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c3bb6-120">Request headers</span></span>
|<span data-ttu-id="c3bb6-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c3bb6-121">Header</span></span>|<span data-ttu-id="c3bb6-122">値</span><span class="sxs-lookup"><span data-stu-id="c3bb6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3bb6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3bb6-123">Authorization</span></span>|<span data-ttu-id="c3bb6-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c3bb6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3bb6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c3bb6-125">Accept</span></span>|<span data-ttu-id="c3bb6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c3bb6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3bb6-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c3bb6-127">Request body</span></span>
<span data-ttu-id="c3bb6-128">要求本文で、deviceConfigurationAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c3bb6-128">In the request body, supply a JSON representation for the deviceConfigurationAssignment object.</span></span>

<span data-ttu-id="c3bb6-129">次の表に、deviceConfigurationAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c3bb6-129">The following table shows the properties that are required when you create the deviceConfigurationAssignment.</span></span>

|<span data-ttu-id="c3bb6-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c3bb6-130">Property</span></span>|<span data-ttu-id="c3bb6-131">型</span><span class="sxs-lookup"><span data-stu-id="c3bb6-131">Type</span></span>|<span data-ttu-id="c3bb6-132">説明</span><span class="sxs-lookup"><span data-stu-id="c3bb6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3bb6-133">id</span><span class="sxs-lookup"><span data-stu-id="c3bb6-133">id</span></span>|<span data-ttu-id="c3bb6-134">String</span><span class="sxs-lookup"><span data-stu-id="c3bb6-134">String</span></span>|<span data-ttu-id="c3bb6-135">割り当てのキー。</span><span class="sxs-lookup"><span data-stu-id="c3bb6-135">The key of the assignment.</span></span>|
|<span data-ttu-id="c3bb6-136">target</span><span class="sxs-lookup"><span data-stu-id="c3bb6-136">target</span></span>|[<span data-ttu-id="c3bb6-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c3bb6-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c3bb6-138">デバイス構成の割り当て先。</span><span class="sxs-lookup"><span data-stu-id="c3bb6-138">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="c3bb6-139">応答</span><span class="sxs-lookup"><span data-stu-id="c3bb6-139">Response</span></span>
<span data-ttu-id="c3bb6-140">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c3bb6-140">If successful, this method returns a `201 Created` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3bb6-141">例</span><span class="sxs-lookup"><span data-stu-id="c3bb6-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="c3bb6-142">要求</span><span class="sxs-lookup"><span data-stu-id="c3bb6-142">Request</span></span>
<span data-ttu-id="c3bb6-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c3bb6-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c3bb6-144">応答</span><span class="sxs-lookup"><span data-stu-id="c3bb6-144">Response</span></span>
<span data-ttu-id="c3bb6-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c3bb6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





